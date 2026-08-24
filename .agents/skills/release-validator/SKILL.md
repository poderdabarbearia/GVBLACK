---
name: release-validator
description: Valida uma alteração antes de merge, deploy ou produção.
---
# Release Validator
Revise diff, arquivos inesperados, secrets, contratos e dependências. Execute quando aplicável formatter, lint, typecheck, testes, SQL contracts, build e smoke. Banco: schema físico, RLS A→A/A→B, grants, SECURITY DEFINER, triggers e Edge. Resultados: PASSOU, FALHOU, NÃO_EXECUTADO ou NÃO_APLICÁVEL. Merge ≠ deploy ≠ produção.