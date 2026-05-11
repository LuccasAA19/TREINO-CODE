# CLAUDE.md

Instruções e contexto para o Claude Code ao trabalhar neste repositório.

## Visão geral

Este é o repositório `TREINO-CODE`, um ambiente de treino e experimentação com o Claude Code. Não há aplicação principal definida ainda — o repositório é usado para testar fluxos, comandos, hooks, e a memória persistente do agente.

## Idioma

- Toda comunicação com o usuário deve ser em **português (Brasil)**, salvo pedido contrário.
- Código pode permanecer em inglês (nomes de variáveis, funções), mas comentários e docs ficam em português.

## Memória

- O arquivo `memory.md` é a memória persistente desta workspace.
- **Sempre leia `memory.md` no início de uma sessão** para recuperar contexto, preferências e histórico.
- **Atualize `memory.md`** sempre que:
  - O usuário compartilhar uma nova preferência ou decisão.
  - Surgir contexto relevante que valha a pena lembrar entre sessões.
  - Uma tarefa relevante for concluída ou ficar pendente.
- Mantenha as seções existentes de `memory.md`; adicione conteúdo em vez de reescrever do zero.

## Convenções de código

- Indentação: 2 espaços (default; ajustar se a linguagem do projeto pedir outro padrão).
- Sem comentários supérfluos — apenas onde o "porquê" não for óbvio.
- Não criar arquivos `.md` extras (planos, resumos, decisões) sem pedido explícito do usuário.

## Convenções de git

- Branch de desenvolvimento ativa: `claude/create-memory-docs-Zx4VR`.
- Commits curtos e descritivos, focados no "porquê".
- Nunca usar `--no-verify`, `--force` ou operações destrutivas sem autorização explícita.
- Não abrir Pull Request a menos que o usuário peça.

## Estilo de resposta

- Respostas concisas, sem floreios.
- Usar ferramentas livremente quando ajudar a resolver melhor o problema — o usuário já autorizou esse estilo.
- Quando uma ação for arriscada (destrutiva, irreversível, ou afeta estado compartilhado), confirmar antes.

## Estrutura do repositório

```
.
├── CLAUDE.md     # este arquivo (instruções para o Claude)
└── memory.md     # memória persistente entre sessões
```

Quando novos diretórios ou arquivos relevantes forem criados, atualizar esta seção.
