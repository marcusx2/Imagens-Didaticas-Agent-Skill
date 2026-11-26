# Imagens Didáticas

<img src="assets/icon-small.png" width="64" height="64" alt="Ícone do ImageGen com uma pilha de três livros">

Skill para planejar, produzir, revisar e auditar imagens didáticas no Codex. Use um material de referência, uma norma, um edital ou uma imagem existente para definir o que cada prancha precisa ensinar e como representar seus conceitos.

## Instalação no Codex

1. Extraia o ZIP e coloque a pasta **imagens-didaticas** em **~/.codex/skills/**. O arquivo [SKILL.md](SKILL.md) fica diretamente dentro da pasta da skill.
2. No Codex, mencione **$imagens-didaticas** na sua solicitação.

O ImageGen integrado ao Codex cria as ilustrações, os diagramas e os textos da prancha. Os blocos podem ser reunidos em uma tela maior para manter os detalhes legíveis ao ampliar. O planejamento e a auditoria de imagens existentes podem ser feitos com o material fornecido.

## Como a skill trabalha

- **Planejamento.** Identifica o que o aluno precisa conseguir explicar, organiza os tópicos por importância e transforma conceitos e relações em cenas ou diagramas.
- **Produção.** Gera blocos ilustrados e os reúne em uma prancha proporcional, com símbolos consistentes e legendas úteis. Usa como referência mínima o tamanho da tela em pixels e entrega em JPG por padrão.
- **Auditoria.** Reavalia figuras, setas, textos, hierarquia, proporção, encaixes e fidelidade à fonte. Descreve os achados e deixa as correções para a etapa de edição.

## Exemplos de pedidos

- “Use $imagens-didaticas para planejar uma prancha a partir do manual fictício de uma biblioteca itinerante. Mostre empréstimos e devoluções como blocos dentro do capítulo de atendimento.”
- “Use $imagens-didaticas para gerar as imagens do plano aprovado em blocos separados. Entregue o conjunto quando estiver pronto.”
- “Use $imagens-didaticas para fazer uma auditoria exaustiva desta prancha. Verifique se cada figura e seta ensina o que o texto descreve. Quero somente os achados.”

## Licença

[MIT](LICENSE)
