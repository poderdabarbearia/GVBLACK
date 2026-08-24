---
name: bug-forensics
description: Investiga bugs e falhas complexas até encontrar causa-raiz comprovada antes de corrigir.
---
# Bug Forensics
Trace UI → rota/estado → service/API → Edge/RPC → schema → RLS/grants → dados → integração → retorno. Localize o primeiro ponto onde observado diverge do esperado. Verifique tenant, contratos, tipos, status, cache, timing, retry, concorrência, idempotência, env, secrets e provider. Não crie migration/fallback por hipótese. Classifique causa como PROVADA, MUITO_PROVÁVEL ou HIPÓTESE e achados P0-P3. Depois use `safe-code-change` para o menor delta.