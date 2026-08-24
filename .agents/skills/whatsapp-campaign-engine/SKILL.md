---
name: whatsapp-campaign-engine
description: Implementa e consolida campanhas/disparos WhatsApp para contatos, segmentos, equipes e grupos selecionados com fila durável, pacing, idempotência e integração conversacional.
---
# WhatsApp Campaign Engine
Audite antes de criar e nunca instale segundo worker/campaign motor sobre um existente. Trace `campaign → audience snapshot → jobs → claim → pre-send validation → provider → delivery → inbound reply → whatsapp-scheduling-engine`. Responsabilidades: audiência, snapshot, templates, jobs duráveis, claim atômico, pacing/quiet-hours, pause/resume/cancel, prioridade de filas, delivery, retry seguro, métricas e grupos selecionados. Grupo usa JID canônico, nunca telefone derivado; discovery não auto-habilita. Default `MENTION_ONLY`; ALL_MESSAGES só com opt-in explícito. Falha pré-I/O pode retry; envio incerto nunca recebe retry cego. Respostas entram no mesmo motor conversacional. Sem provider/grupo real: FUNCTIONAL_UNHOMOLOGATED.