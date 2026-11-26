# Imagens Didáticas

<img src="assets/icon-small.png" width="64" height="64" alt="Ícone do ImageGen com uma pilha de três livros">

Skill para planejar, produzir, revisar e auditar imagens didáticas no Codex. Use um material de referência, uma norma, um edital ou uma imagem existente para definir o que cada prancha precisa ensinar e como representar seus conceitos.

## Instalação no Codex

1. Extraia o ZIP e coloque a pasta **imagens-didaticas** em **~/.codex/skills/**. O arquivo [SKILL.md](SKILL.md) fica diretamente dentro da pasta da skill.
2. No Codex, mencione **$imagens-didaticas** na sua solicitação.

A produção visual usa exclusivamente o ImageGen integrado ao Codex por padrão. Isso inclui reunir os blocos, inserir títulos e rótulos e desenhar setas. Código e SVG são opções sob pedido. O planejamento e a auditoria de imagens existentes podem ser feitos com o material fornecido.

## Como a skill trabalha

- **Planejamento.** Analisa as fontes, define o nível de detalhe e traduz cada ideia importante em uma cena ou diagrama. Quando o assunto tem hierarquia, capítulos ou categorias aparecem como regiões visuais contendo seus subitens.
- **Produção.** Gera e reúne blocos ilustrados no ImageGen. Mantém as pranchas proporcionais, os símbolos consistentes e as legendas úteis. Entrega as imagens em JPG por padrão.
- **Auditoria.** Reavalia figuras, setas, textos, hierarquia, proporção, encaixes e fidelidade à fonte. Descreve os achados e deixa as correções para a etapa de edição.

## Exemplos de pedidos

- “Use $imagens-didaticas para planejar uma prancha a partir do manual fictício de uma biblioteca itinerante. Mostre empréstimos e devoluções como blocos dentro do capítulo de atendimento.”
- “Use $imagens-didaticas para gerar as imagens do plano aprovado em blocos separados. Entregue o conjunto quando estiver pronto.”
- “Use $imagens-didaticas para fazer uma auditoria exaustiva desta prancha. Verifique se cada figura e seta ensina o que o texto descreve. Quero somente os achados.”

## Licença

[MIT](LICENSE)
