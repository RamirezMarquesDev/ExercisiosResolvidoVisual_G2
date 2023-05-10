# Atividade Lógica de Programação
----------------------------------
##### Ramirez Marques
----------------------
##### Parte 2: Condicional Para

**01 - Ler um número inteiro N, daí mostrar na tela a tabuada de N para 1 a 10, conforme exemplo.**

```algoritmo "condicional_para1"
var
   n,i, produto : inteiro
inicio
      escreval ("Digite a tabuada para qual valor? ")
      leia (n)
      para i de 1 ate 10 faca
      produto <- n * i
      escreval (n, " x ",i," = ", produto)
      fimpara
fimalgoritmo
```

**02 - Leia 2 valores inteiros X e Y (em qualquer ordem). A seguir, calcule e mostre a soma dos números impares entre eles.**

```algoritmo "exercicio_para2"
var
   x, y, i, aux, soma: inteiro
inicio
   escreval ("Digite dois Numeros Inteiros: ")
   leia (x)
   leia (y)
   se x > y entao
      aux <- x
      x <- y
      y <- aux
   fimse
   para i de x + 1 ate y - 1 faca
        se (i%2<>0) entao
           soma <- soma + i
        fimse
   fimpara
   escreval("SOMA =", soma)
fimalgoritmo
```

**03 - Leia um valor inteiro X. Em seguida mostre os ímpares de 1 até X, um valor por linha, inclusive o X, se for o caso.**

```algoritmo "exercisio_para3"
var
   x,i: inteiro
inicio
      escreva ("Digite um numero inteiro: ")
      leia (x)
      para i de 1 ate x faca
          se (i%2<>0) entao
            escreval(i)
          fimse
      fimpara
fimalgoritmo
```

**04 - Leia um valor inteiro N. Este valor será a quantidade de valores inteiros X que serão lidos em seguida. Mostre quantos destes valores X estão dentro do intervalo [10,20] e quantos estão fora do intervalo, conforme exemplo:**

```algoritmo "exercisio_para4"
var
  i,n,x,dentro,fora: inteiro
inicio

   dentro <-0
   fora <-0
   escreval("Quantos numeros voce vai digitar?")
   leia (n)
   
   para i de 1 ate n faca
   
      escreval("Digite um Numero: ")
      leia (x)
      se (x >= 10) e (x<=20) entao
         dentro <- dentro+1
         senao
              fora <- fora + 1
      fimse
   fimpara
      escreval(dentro , " Dentro")
      escreva(fora , " Fora")
fimalgoritmo
```

**05 - Leia um valor inteiro N. Este valor será a quantidade de números inteiros que serão lidos em seguida. Para cada valor lido, mostre uma mensagem dizendo se este valor lido é PAR ou IMPAR, e também se é POSITIVO ou NEGATIVO. No caso de o valor ser igual a zero (0), seu programa deverá imprimir apenas NULO.**

```algoritmo "exercisio_para5"
var
  I,n,x: inteiro
inicio
     escreval("Quantos numeros voce vai digitar?")
     leia (n)
     para i de 1 ate n faca
         escreval("Digite um Numero: ")
         leia (x)
         se (x%2<>0)e (x<0) entao
            escreval ("IMPAR NEGATIVO")
           senao
             se (x%2=0)e (x<0)entao
               escreval ("PAR NEGATIVO")
               senao
                 se (x%2<>0)e (x>0)entao
                   escreval ("IMPAR POSITIVO")
                   senao
                     se (x%2=0) e (x>0) entao
                       escreval("PAR POSITIVO")
                     senao
                     escreval ("NULO")
                 fimse
              fimse
            fimse
         fimse
     fimpara
fimalgoritmo
```

**06 - Leia um valor inteiro N, que representa o número de casos de teste que vem a seguir. Cada caso de teste consiste de 3 valores reais, para os quais você deverá calcular e mostrar a média ponderada, sendo que o primeiro valor tem peso 2, o segundo valor tem peso 3 e o terceiro valor tem peso 5. Vale lembrar que a média ponderada é a soma de todos os valores multiplicados pelo seu respectivo peso, dividida pela soma dos pesos.**

```algoritmo "exercisio_para6"
var
   n,i : inteiro
   a,b,c,media:real
inicio
      escreval ("Quantos Casos voce vai digitar: ")
      leia (n)
      para i de 1 ate n faca
           escreval ("Digite os tres numeros: ")
           leia (a)
           leia (b)
           leia (c)
           media <- (2*a + 3*b + 5*c)/10
           escreval ("MEDIA = ", media:3:1)
     fimpara
fimalgoritmo
```

**07 - Escreva um algoritmo que leia dois números e imprima o resultado da divisão
do primeiro pelo segundo. Caso não for possível, mostre a mensagem “DIVISAO
IMPOSSIVEL”.**

```algoritmo "exercisio_para7"
var
   i,n,num, den: inteiro
   di: real
inicio
      escreval ("Quantos Casos voce vai digitar? ")
      leia (n)
      para i de 1 ate n faca
           escreval ("Entre com o Numerador: ")
           leia (num)
           escreval ("Entre com o Denominador: ")
           leia (den)
           se (num = 0) e (den = 0)entao
              escreval ("DIVISÃO IMPOSSÍVEL")
             senao
                  se den = 0 entao
                     escreval ("DIVISÃO IMPOSSÍVEL")
                      senao
                           di <- num / den
                           escreval ("Divisão = ",di)
                  fimse
           fimse
      fimpara
fimalgoritmo
```




