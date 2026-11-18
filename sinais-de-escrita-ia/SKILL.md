---
name: sinais-de-escrita-ia
description: >-
  Diagnostica padrões de redação associados a modelos de linguagem em textos e edições da Wikipédia, apoia revisão editorial e audita edições distinguindo verificações documentais de inferências estilísticas. Use quando o usuário pedir para examinar um texto, trecho, resumo de edição ou diff em busca desses padrões, revisar a redação preservando os fatos ou verificar fontes e alterações de uma edição.
---

# Sinais de escrita por IA

Skill em português para **diagnóstico**, **revisão editorial** e **auditoria de edições**. É uma
síntese do guia do WikiProject AI Cleanup, [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).

Para identificar um padrão específico, consulte [`references/catalogo.md`](references/catalogo.md)
e leia também os falsos positivos daquela seção. Este arquivo descreve o método; o catálogo
contém os sinais, os exemplos em inglês e as ressalvas detalhadas.

## Princípios

- **Padrão não prova autoria.** Não conclua que uma pessoa usou IA, não acuse ninguém e não
  atribua uma porcentagem de autoria. Um marcador técnico pode indicar resíduo de uma ferramenta
  ou de uma etapa de edição, mas, por si só, não identifica quem o produziu nem como foi usado.
- **Separe observação, verificação e inferência.** Um traço estilístico é uma observação, não um
  fato documental. Só diga que uma fonte confirma uma afirmação depois de conferir a fonte.
- **A fonte trata principalmente do inglês.** Não aplique mecanicamente ao português as listas
  lexicais do original. Priorize sinais estruturais e trate semelhanças lexicais como hipóteses.
- **Considere contexto e data.** Os padrões mudam entre ferramentas, épocas, gêneros e pessoas.
  Leia o texto inteiro e examine o histórico quando a tarefa envolver uma edição.
- **O catálogo é descritivo, não uma política editorial.** Corrigir um sinal superficial não
  substitui apurar fatos, avaliar fontes ou seguir as regras da comunidade pertinente.

## Fluxo de trabalho

1. **Delimite a tarefa.** Identifique o material e escolha um dos três modos abaixo. Se o pedido
   for ambíguo, pergunte; não presuma que o usuário quer um diagnóstico de autoria.
2. **Leia o material por inteiro.** Para uma edição, reúna o diff, a versão anterior e posterior,
   o resumo e o histórico disponíveis. Se faltarem dados essenciais, declare a limitação ou peça-os.
3. **Consulte o catálogo.** Abra a seção pertinente em `references/catalogo.md` e verifique seus
   falsos positivos antes de relatar um sinal.
4. **Registre evidências.** Para cada observação, cite um trecho curto ou indique o elemento
   verificável (por exemplo, um link quebrado ou parâmetro de URL). Não infira além dele.
5. **Separe os tipos de achado.** Use, quando útil:
   - **Marcador técnico:** resíduo, placeholder ou sintaxe anômala; descreva o que está presente,
     sem transformar isso em prova de autoria.
   - **Combinação de padrões:** vários sinais independentes no mesmo contexto; ainda não é prova.
   - **Traço isolado:** sinal fraco, comum também em escrita humana.
6. **Responda no formato do modo escolhido** e indique o que continua sem verificação.

## Modo 1 — Diagnóstico

**Objetivo:** descrever padrões observáveis em um texto, sem concluir quem o escreveu.

- Leia o trecho no contexto; para texto longo, considere a estrutura e a distribuição dos sinais.
- Selecione apenas padrões sustentados por evidência textual e cite cada trecho observado.
- Diferencie marcador técnico, combinação de padrões e traço isolado. Explique os falsos positivos
  plausíveis, em vez de somar sinais como se fossem uma pontuação de autoria.
- Declare os limites do material: por exemplo, um excerto não informa a origem nem o histórico
  de edição.
- Não reescreva o texto, salvo se o usuário também pedir revisão.

## Modo 2 — Revisão editorial

**Objetivo:** tornar a redação mais específica, clara e verificável, preservando os fatos.

- Preserve o sentido e os fatos fornecidos. Não acrescente informação para preencher lacunas;
  não elimine uma afirmação factual só por ela soar genérica sem indicar a mudança.
- Remova ou qualifique generalizações, repetição, linguagem promocional e análise sem apoio,
  explicando as alterações.
- Não invente fontes, autores, títulos, URLs, DOIs ou ISBNs. Marque afirmações que precisam de
  comprovação como **[fonte necessária]** e liste-as ao final.
- Se não puder verificar uma afirmação, mantenha a incerteza explícita e sugira o tipo de fonte
  que seria necessário consultar.
- Não altere a voz do autor além do necessário para o objetivo solicitado.

**Entregue:** texto revisado; alterações principais e motivos; afirmações que precisam de fonte.

## Modo 3 — Auditoria de edição

**Objetivo:** examinar uma edição da Wikipédia e separar o que foi verificado do que apenas se
parece com padrões do catálogo.

- Identifique a página, a revisão ou o diff e o intervalo examinado. Se só houver um link, abra
  e confira o material acessível; não suponha o conteúdo de revisões que não conseguiu consultar.
- Verifique documentalmente a sintaxe, os links, os identificadores bibliográficos e as fontes
  citadas, na medida em que o material permita. Para avaliar se uma fonte sustenta uma frase,
  leia a fonte; a presença de uma citação não basta.
- Organize os resultados em três blocos:
  - **Verificado:** fatos diretamente conferidos (por exemplo, link que não abre, placeholder
    literal, referência incompatível com o identificador ou afirmação não sustentada pela fonte
    consultada).
  - **Padrão de estilo:** semelhanças com o catálogo, sem tratá-las como prova de origem.
  - **A verificar:** questões que dependem de fonte, histórico ou contexto ainda não consultado.
- Distinga correções mecânicas de decisões editoriais que dependem das políticas e da comunidade
  da Wikipédia. Termine com ações sugeridas em ordem de prioridade.

## Formato de resposta

Adapte a extensão ao pedido. Omita seções que não se aplicam; nunca preencha lacunas com suposições.

### Diagnóstico

```markdown
## Material e objetivo
<texto/trecho analisado e escopo>

## Padrões observados
| Padrão | Evidência | Tipo | Ressalva / falso positivo |
|---|---|---|---|
| … | “…” | Traço isolado / combinação / marcador técnico | … |

## Limites
<o que o material não permite verificar ou concluir>
```

### Revisão editorial

```markdown
## Texto revisado
<versão revisada, com [fonte necessária] onde couber>

## Alterações
| Trecho | Mudança | Motivo |
|---|---|---|
| … | … | … |

## Afirmações que precisam de fonte
- …
```

### Auditoria

```markdown
## Escopo
<página, diff/revisão e material consultado>

## Verificado
- …

## Padrões de estilo
- …

## A verificar
- …

## Ações sugeridas
1. …
```

## Uso sem suporte nativo a skills

Forneça **os dois arquivos Markdown** como contexto: este `SKILL.md` explica o método e
`references/catalogo.md` contém o repertório de padrões. Preserve essa relação e consulte o
catálogo para cada sinal específico; não é necessário copiar todo o catálogo para este arquivo.
