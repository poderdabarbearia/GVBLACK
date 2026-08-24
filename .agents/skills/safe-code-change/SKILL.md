---
name: safe-code-change
description: Executa correções mínimas e seguras após causa-raiz identificada.
---
# Safe Code Change
Pré-condição: projeto/repo, implementação atual, causa e menor delta confirmados. Reaproveite objetos existentes; não duplique módulos; preserve contratos, rotas, tipos e mudanças do usuário; sem refatoração fora do escopo; não desabilite RLS nem exponha service_role; não use browser como autoridade financeira; não crie fallback para esconder falha. Valide lint/typecheck/testes/SQL/build/smoke.