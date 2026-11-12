# Projeto Secure

Site educativo de conscientização sobre segurança digital, desenvolvido como atividade acadêmica. O objetivo é explicar situações comuns do ambiente digital, apresentar os riscos mais frequentes e mostrar atitudes simples que ajudam a proteger dados e dispositivos.

## Conteúdos

| Página | Arquivo | Situação |
| --- | --- | --- |
| Início | `index.html` | Pronta |
| Phishing e engenharia social | `phishing.html` | Pronta |
| Segurança com IA (quiz) | `ia.html` | Pronta |
| Software e aplicativos | `software.html` | Pendente |
| Segurança de dispositivos | `dispositivos.html` | Pendente |
| Senhas e MFA | `senhas.html` | Pendente |
| Proteção de dados | `dados.html` | Pendente |
| Wi-Fi e conexões | `wifi.html` | Pendente |

Os links das páginas pendentes já estão no menu de navegação.

## Estrutura do projeto

```
projeto-secure/
├── index.html
├── phishing.html
├── ia.html
├── software.html
├── dispositivos.html
├── senhas.html
├── dados.html
├── wifi.html
├── style.css
└── README.md
```

Todas as páginas compartilham o mesmo `style.css`.

## Como executar

Não é necessário instalar nada.

1. Baixe ou clone o projeto.
2. Mantenha todos os arquivos na mesma pasta.
3. Abra o `index.html` no navegador.

As fontes são carregadas do Google Fonts, por isso é preciso estar conectado à internet para vê-las. Sem conexão, o site usa fontes do sistema.

## Tecnologias

- HTML5
- CSS3, com variáveis, Grid, Flexbox, animações e media queries
- Google Fonts: Bricolage Grotesque (títulos) e Figtree (textos)

Não há JavaScript nem bibliotecas externas. O quiz funciona só com HTML e CSS.

## Identidade visual

| Cor | Hexadecimal | Uso |
| --- | --- | --- |
| Azul-marinho | `#1C1C85` | Textos, botões, rodapé e destaques |
| Rosa claro | `#F5E6E8` | Fundos de seções e cartões |
| Roxo | `#A243AC` | Item ativo do menu, alertas e detalhes |
| Azul médio | `#7192BE` | Bordas e sombras |
| Azul aço | `#4D7EA8` | Textos secundários |
| Branco | `#FFFFFF` | Fundo geral |

As cores ficam como variáveis no início do `style.css` (`:root`).

## Organização do CSS

- **Variáveis** no `:root` para cores e fontes.
- **Componentes compartilhados:** cabeçalho, menu, botões, cartões, seções de exemplo, dicas, quadro de lembrete e rodapé.
- **Variações por página:** cada `<body>` recebe uma classe que muda o layout do hero.
  - `page-home`: hero padrão.
  - `page-phishing`: hero espelhado, com destaque em roxo.
  - `page-ia`: hero em coluna única, seguido do quiz.
- **Quiz:** as alternativas são `input type="radio"` estilizados pelo `label`, e o gabarito usa `<details>`.
- **Responsividade:** ajustes em 900px e 700px. No celular o menu rola na horizontal.
- **Acessibilidade:** foco visível no teclado, textos alternativos por `aria-label` e `aria-hidden` nos elementos decorativos, e animações desativadas para quem pede "reduzir movimento" no sistema.

## Equipe

- André Rocha
- Eyshila Marques
- Giovanna Sanches
- Gustavo Rodrigues
- Jenifer Ferreira
- Julia Gonçalves
- Thiago Araujo

## Contexto

Conteúdo educativo desenvolvido para atividade acadêmica. Os exemplos de golpes exibidos no site são fictícios e servem apenas para fins didáticos.
