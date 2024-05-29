# Teste de Sistemas Operativos - Módulo 5

Faz *fork* do repositório para teres a tua cópia.

Preenche o ficheiro README diretamente no GitHub. A partir da página principal do repositório, clica em "Edit File" (ícone representando um lápis).

Escreve as respostas dentro dos blocos correspondentes. Substitui as reticências pelo que é pedido em cada pergunta. Não desformates o documento.

Quando acabares, carrega no botão "Commit Changes".

## Informação do aluno

    Nome: Bohdan

## P1 - Para as seguintes questões, assinala a opção correta: (2.5v)

  1. Que comando é usado para definir permissões de execução num script Bash?

    A) chmod +x script.sh
    B) chmod -x script.sh
    C) chmod +r script.sh
    D) chmod -r script.sh
    
    Resposta: A

  2. Como se define um comentário num script Bash?

    A) // comentário
    B) /* comentário */
    C) # comentário
    D) -- comentário
    
    Resposta: c
   
  3. Que comando é usado para adicionar uma linha de texto ao final de um arquivo em Bash?

    A) echo "texto" > arquivo
    B) echo "texto" < arquivo
    C) echo "texto" | arquivo
    D) echo "texto" >> arquivo
    
    Resposta: D

  4. Qual é o comando usado para ler a entrada do utilizador num script Bash?

    A) read
    B) input
    C) get
    D) scan
    
    Resposta: A

  5. Que símbolo é usado para denotar uma variável em Bash?

    A) %
    B) $
    C) &
    D) #
    
    Resposta: B

## P2 - Escreve scripts em Bash para realizar as seguintes instruções: (7.5v)

  1. Exibir a mensagem "Olá, Mundo!" no terminal.

    Resposta:
    #!/bin/bash
    nano ola_mundo.sh
    
    
  2. Receber dois números como entrada, e exibir a soma dos dois.

    Resposta:
     #!/bin/bash
     echo "4:"
    read num1
    echo "6:"
    read num2
    soma=$((num1 + num2)) 
    echo "A soma de $num1 e $num2 é: $soma"
    

  3. Ler um valor numérico e imprimir uma mensagem a informar se o mesmo é par ou ímpar.

    Resposta:
    #!/bin/bash        
    echo "2:"
    read numero
    if (( numero % 2 == 0 )); then
    echo "O número $numero é par."
    else
    echo "O número $numero é ímpar."
    fi
      

## P3 - Indica o que é realizado pelas seguintes instruções: (6v)

  1. 
    
    echo "scale=2;22/7" | bc

    Resposta:
    código define o número de casas décimais que o número pode ter. O bc é uma calculadora que permite fazer cálculos.
    
     
  2. 
    
    #!/bin/bash
    sum=0S
    for i in {1..5}
    do
      sum=$((sum + i))
    done
    echo "A soma dos números de 1 a 5 é $sum."


    Resposta:
    soma dos numeros de 1 a 5

  3. 
    
    #!/bin/bash
    num=10
    while [ $num -gt 0 ]
    do
      echo "Número: $num"
      ((num--))
    done

    Resposta:
     faz a listagem de número de 10 a 1

## P4 - Realiza os seguintes exercícios, com respostas detalhadas: (4v)

  1. O que é um **shebang** (#!) e qual é a sua função num script?

    Resposta:
    Um shebang é uma sequência de dois caracteres (#!) usada em scripts de shell e a sua função principal é indicar ao sistema operacional qual interpretador de comandos deve ser usado para executar o script. Por exemplo, se um script começa com #!/bin/bash, isso significa que o script deve ser executado pelo interpretador de shell Bash.

  2. Como se utiliza a instrução 'if-else' num script Bash? Escreve um exemplo simples.

    Resposta:
   
    if [ $((numero % 2)) -eq 0 ]; then
    echo "$numero é um número par."
    else
    echo "$numero é um número ímpar."
    fi
    
