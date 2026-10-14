> Atualizado: as tarefas agora leem e gravam nas tabelas `jv_*` do Supabase (via conector Supabase, `execute_sql`), não mais no armazenamento do artifact. Onde este texto disser "db do artifact", leia "tabela jv_* correspondente" (jv_memoria, jv_leads, jv_briefing, jv_saas_pedidos, jv_config).

# Tarefas agendadas do Jarvis

| Tarefa | Quando (America/Recife) | Prompt |
|---|---|---|
| Briefing do Jarvis | todo dia 06:56 | briefing.md |
| Relatório MaisOdonto | todo dia (ex.: 08:54) | relatorio-maisodonto.md |
| Turno do Jarvis | a cada 2 horas, aos 3 min | turno.md |
| Ideias de SaaS | a cada hora, aos 19 min | ideias-saas.md |
| Gerador de SaaS | sob demanda (botão Gerar no painel) | gerador-saas.md |

Agenda dos turnos: 00h, 02h e 04h prospecção; 06h produção; 08h resumo; 10h, 14h e 18h follow-up; 12h e 16h pesquisa; 20h aprovações; 22h fechamento (domingo com placar semanal).

Toda a memória é lida e gravada com a ferramenta ArtifactData no artifact do painel, collection `memoria`. O `doc_id` é o caminho com "/" trocado por "__".
