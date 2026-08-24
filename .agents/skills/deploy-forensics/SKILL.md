---
name: deploy-forensics
description: Diagnostica divergências entre GitHub, build, Lovable, preview, deploy público, assets e cache.
---
# Deploy Forensics
Estabeleça a fonte de verdade: commit da main, source GitHub, source Lovable, CI/build, preview e produção. Diferencie código incorreto, dependência/lock, build, erro literal injetado, CSS/assets ausentes, sync stale, deploy stale, cache e runtime/secrets. Sequência: evidência → hipótese → verificação → delta mínimo → CI → merge → sync → deploy → verificação final. Build verde não prova produção atualizada; merge não prova deploy.