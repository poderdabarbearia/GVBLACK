---
name: whatsapp-scheduling-engine
description: Implementa, consolida e homologa motor conversacional WhatsApp com IA para atendimento, dúvidas, suporte, agendamento, remarcação, cancelamento e grupos selecionados.
---
# WhatsApp Scheduling Engine V2
Mantenha um único motor. Audite ABSENT/FRAGMENTED/PARTIAL/FUNCTIONAL_UNHOMOLOGATED/HOMOLOGATED; em tentativa existente use REPAIR_AND_CONSOLIDATE. Trace `provider → webhook autenticado → tenant/instance server-side → inbound dedup → policy direct/group → conversation claim → durable state → deterministic/LLM → knowledge/tools → disponibilidade/ação → confirmação → commit → outbound/worker`.

Contatos novos podem perguntar sem cadastro forçado. Autoridade de conhecimento: dados estruturados → documentação oficial → RAG tenant → contexto → LLM para interpretar/redigir. Determinístico primeiro para negações, sim/não, opções, datas, horários e quoted replies. Agenda server-authoritative, slots completos e commit concorrente-safe. Booking/remarcação/cancelamento exigem confirmação explícita; `business_action_committed` não pode repetir ação por falha posterior.

Exactly-once: inbound único, uma run, um processing/conversa, uma resposta/inbound, idempotency key e context_version. Grupos são opt-in; preserve group_jid e participant_jid, contexto por participante e privacidade; dados privados vão para fluxo seguro/privado. Human mode durável; retry pré-I/O, uncertain sem resend cego. Segurança: webhook protegido, RLS, tenant server-side, service_role backend only, SECURITY DEFINER/grants seguros. Sem E2E real: FUNCTIONAL_UNHOMOLOGATED.