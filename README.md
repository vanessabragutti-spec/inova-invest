# Inova+Invest — Design System

Design system dos **materiais** do Inova+Invest (posts, slides, one-pagers, banners, e-mails). Versão navegável: https://claude.ai/artifact/CFBB7KqZahpfgeFNrAeYZX

## Estrutura do repositório

| Caminho | O que é |
|---|---|
| `styles.css` | Ponto de entrada. Importa `tokens/tokens.css` e `componentes/componentes.css`. Carregue só este arquivo. |
| `tokens/tokens.css` | Variáveis CSS de cor, espaçamento, raio e medidas de marca, e as classes de tipografia (`.display`, `.titulo-1`, `.titulo-2`, `.titulo-3`, `.numero`, `.lead`, `.corpo`, `.legenda`, `.etiqueta`). O tema claro é o padrão; `data-theme="azul"` num contêiner troca para o tema de fundo azul. |
| `tokens/tokens.json` | Os mesmos tokens em JSON, com a nota de uso de cada um. |
| `componentes/componentes.css` | Classes dos componentes: `ii-etiqueta`, `ii-botao`, `ii-assinatura`, `ii-agenda`, `ii-palestrante`, `ii-destaque`, `ii-peca`, `ii-trapezio`, `ii-mais`. |
| `componentes/<nome>/` | Um exemplo HTML (`exemplo.html`) e as regras de uso (`README.md`) de cada componente: etiqueta, botao, assinatura, agenda, palestrante, destaque, post-feed, slide, capa. |
| `assets/logos/` | As 6 versões do logo Inova+Invest (PNG transparente). |
| `assets/assinatura/` | ABVCAP, trio ApexBrasil + Governo do Brasil, ACE Ventures. |
| `assets/grafismos/` | Trapézio verde (19°) e sinal + (SVG). |
| `referencias/` | Guia de ID visual Inova+Invest e Brandbook ApexBrasil Projetos Setoriais 2025, as fontes deste sistema. |
| `arquivos-originais/` | Matrizes recebidas (AI, PDF, PSD, JPG, PNG) para impressão e edição. Não são usadas diretamente pelo sistema. |

Fonte oficial: **Museo Sans 500 e 700**. Os arquivos da fonte não estão neste pacote por licença; instale no computador para produzir as peças. Substituta em tela: Nunito Sans (Google Fonts).

O Inova+Invest é um Projeto Setorial da ABVCAP em convênio com a ApexBrasil, com a ACE Ventures como parceira. O programa prepara startups para captar investimento e as conecta a investidores qualificados. Este sistema serve para **materiais**: posts, slides, one-pagers, banners de evento e e-mails. Toda peça segue duas fontes ao mesmo tempo: o guia de ID visual do Inova+Invest e o Brandbook de Projetos Setoriais 2025 da ApexBrasil.

## Princípios

- **O projeto lidera.** O logo Inova+Invest é a marca principal da peça. As outras marcas entram só no bloco de assinatura (veja Assinatura).
- **Azul manda, verde soma.** `azul` ocupa a maior área. `verde` aparece pouco e sempre como acento: o +, o trapézio, um número, o botão.
- **Cantos retos, ângulo de 19°.** A marca é feita de retas. Use `radius-0` em tudo, exceto botões e etiquetas (`radius-1`). O único ângulo é o `grafismo-inclinacao` (19°), o mesmo do acento do á.

## Conteúdo e voz

- Escreva em português, frases curtas e diretas, falando com o founder em segunda pessoa ("sua startup").
- **Sem caixa alta em títulos e chamadas** (regra ApexBrasil). Caixa alta só em etiquetas e botões, com o estilo `etiqueta`.
- **Alinhe o texto à esquerda.** Nunca justifique nem centralize texto corrido.
- Escreva o nome sempre **Inova+Invest**, com o + e sem espaços. Escreva **ApexBrasil** junto, sem hífen. Em textos longos, apresente uma vez por extenso: "Agência Brasileira de Promoção de Exportações e Investimentos (ApexBrasil)".
- Use dados concretos: "Inscrições até 02/02/2026", "faturamento anual a partir de ~R$ 500 mil", "28 de janeiro de 2026, 17h às 18h, online".
- Não use emoji em peças gráficas. Em legenda de post, no máximo um por bloco de informação (📅, 📍).

## Cor

- Dois temas: **Fundo claro** (`fundo` branco) e **Fundo azul** (`fundo` = `azul`). Cada peça escolhe um. Em campanha, alterne os dois.
- Para texto use `texto` sobre `fundo` ou `fundo-alt`. Para cargos e metadados use `texto-suave`.
- Destaque uma palavra ou número com `texto-destaque`. No fundo claro ele vira `verde-escuro`, porque o verde oficial sobre branco não passa em contraste.
- **Nunca coloque texto branco sobre verde** (2,05:1). Sobre `acento`, use sempre `sobre-acento` (azul, 6,95:1).
- `preto` e `cinza` servem só para as versões monocromáticas do logo e para impressão a 1 cor.
- Cores oficiais para impressão: Azul C100 M85 K25 (Pantone 280 C / 287 U) e Verde C65 Y100 (Pantone 376 C / 381 U). Em tela use os HEX dos tokens.

## Tipografia

- A família oficial é **Museo Sans** (500 e 700), a mesma do guia de ID visual. Enquanto os arquivos da fonte não estiverem no sistema, as prévias usam **Nunito Sans** como substituta. Em peças finais, instale a Museo Sans.
- Use `display` uma vez por peça, para a chamada principal. Use `titulo-1` a `titulo-3` para a hierarquia, `corpo` para texto corrido e `legenda` para cargos e créditos.
- Use `numero` para datas, valores e prazos que são o ponto da peça. Pinte com `texto-destaque` ou `texto`.
- Limite as linhas de texto corrido a uns 65 caracteres.

## Logo

- Use os arquivos de **Logos**, nunca redesenhe a marca. Escolha a versão pelo fundo:
  - fundo branco ou claro: `inova-invest-cor`
  - fundo azul: `inova-invest-negativa` (branca com + verde)
  - fundo escuro ou foto escura: `inova-invest-negativa`, ou `inova-invest-branca` quando o verde brigar com a imagem
  - impressão em 1 cor ou P&B: `inova-invest-preta`, `inova-invest-cinza`, `inova-invest-cinza-negativa`
- **Área de proteção:** deixe livre em volta do logo a altura da letra "v" de "inova", nos quatro lados.
- **Tamanho mínimo:** `logo-min-tela` (100 px) e `logo-min-impresso` (15 mm).
- Não distorça, não gire, não troque as cores, não separe o + do nome, não aplique sombra nem contorno, não coloque sobre fundo poluído.

## Assinatura

- Peças oficiais levam o bloco de assinatura no rodapé, numa ordem fixa: **Inova+Invest → ABVCAP → ApexBrasil + Ministério + Governo Federal**. A ACE Ventures, parceira, entra depois, separada, sob o rótulo "Parceria".
- Use os arquivos de **Assinatura**. O trio ApexBrasil/Governo vai sempre na versão colorida em fundo claro (`apex-gov-horizontal-cor`). A versão negativa (`apex-gov-horizontal-negativa`) só entra em fundo azul ou escuro.
- Nenhuma marca do bloco pode passar da altura nem da largura da marca ApexBrasil. A marca ApexBrasil não pode ficar menor que `apex-min-tela` (35 px) ou `apex-min-impresso` (7 mm).
- A marca Brasil só aparece em ações no exterior ou para público estrangeiro.
- Peças com o bloco de assinatura vão para aprovação da ApexBrasil antes de publicar: valida@apexbrasil.com.br.

## Grafismos

- **Trapézio verde** (`trapezio-verde`): um bloco de `acento` com a lateral inclinada a 19°, sangrando por uma borda da peça (canto inferior esquerdo, como na capa do guia). No máximo um por peça.
- **Sinal +** (`sinal-mais-verde`, `sinal-mais-azul`): o + do logo como marcador de lista, ícone de "benefício" ou elemento grande recortado pela borda. Mantenha a proporção original.
- Não misture trapézio e + grandes na mesma peça. Escolha um como protagonista.

## Layout

- Margem interna de post e slide: `space-6` (48 px a 1080 px de largura). Entre seções: `space-7`.
- Blocos e fotos de cantos retos (`radius-0`). Fotos de palestrante podem usar `radius-foto` (círculo).
- Sem sombras e sem degradês. A profundidade vem de `fundo-alt` e da troca entre fundo claro e fundo azul.
- Agrupe informações práticas (data, horário, formato) num bloco só, sempre no mesmo lugar da série.

## Iconografia

- O sistema não tem um conjunto de ícones próprio. Use o + como marcador. Quando precisar de ícone, use traço simples, monolinha, na cor `texto` ou `texto-destaque`.
