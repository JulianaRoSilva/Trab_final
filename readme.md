# 🎃 Portal Halloween: filmes e séries de terror

Projeto educacional de versionamento com Git e GitHub: um pequeno portal sobre filmes e séries de terror para uma maratona de Halloween.

## Objetivo

Praticar o fluxo de trabalho com Git e GitHub em um projeto simples, usando branches, commits, merges, resolução de conflitos, Pull Requests, tags e releases. O conteúdo do portal (filmes fictícios e sugestões de séries) serve apenas de apoio para esse exercício.

## Tecnologias utilizadas

- **HTML5 e CSS3**: estrutura e estilo das páginas
- **JavaScript**: validação simples do formulário de cadastro
- **Git**: controle de versão local
- **GitHub**: repositório remoto, Pull Requests e releases
- **VS Code**: editor de código

## Estrutura dos arquivos

```
Trab_final/
├── index.html      # Página inicial do portal
├── series.html     # Sugestões de séries de terror
├── cadastro.html   # Formulário de cadastro (demonstração)
├── Readme.md       # Documentação do projeto
└── .gitignore      # Itens locais que não entram no repositório
```

## Como abrir o portal

1. Clone o repositório ou baixe os arquivos:
   ```bash
   git clone https://github.com/JulianaRoSilva/Trab_final.git
   ```
2. Abra a pasta `Trab_final`.
3. Dê um duplo clique no arquivo `index.html` para abri-lo no navegador.
4. Use o menu no topo para navegar entre **Início**, **Séries** e **Cadastro**.

Não é necessário instalar nada nem rodar um servidor.

> **Aviso:** o formulário de cadastro é apenas uma demonstração. Nenhum dado é enviado, armazenado ou compartilhado.

## Branches

| Branch | Função |
| --- | --- |
| `main` | Versão estável do projeto. Só recebe código pronto, vindo da `develop`. |
| `develop` | Branch de integração, onde as funcionalidades são reunidas antes de ir para a `main`. |
| `feature/series` | Desenvolvimento da página `series.html`. |
| `feature/cadastro` | Desenvolvimento da página `cadastro.html`. |
| `fix/correcao` | Correção do texto de destaque do `index.html`, que gerou um conflito de merge. |

As branches `feature/series`, `feature/cadastro` e `fix/correcao` partem da `develop`.

## Estratégia de Pull Requests

- Cada funcionalidade é integrada à `develop` por meio de um Pull Request próprio:
  - `feature/series` → `develop`
  - `feature/cadastro` → `develop`
- Antes de confirmar, conferimos a branch de origem, a branch de destino e os arquivos alterados.
- A correção (`fix/correcao`) foi integrada localmente na `develop`, com a resolução manual do conflito, por isso não precisou de Pull Request.
- Depois que as funcionalidades estão reunidas e testadas, um último Pull Request leva a `develop` para a `main`.

## Histórico de versões

| Versão | Descrição |
| --- | --- |
| `v0.1.0` | **Versão inicial do portal**: `index.html`, `Readme.md` e `.gitignore`, antes das funcionalidades. |
| `v1.0.0` | **Portal Halloween completo**: páginas de séries e cadastro, além da correção do texto de destaque. |

## Autora

Juliana Rodrigues: [github.com/JulianaRoSilva](https://github.com/JulianaRoSilva)