# Produção

Abra esta referência quando o usuário autorizar a geração, a correção ou a exportação.

## Prepare a série e os blocos

1. Trabalhe com a versão vigente, as decisões aprovadas e o mapa de cobertura de [Planejamento](planejamento.md). Confira o que cada bloco precisa ensinar e consulte a skill **imagegen** para produzi-lo.
2. Divida a prancha em blocos por unidade didática. Em material denso, produza cada bloco separadamente com ImageGen. Um bloco deve conter a cena, seus rótulos e as explicações imediatas. Gere também no ImageGen as faixas, os títulos ou as conexões entre blocos que fizerem parte da arte final.
3. Planeje o espaço real antes de consolidar. Para pranchas que precisam ser equilibradas, um ponto de partida é uma tela quase quadrada ou levemente horizontal, como 4:3. Ajuste em função da composição. Expanda as dimensões ao acomodar uma tabela maior, uma região de vários cartões ou um fluxo longo. Preserve a escala legível do conteúdo. Use espaços entre grupos para mostrar separação, evitando intervalos sem função.
4. Dê ao gerador a cena, a relação espacial, o sentido das setas e o texto exato da parte. Indique o papel das imagens de referência. Em revisões, descreva as invariantes, incluindo identidade, direção do olhar, posição, escala, símbolos aprovados e relações que já funcionam, conforme o caso.
5. Apresente na legenda os símbolos que reaparecem e use-os nas cenas. Repita a forma e a cor do símbolo sempre que ele tiver o mesmo significado. Diferencie estados com sinais que funcionem mesmo sem cor, como uma mudança de forma ou um rótulo curto.

## Monte e revise

- Use ImageGen para gerar e editar ilustrações, textos da prancha, diagramas, símbolos e setas. Reserve código, SVG ou outro método para produzir essa arte mediante pedido explícito do usuário.
- Para reunir blocos prontos, use a ferramenta raster disponível, inclusive via código. A montagem pode posicionar blocos inteiros, recortar margens, alinhar regiões e ajustar o tamanho proporcionalmente para acomodar os encaixes. O fundo da tela, as margens e os espaçamentos podem ser definidos na própria montagem. Sharp, Pillow e ImageMagick são exemplos intercambiáveis.
- Em pranchas densas, prefira montagem raster em uma tela maior. Use os blocos aprovados na resolução em que foram gerados e preserve os pixels originais sempre que couberem. Faça os ajustes de composição sem redesenhar textos ou elementos didáticos. Caso use o ImageGen para reunir os blocos, confira se a saída conserva as dimensões e a legibilidade do material de origem.
- Corrija o menor bloco que permite resolver o problema por completo. Regere e confira a região maior se a falha estiver na hierarquia, na leitura do fluxo ou numa duplicação. Preserve os demais blocos e os símbolos definidos. Se o erro voltar após uma regeneração, mude a estrutura da cena ou o encaixe que o causa e verifique o resultado esperado.
- Compare a arte gerada com o mapa de cobertura. Confira se cada bloco ensina a regra planejada, se as conexões continuam fiéis à fonte e se os encaixes funcionam na prancha completa. Inspecione texto, símbolos, setas e alinhamento antes de trocar a versão ativa.

## Resolução e formato

- Para novas pranchas, use por padrão a resolução em pixels da tela de destino como piso. A largura final deve alcançar pelo menos a largura da tela, e a altura final deve alcançar pelo menos a altura da tela. Use preferencialmente as dimensões do monitor indicado pelo usuário ou do monitor principal quando houver acesso ao dispositivo. Dimensões explícitas no pedido têm precedência.
- Consulte a resolução física em pixels quando possível. Quando ela estiver indisponível, use um piso estimado compatível com o caso, como 3840 × 2160 para uma tela horizontal, e registre a referência adotada. Preserve a proporção escolhida para a prancha ao atingir o piso. A densidade do conteúdo pode exigir uma tela bem maior.
- Verifique a nitidez separadamente das dimensões. Ganhe legibilidade gerando blocos maiores ou subdividindo regiões densas. Uma ampliação proporcional pode ajudar a alcançar o tamanho do arquivo, mas a resolução efetiva do conteúdo continua limitada pelos blocos de origem.

## Exporte e confirme a entrega

- Por padrão, entregue o JPG final a partir do PNG mestre. Reserve o PNG para revisão e reexportação. Use um conversor de formato pronto para exportar a imagem concluída, preservando a composição. Se o usuário indicar um fator de escala, aplique-o ao mestre preservando a proporção. Respeite pedidos explícitos de outro formato ou de adiar a exportação.
- Preserve o trabalho de referência e os blocos necessários para continuar. Produza uma cópia para as revisões quando a substituição do original não tiver sido pedida. Evite cópias intermediárias grandes sem função. Uma limpeza pedida pelo usuário deve respeitar o escopo indicado e as necessidades da revisão ativa.
- Confira as dimensões finais nas duas direções. Abra o JPG entregue na resolução nativa e examine os blocos mais densos e os encaixes para detectar perda de nitidez, recortes ou deformações introduzidas na montagem.
- Entregue os arquivos finais do conjunto juntos quando esse for o combinado. Dê links aos arquivos finais e indique as decisões relevantes de composição e exportação.

## Compatibilidade com Firefox

1. **JPG.** Exporte em **JPEG sequencial (baseline)**. No conversor, selecione **Baseline** ou **Standard** e desative a opção **Progressivo** (*Progressive*). Use sRGB com 8 bits por canal e alta qualidade. Quando a inspeção do cabeçalho estiver disponível, confirme o marcador **SOF0**.
2. **PNG.** Exporte como **PNG estático sem entrelaçamento**. Desative a opção **Entrelaçado** (*Interlace*) para que o campo **Interlace method** no cabeçalho **IHDR** seja **0**. Use sRGB com 8 bits por canal e mantenha o canal alfa se a imagem precisar de transparência.
3. **Conferência.** Verifique o formato, as dimensões, a codificação e a legibilidade no arquivo entregue. O teste de abertura no navegador é uma verificação adicional quando solicitado.

Referências de formato. [JPEG T.81, tabela B.1](https://www.w3.org/Graphics/JPEG/itu-t81.pdf#page=36) e [PNG, cabeçalho IHDR](https://www.w3.org/TR/png-3/#11IHDR).
