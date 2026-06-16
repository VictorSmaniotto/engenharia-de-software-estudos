---
title: "Aula 15 - Recursividade"
source: "https://ead.unimar.br/aulas/algoritmo-logica-programacao/aula-15.html"
author:
published:
created: 2026-06-15
description:
tags:
---
Disciplina: Algoritmos e Lógica de Programação
Aula 15 - Recursividade

## Sub-Rotinas: Recursividade

O uso de sub-rotinas é bastante interessante, e permite que algoritmos sejam estruturados de forma distinta, permitindo melhor compreensão da lógica e maior possibilidade de reuso de código.

As sub-rotinas são utilizadas geralmente para processamentos mais específicos e que possam ser realizados com certa independência do restante do algoritmo, além de serem uma forma importante de implementação de algoritmos, pois uma sub-rotina representa um trecho de algoritmos que pode ser chamada a qualquer instante durante a execução do mesmo, sem que haja necessidade de duplicação deste trecho do algoritmo, reduzindo a quantidade de linhas e de tempo necessário para implementação.

Um recurso um tanto complexo e que será trabalhado nesta aula com alguns exemplos é a execução de sub-rotinas de forma recursiva em que uma sub-rotina em execução pode, se necessária, chamar a si mesma para que sucessivas iterações da execução da sub-rotina sejam possíveis, assim como ocorre em laços de repetição.

Um detalhe bastante pertinente é que nessa comparação feita, pode-se imaginar laços de repetição sendo implementados como sub-rotinas recursivas, em que as execuções das iterações por chamadas à sub-rotina por ela mesma podem ser programadas para ocorrerem como nas condições dos laços de repetição.

Muitas vezes, as sub-rotinas recursivas são utilizadas para a realização de cálculos matemáticos, mas podem ser também utilizadas para outras finalidades diversas sem envolver necessariamente cálculos.

O que reduz muito o uso da recursão é a forma como é elaborada a lógica e o raciocínio em soluções baseadas nesta técnica, pois a forma como se estruturam sub-rotinas recursivas é mais complexo que outras estruturas do desenvolvimento de algoritmos em geral, mas isto é algo que com a prática, se torna mais fácil e pode ser incorporada como uma prática comum no desenvolvimento de algoritmos.

Após a apresentação do conceito de recursividade, é importante que se exercitem exemplos de código, modifique-se cada um para que se obtenham novas alternativas de funções recursivas, e assim, possa ser compreendido este conceito.

Acesse o link:[Disponível aqui](https://www.embarcados.com.br/recursividade/)

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-conecte-se-center.svg)

A elaboração de algoritmos que utilizem o recurso é bastante comum, pois, em geral, não é todo o algoritmo que é recursivo, mas apenas uma ou mais sub-rotinas contidas no algoritmo para realização de algum processamento repetitivo que possa ser realizado utilizando recursão.

Existem alguns exemplos bastante comuns de aplicação da recursão, mas em geral, não são implementados desta forma devido ao maior grau de complexidade lógica necessário para sua elaboração, mas para efeito de estudos, podem ser exemplos bastante interessantes. Observe o exemplo de função da imagem 44.

FUNÇÃO POTENCIA (INTEIRO BASE, INTEIRO EXPOENTE) DE INTEIRO

SE (EXPOENTE = 0) ENTÃO

RETORNE 1;

SENÃO

RETORNE (BASE \* POTENCIA (BASE, EXPOENTE-1));

FIMSE;

FIM;

Imagem 44: Exemplo de função recursiva.| Fonte: O autor.

Neste exemplo da figura 44, é possível observar que a escrita de uma função recursiva em sua sintaxe é semelhante a qualquer outra função, mas existe um detalhe que indica a existência de uma possível recursão logo num primeiro olhar, quando se percebe que a função, em determinado momento, chama a si mesma.

Analisando com mais detalhes, a funcionalidade da sub-rotina se baseia em calcular, a partir de dois valores recebidos como parâmetros, a operação exponencial matemática, e o resultado seja devolvido ao ponto do algoritmo que chama esta sub-rotina.

Para que o cálculo possa ser realizado, existe uma estrutura de repetição encarregada de finalizar a função ou chamá-la novamente para que uma nova iteração ocorra desta sub-rotina, e a recursão seja realizada.

A lógica da recursão neste exemplo se baseia na forma como o cálculo é realizado para que se possa pensar em como realizar as sucessivas operações até que uma condição indique que não são mais necessárias chamadas da função, e o processo de repetição termine, mas não ocorre apenas o término das iterações, mas todos os retornos das novas chamadas da função.

Ao receber os dados por meio dos parâmetros, é realizada uma verificação em uma estrutura condicional para retornar o valor 1 como resposta no caso de o expoente ser igual a zero, operação definida como padrão pela matemática o resultado 1 para qualquer número elevado a zero.

Caso não seja 1 o valor do expoente, a função chama a si mesma novamente solicitando a multiplicação do valor a base pelo retorno da função, repetindo o mesmo valor para a base, mas reduzindo uma unidade no expoente para que a cada iteração, cada nova chamada da função, o processo se repita.

Com isto, se fossem passados os valores 5 para base, e 3 para expoente, a execução da função ocorreria de forma que 3 seria comparado a zero, e sendo diferentes, a condição alternativa para falso inicia a multiplicação do valor da base pelo resultado da chamada da própria função pela recursividade.

Numa segunda iteração da função, o expoente valeria 2, sendo diferente de zero ainda, e engatilhando nova multiplicação da base na expressão já iniciada na iteração anterior, e passando para a nova ocorrência da chamada da função com base igual, e expoente menos 1.

Na próxima iteração (terceira), tem-se agora o expoente 1, que ainda permanece diferente de zero, e por isto, nova multiplicação é organizada, tendo agora três operações “5 \* ” encadeadas.

Novamente a função é chamada com a mesma base, mas agora, com mais uma redução do expoente, seu valor segue como zero para a nova iteração, e nela, como o expoente tem seu valor igual ao da comparação, realmente ocorre o retorno de um valor 1 para ser utilizado na expressão, e ao fim de uma quarta iteração, a expressão se encontra semelhante a “5 \* 5 \* 5 \* 1”.

Realizando o cálculo normalmente, obtém-se um resultados 125 pelas três multiplicações com 5 e uma inicial pelo valor 1, e assim, com os sucessivos retornos, este resultado é obtido e a função encerra seu processamento.

Esse exemplo traz uma demonstração de como se pode aplicar recursividade em algoritmos, mas este mesmo exemplo pode ser escrito em forma de algoritmo imperativo sem a modularização em forma de função ou sem o uso da recursividade. Observe o exemplo da imagem 59.

FUNÇÃO POTENCIA (INTEIRO BASE, INTEIRO EXPOENTE) DE INTEIRO

DECLARE

INTEIRO: I, RESULTADO;

RESULTADO <- 1;

PARA I DE 1 ATÉ EXPOENTE PASSO 1 FAÇA

RESULTADO <- RESULTADO \* BASE;

FIMPARA;

FIM;

Imagem 44: Exemplo de função recursiva.| Fonte: O autor.

Nesta versão alternativa da imagem 44, a funcionalidade se mantém inalterada, mas a forma como se desenvolve o processamento é totalmente diferente, pois, ao invés de ser utilizado o recurso da função chamar a si mesma pela recursividade, apenas uma estrutura de repetição se encarrega da obtenção do mesmo resultado.

A lógica elaborada para essa versão da solução é mais simples de ser pensada e de implementar inicialmente, mas é preciso observar que alguns detalhes não podem ser ignorados como a necessidade de duas variáveis adicionais locais à função, a correta inicialização da variável “RESULTADO” e a correta elaboração do laço de repetição.

Esse processo de elaboração de estruturas de repetição necessita de prática para que se torne simples seu uso, assim como o uso da técnica de recursividade que necessita de prática para que se esteja familiarizado com a sua lógica.

O chamado aninhamento ou encadeamento de estruturas de controle é um recurso muito útil e acrescenta muitos recursos no desenvolvimento de algoritmos, mas também traz um aumento na complexidade de algoritmos que pode confundir iniciantes.

É importante praticar o desenvolvimento de pequenos algoritmos contendo estruturas de controle variadas para compreender a mecânica dos aninhamentos e como uma estrutura possui influência sobre a outra, além de compreender melhor os motivos de ser necessário aninhar estruturas e como definir quais tipos são adequados a cada situação.

![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/cx-gabaritar-center.svg)

A ideia de que funções utilizando recursividade possuem características semelhantes às de estruturas de repetição mostram que a recursividade pode ser uma ferramenta muito eficiente para a realização de ações repetitivas.

O mais importante é observar diferentes exemplos, avaliar sua lógica, e a partir do amadurecimento da compreensão do mecanismo da recursividade, construir algoritmos cada vez mais completos, eficientes e com maior complexidade para a solução de problemas também mais complexos.

FUNÇÃO TABUADA (INTEIRO VALOR1, INTEIRO VALOR2) DE INTEIRO

DECLARE

SE (VALOR1 = 0) ENTÃO

RETORNE 1;

SENÃO

ESCREVA (VALOR2, “ X “, VALOR1, “ = “, VALOR1 \* VALOR2);

RETORNE (TABUADA (VALOR1-1, VALOR2));

FIMSE;

FIM;

Imagem 45: Exemplo de função recursiva. | Fonte: autor.

Neste outro exemplo trazido na imagem 45, é elaborado um algoritmo para exibir a tabuada de um determinado valor. Como artifícios para o funcionamento da tabuada são utilizados dois parâmetros para a função, mas ambos são utilizados para o mesmo valor referente a qual tabuada deve ser exibida.

O detalhe é que são utilizados esses dois parâmetros para que um possa ser utilizado nas iterações da recursão, e o outro para manter intacto o valor original da tabuada a ser exibida. Isto é feito, pois a cada nova chamada da função recursiva, um dos parâmetros é decrementado em uma unidade para controle das iterações, e o outro permanece o mesmo.

Outro ponto relevante é que a cada iteração da recursão não é apenas realizado um cálculo no momento da chamada da função, mas uma instrução para exibição de conteúdo ao usuário com texto, dados e mais o resultado do cálculo de cada iteração tem o propósito de construir a tabuada sequencialmente.

Importante realçar que a construção da tabuada é realizada sequencialmente, mas em ordem inversa à redução do valor da variável “VALOR1” a cada nova chamada da função, pois o processamento é realizado apenas após a condição de parada ser atendida e as sucessivas recursões irem retornando e realizando a instrução baseada no comando “ESCREVA”.

  <video controls=""><source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.mp4"> <source src="https://ead.unimar.br/aulas/algoritmo-logica-programacao/videos/bg-video_1-transcode.webm"> </video>![](https://ead.unimar.br/aulas/algoritmo-logica-programacao/images/videoaula.svg)

### Nesta aula estudamos:

- Sub-Rotinas: Recursividade

Para complementar seus estudos, assista à videoaula a seguir: