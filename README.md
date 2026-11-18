# ensinado

Repositório da skill **Sinais de escrita por IA**, baseada no guia editorial da Wikipédia em inglês. A skill está em português e ajuda a diagnosticar padrões de redação, revisar textos e auditar edições da Wikipédia — sem tratar esses padrões como prova de autoria.

## Arquivos

| Arquivo | Conteúdo |
|---|---|
| [`sinais-de-escrita-ia/SKILL.md`](sinais-de-escrita-ia/SKILL.md) | Instruções da skill, três modos de análise, fluxo de trabalho e formatos de resposta. |
| [`sinais-de-escrita-ia/references/catalogo.md`](sinais-de-escrita-ia/references/catalogo.md) | Síntese dos padrões de conteúdo, linguagem, formatação, referências e histórico; inclui falsos positivos e exemplos em inglês. |

## Como usar

Importe a pasta `sinais-de-escrita-ia` em uma ferramenta compatível com Agent Skills. Se a ferramenta não aceitar skills, forneça os **dois arquivos Markdown** como contexto e mantenha a relação entre eles: o `SKILL.md` traz o método; `references/catalogo.md` reúne os padrões detalhados.

Depois, envie um texto, trecho ou link e indique o objetivo. Por exemplo:

- **Diagnóstico:** “Analise este trecho e cite os padrões observados, sem concluir quem o escreveu.”
- **Revisão editorial:** “Revise este texto para torná-lo mais específico. Preserve os fatos e sinalize o que precisar de fonte.”
- **Auditoria:** “Examine esta edição da Wikipédia. Distinga o que verificou nas fontes do que é apenas um padrão de estilo.”

**Os sinais não provam autoria.** As observações lexicais da fonte se referem principalmente ao inglês e não devem ser aplicadas mecanicamente ao português.

## Fonte

- [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), do WikiProject AI Cleanup.
- [Revisão consultada (18 de novembro de 2026)](https://en.wikipedia.org/w/index.php?title=Wikipedia:Signs_of_AI_writing&oldid=1386452058). O catálogo é uma síntese em português; consulte o original para exemplos e referências da Wikipédia.
