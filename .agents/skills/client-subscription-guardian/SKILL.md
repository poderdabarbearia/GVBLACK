---
name: client-subscription-guardian
description: Protege assinaturas de clientes finais, validade, frequência, dias permitidos, consumo de benefícios e bloqueios.
---
# Client Subscription Guardian
Não confundir assinatura do cliente final com billing SaaS. Fonte de verdade: assinatura canônica → plano → pagamento/status → início/vencimento → data solicitada → dias permitidos → franquia → usos/agendamentos → autorização atômica. A checagem final deve existir server-side e ser concorrente-safe em todos os canais, inclusive WhatsApp/IA. Remarcação exclui o próprio agendamento da contagem. Preserve objetos existentes e teste quota, vencimento, dias proibidos, cancelamento/no-show, concorrência e isolamento tenant.