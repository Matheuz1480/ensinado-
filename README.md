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

## Publicar no GitHub pelo navegador

O arquivo `ensinado.zip` é um pacote local com o README e a pasta da skill; não o envie ao GitHub. Para criar um repositório novo e enviar os arquivos pelo site:

1. Extraia `ensinado.zip`. Você verá `README.md` e a pasta `sinais-de-escrita-ia`.
2. Entre na sua conta e abra [github.com/new](https://github.com/new).
3. Escolha a conta proprietária, digite `ensinado` em **Repository name** e selecione **Public** se quiser disponibilizá-lo para todos. Não inicialize com README, `.gitignore` ou licença; o repositório precisa começar vazio para este método.
4. Clique em **Create repository**. Na página seguinte, escolha **uploading an existing file** (ou, num repositório já iniciado, **Add file → Upload files**).
5. Envie o `README.md` e a pasta `sinais-de-escrita-ia` extraídos. **Não envie o ZIP.** Confira que `SKILL.md` está dentro da pasta da skill e que `catalogo.md` está dentro de `references/`.
6. Escreva uma mensagem de commit, por exemplo `Adiciona skill e catálogo`, e clique em **Commit changes**. Confira se o README aparece na página inicial e se os dois links da tabela acima abrem corretamente.

## Alternativa pelo terminal

Crie primeiro um repositório vazio no GitHub. Com o Git instalado, abra um terminal na pasta extraída que contém `README.md` e substitua `SEU-USUARIO` pelo seu usuário ou organização:

```sh
git init -b main
git add README.md sinais-de-escrita-ia
git commit -m "Adiciona skill e catálogo"
git remote add origin https://github.com/SEU-USUARIO/ensinado.git
git push -u origin main
```

Faça a autenticação pelo gerenciador de credenciais do Git ou pelo GitHub CLI. **Não compartilhe tokens ou senhas.**

## Fonte

- [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), do WikiProject AI Cleanup.
- [Revisão consultada (18 de novembro de 2026)](https://en.wikipedia.org/w/index.php?title=Wikipedia:Signs_of_AI_writing&oldid=1386452058). O catálogo é uma síntese em português; consulte o original para exemplos e referências da Wikipédia.
