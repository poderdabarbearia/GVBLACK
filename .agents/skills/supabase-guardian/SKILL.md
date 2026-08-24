---
name: supabase-guardian
description: Protege Supabase: schema, migrations, RLS, RPCs, triggers, grants, Edge e PostgREST.
---
# Supabase Guardian
Antes de SQL classifique: código incorreto; migration ausente/não aplicada/parcial; schema físico divergente; cache PostgREST; RLS; grant; SECURITY DEFINER; dados; ambiente; Edge antiga; secret/config. Não recrie objetos existentes. SECURITY DEFINER exige search_path seguro, auth/membership/role/tenant e grants mínimos. service_role só backend. Reporte migration versionada e aplicada separadamente.