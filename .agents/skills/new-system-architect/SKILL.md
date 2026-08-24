---
name: new-system-architect
description: Arquitetura novos sistemas e SaaS com PODER PLATFORM CORE antes de código.
---
# New System Architect
Antes de implementar: classifique B2C/B2B/B2B2B; defina tenant, payer, usuários e roles; separe Core, módulos de plataforma e vertical; classifique CORE-01..15; defina billing, segurança, eventos, auditoria e Quality Gate. Reuse invariantes das referências oficiais sem copiar migrations cegamente. Sistema existente: AUDITAR → comparar → preservar → delta mínimo → implementar → validar.