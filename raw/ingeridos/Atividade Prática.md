Disciplina: Algoritmos e Lógica de Programação

Digamos que seja necessária a elaboração de um algoritmo para o desenvolvimento de um simples jogo do tipo quiz de perguntas e respostas com pontuação e avaliação de desempenho baseado nos critérios a seguir.   

* JOGO COM 5 PERGUNTAS SOBRE A DISCIPLINA CADA ACERTO VALE 10 OU 5 PONTOS.

  

10 PONTOS NA PRIMEIRA TENTATIVA

5 PONTOS NA SEGUNDA TENTATIVA

0 PONTOS SE ERRAR AS DUAS TENTATIVAS. 

  

* AO FINAL, EXIBIR A PONTUAÇÃO TOTAL . 

* EXIBIR MENSAGEM JUNTO A PONTUAÇÃO . 

  

"EXCELENTE" SE ATINGIR 50 PONTOS. 

"ÓTIMO" SE FIZER ENTRE 37 E 49 PONTOS. 

"BOM" SE FIZER ENTRE 25 E 36 PONTOS. 

"RUIM" SE FIZER MENOS DE 25 PONTOS. 

  

Elaborar um algoritmo capaz de permitir jogar este quiz de perguntas e respostas. 

É interessante observar que é possível utilizar uma versão testável na ferramenta Visual G, por exemplo, em função da maior complexidade do algoritmo. 

O mais importante na atividade é a lógica correta, avaliação de respostas e cálculo da pontuação, mas a aparência e uso de elementos especiais para melhoria da jogabilidade são desnecessários em termos de pontuação na atividade. 

Encaminhe apenas o TXT com o seu código.

Resposta abaixo:

```c
algoritmo "Quiz de Lógica"

var
  resposta, opcaoCorreta: caractere
  contador, tentativas, pontos, questoes: inteiro
  opcoes: vetor[1..4] de caractere

inicio

  escreval("Bem vindo(a) ao Quiz sobre Algoritmos e Lógica de Programação!!!")
  escreval("----------------------------------------------------------------")
  escreval("Responda as 5 perguntas a seguir para validarmos seu conhecimento.")
  escreval("Regras do jogo: Você terá duas tentativas de acerto para cada questão, se acertar de primeira ganha 10 pontos, na segunda 5 pontos e se errar duas vezes é 0 pontos!")
  escreval("Boa sorte!")
  escreval("----------------------------------------------------------------")
  escreval(" Questões — Algoritmos e Lógica de Programação\n")


  opcoes[1] <- "a"
  opcoes[2] <- "b"
  opcoes[3] <- "c"
  opcoes[4] <- "d"

  questoes <-1
  pontos <-0


  enquanto questoes <= 5  faca

    se questoes = 1 entao
      escreval("Questão ", questoes)
      escreval("Em algoritmos, os operadores são classificados em três grupos: matemáticos, relacionais e lógicos. Cada grupo tem comportamento e finalidade distintos. Considerando o operador % e sua aplicação em pseudocódigo, assinale a alternativa correta:")
      escreval("a) O operador % realiza a divisão entre dois números reais e retorna o quociente com casas decimais.")
      escreval("b) O operador % é classificado como operador relacional e retorna verdadeiro quando dois valores são proporcionais.")
      escreval("c) O operador % retorna o resto inteiro de uma divisão, sendo utilizado exclusivamente com números inteiros.")
      escreval("d) O operador % substitui o símbolo ÷ nos algoritmos por limitação do teclado, tendo o mesmo comportamento da divisão comum.")

      opcaoCorreta <- opcoes[3]
      tentativas <- 1
    fimse

    se questoes = 2 entao
      escreval("Questão ", questoes)
      escreval("A precedência de operadores define a ordem em que as operações são avaliadas em uma expressão. Considere a expressão abaixo e assinale o valor correto que será atribuído à variável RESULTADO:")
      escreval("a) 12, pois as somas são realizadas antes das multiplicações.")
      escreval("b) 0, pois os parênteses mais externos anulam o resultado interno.")
      escreval("9, pois a soma 5 + 3 é calculada primeiro por estar à esquerda.")
      escreval("d) 6, pois (1+4)=5 é avaliado primeiro, depois 3*2=6, depois 6-5=1, e por fim 5+1=6.")
      opcaoCorreta <- opcoes[4]
      tentativas <- 1
    fimse

    se questoes = 3 entao
      escreval("Questão ", questoes)
      escreval("As estruturas de repetição permitem que blocos de instruções sejam executados múltiplas vezes. Uma diferença fundamental entre ENQUANTO...FAÇA e REPITA...ATÉ diz respeito ao momento em que a condição de controle é verificada. Sobre essa diferença, assinale a alternativa correta:")
      escreval("a) Ambas as estruturas verificam a condição no início, mas REPITA exige que a condição seja verdadeira para iniciar, enquanto ENQUANTO exige que seja falsa.")
      escreval("b) ENQUANTO verifica a condição antes da primeira iteração, podendo não executar nenhuma vez; REPITA verifica ao final, garantindo ao menos uma execução.")
      escreval("c) REPITA verifica a condição no início e para quando ela é falsa; ENQUANTO verifica ao final e continua enquanto ela é verdadeira.")
      escreval("d) As duas estruturas são equivalentes em comportamento; a diferença está apenas na sintaxe da palavra reservada utilizada.")
      opcaoCorreta <- opcoes[2]
      tentativas <- 1
    fimse

    se questoes = 4 entao
      escreval("Questão ", questoes)
      escreval("A estrutura ESCOLHA...CASO é uma alternativa à estrutura SE aninhado para tratamento de múltiplas opções. Porém, ela possui uma limitação importante em relação ao SE. Assinale a alternativa que descreve corretamente essa limitação:")
      escreval("a) ESCOLHA...CASO não permite a cláusula CASO CONTRÁRIO, obrigando o programador a tratar todos os valores possíveis explicitamente.")
      escreval("b) ESCOLHA...CASO só pode ser utilizada dentro de estruturas de repetição, não podendo aparecer no fluxo principal do algoritmo.")
      escreval("c) ESCOLHA...CASO aceita expressões lógicas compostas com operadores E e OU, mas não aceita operadores relacionais como > e <.")
      escreval("d) ESCOLHA...CASO só suporta comparação de igualdade com valores discretos de uma única variável, não aceitando expressões lógicas ou relacionais compostas.")
      opcaoCorreta <- opcoes[4]
      tentativas <- 1
    fimse

    se questoes = 5 entao
      escreval("Questão ", questoes)
      escreval("Um algoritmo em pseudocódigo utiliza o seguinte trecho para coletar e exibir dados:")
      escreval("ESCREVA ('INFORME SUA IDADE: ');")
      escreval("LEIA (IDADE);")
      escreval("ESCREVA ('Você tem ', IDADE, ' anos.);")
      escreval("Sobre o comportamento desse trecho e as regras de uso das instruções LEIA e ESCREVA, assinale a alternativa correta:")
      escreval("a) O comando ESCREVA não pode receber uma variável e um texto na mesma instrução; seria necessário usar dois comandos separados.")
      escreval("b) O comando LEIA exibe automaticamente uma mensagem de solicitação ao usuário antes de aguardar a digitação, dispensando o primeiro ESCREVA.")
      escreval("c) O valor exibido pelo segundo ESCREVA será sempre o valor padrão do tipo da variável, pois LEIA não altera o conteúdo de IDADE antes da exibição.")
      escreval("d) Os parâmetros do ESCREVA separados por vírgula são concatenados na exibição; o valor digitado pelo usuário em LEIA é armazenado em IDADE e exibido no segundo ESCREVA.")
      opcaoCorreta <- opcoes[4]
      tentativas <- 1
    fimse


    repita
      escreva("Digite a letra da sua resposta: ")
      leia(resposta)
      resposta <- Minusc(resposta)
      escreval(resposta)

      se (tentativas = 1) e (resposta = opcaoCorreta) entao
        pontos <- pontos + 10
        escreval("Parabens! Conseguiu ", pontos, " pontos")
        tentativas <-3

      senao se (tentativas = 2) e (resposta = opcaoCorreta) entao
        pontos <- pontos + 5
        escreval("Parabens! Conseguiu ", pontos, " pontos")
        tentativas <-3

      senao se (resposta <> opcaoCorreta) e ((resposta = opcoes[1]) ou (resposta = opcoes[2]) ou (resposta = opcoes[3]) ou (resposta = opcoes[4])) entao
        escreval("Você errou! Tente novamente")
        tentativas <- tentativas + 1

      senao escreval("Resposta inválida! Digite a, b, c ou d.")

      fimse fimse fimse
    ate tentativas = 3
    questoes <- questoes + 1
    escreval("----------------------------------------------------------")



  fimenquanto

  escreval("Seu resultado:")

  se pontos = 50 entao
    escreval("EXCELENTE")
  senao se pontos >= 37 entao
    escreval("ÓTIMO")
  senao se pontos >= 25 entao
    escreval("BOM")
  senao
    escreval("RUIM")
  fimse fimse fimse


fimalgoritmo

```