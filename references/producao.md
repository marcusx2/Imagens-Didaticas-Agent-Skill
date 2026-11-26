# Produção

Abra esta referência quando o usuário autorizar a geração, a correção ou a exportação.

## Prepare a série e os blocos

1. Fixe o plano aprovado, o conjunto de símbolos, as artes de referência e a versão ativa. Use o formato de entrega pedido e adote JPG quando esse detalhe estiver em aberto. Consulte a skill **imagegen** para a produção visual.
2. Divida a prancha em blocos por unidade didática. Em material denso, produza cada bloco separadamente com ImageGen. Um bloco deve conter a cena, seus rótulos e as explicações imediatas. Reúna os blocos no ImageGen dentro da hierarquia planejada, com o mesmo padrão de margens, títulos e alinhamento.
3. Planeje o espaço real antes de consolidar. Para pranchas que precisam ser equilibradas, um ponto de partida é uma tela quase quadrada ou levemente horizontal, como 4:3. Ajuste em função da composição. Expanda as dimensões ao acomodar uma tabela maior, uma região de vários cartões ou um fluxo longo. Preserve a escala legível do conteúdo. Use espaços entre grupos para mostrar separação, evitando intervalos sem função.
4. Dê ao gerador a cena, a relação espacial, o sentido das setas e o texto exato da parte. Indique o papel das imagens de referência. Em revisões, descreva as invariantes, incluindo identidade, direção do olhar, posição, escala, símbolos aprovados e relações que já funcionam, conforme o caso.
5. Apresente na legenda os símbolos que reaparecem e use-os nas cenas. Repita a forma e a cor do símbolo sempre que ele tiver o mesmo significado. Diferencie estados com sinais que funcionem mesmo sem cor, como uma mudança de forma ou um rótulo curto.

## Monte e revise

- Use exclusivamente ImageGen por padrão para gerar, editar e montar a arte, incluindo textos, diagramas, símbolos e ilustrações. Na montagem, forneça os blocos como referência, indique sua posição e reinspecione o resultado por inteiro.
- Considere parte da produção visual qualquer etapa que determine o que aparece na prancha. Colar blocos gerados em uma tela, sobrepor títulos e rótulos, desenhar setas ou molduras e inserir ícones são exemplos. Faça todas essas etapas no ImageGen por padrão, inclusive quando a arte de origem já tiver sido gerada nele.
- Use código, SVG ou outro método de produção visual somente quando o usuário pedir expressamente esse método. Se houver uma falha persistente com ImageGen, informe o ponto que ficou pendente.
- Corrija o menor bloco que permite resolver o problema por completo. Regere e confira a região maior se a falha estiver na hierarquia, na leitura do fluxo ou numa duplicação. Preserve os demais blocos e os símbolos definidos. Se o erro voltar após uma regeneração, mude a estrutura da cena ou o encaixe que o causa e verifique o resultado esperado.
- Inspecione o recorte afetado e seus encaixes. Confira texto, símbolos, figuras, setas e alinhamento antes de trocar a versão ativa. Depois, confira a composição inteira na tela. Verifique as características pedidas na arte efetivamente gerada.

## Exporte e confirme a entrega

- Por padrão, entregue o JPG final a partir do PNG mestre. Reserve o PNG para revisão e reexportação. Use um conversor de formato pronto para exportar a imagem concluída, preservando a composição. Se o usuário indicar um fator de escala, aplique-o ao mestre preservando a proporção. Respeite pedidos explícitos de outro formato ou de adiar a exportação.
- Preserve o trabalho de referência e os blocos necessários para continuar. Produza uma cópia para as revisões quando a substituição do original não tiver sido pedida. Evite cópias intermediárias grandes sem função. Uma limpeza pedida pelo usuário deve respeitar o escopo indicado e as necessidades da revisão ativa.
- Entregue os arquivos finais do conjunto juntos quando esse for o combinado. Dê links aos arquivos finais e indique as decisões relevantes de composição e exportação.

## Compatibilidade com Firefox

1. **JPG.** Exporte em **JPEG sequencial (baseline)**. No conversor, selecione **Baseline** ou **Standard** e desative a opção **Progressivo** (*Progressive*). Use sRGB com 8 bits por canal e alta qualidade. Quando a inspeção do cabeçalho estiver disponível, confirme o marcador **SOF0**.
2. **PNG.** Exporte como **PNG estático sem entrelaçamento**. Desative a opção **Entrelaçado** (*Interlace*) para que o campo **Interlace method** no cabeçalho **IHDR** seja **0**. Use sRGB com 8 bits por canal e mantenha o canal alfa se a imagem precisar de transparência.
3. **Conferência.** Verifique o formato, as dimensões, a codificação e a legibilidade no arquivo entregue. O teste de abertura no navegador é uma verificação adicional quando solicitado.

Referências de formato. [JPEG T.81, tabela B.1](https://www.w3.org/Graphics/JPEG/itu-t81.pdf#page=36) e [PNG, cabeçalho IHDR](https://www.w3.org/TR/png-3/#11IHDR).
