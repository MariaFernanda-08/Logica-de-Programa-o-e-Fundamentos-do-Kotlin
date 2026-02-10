# Lógica de Programação e Fundamentos do Kotlin
Atividade 2

## Exercício 1 - Diferença de Dois Números ➖
```Kotlin
fun main() {  
    print("Insira um número:")
    val n1 = readln().toInt()
    print("Insira outro número:")
    val n2 = readln().toInt()
    
    val diferenca = n1 - n2
    print("A diferença entre os dois números escolhidos é $diferenca")
}   
```
---
## Exercício 2 - Nome Completo ✏️
```Kotlin
fun main() {  
    print("Digite seu nome:")
    val nome = readln().toString()
    print("Digite seu sobrenome:")
    val sobrenome = readln().toString()
    
    print("Nome Completo: $nome $sobrenome")
}   
```
---
## Exercício 3 - Quatro Operações ✖️
```Kotlin
fun main(){
    print("Digite um número:")
    val n1 = readln().toInt()
    print("Digite outro número:")
    val n2 = readln().toInt()
    
    val soma = n1 + n2
    val subtracao = n1 - n2
    val multiplicacao = n1 * n2
    val divisao = n1/n2
    
    println("Adição: $n1 + $n2 = $soma")
    println("Subtração: $n1 - $n2 = $subtracao")
    println("Multiplicação: $n1 * $n2 = $multiplicacao")
    print("Divisão: $n1/$n2 = $divisao")
}
```
---
## Exercício 4 - Área do Quadrado 🟥
```Kotlin
fun main() {  
    print("Insira o comprimento do quadrado:")
    val comprimento = readln().toInt()
    val area = comprimento * comprimento
    
    print("A área do quadrado é $area cm²")
}  
```
---
## Exercício 5 -  Área do Triângulo 📐
```Kotlin
fun main() {  
    print("Insira a altura do triângulo:")
    val altura = readln().toInt()
    print("Insira a base do triângulo:")
    val base = readln().toInt()
    val area = (base * altura)/2
    
    print("A área do triângulo é $area cm²")
} 
```
---
## Exercício 6 - IMC ⚖️
```Kotlin
fun main() {
    print("Digite seu peso(kg):")
    val peso = readln().toFloat()
    
    print("Digite sua altura(m):")
    val altura = readln().toFloat()
    
    val imc = peso/(altura * altura)
    
    if (imc <= 18.5){
        print("Abaixo do peso - IMC: $imc kg/m²")
    } else if (imc > 18.5 && imc <= 24.9){
        print("Peso normal - IMC: $imc kg/m²")
    } else if(imc >= 25 && imc <= 29.9 ){
        print("Sobrepeso - IMC: $imc kg/m²")
    } else{
        print("Obesidade - IMC: $imc kg/m²")
    }  
}   
```
---
## Exercício 7 - Idade 📅
```Kotlin
fun main() {
    println("Digite a idade em dias:")
    val totalDias = readln()!!.toInt()

    val anos = totalDias/365
    val restoAnos = totalDias % 365

    val meses = restoAnos/30
    val dias = restoAnos % 30
    println("$anos anos, $meses meses e $dias dias")
}
```
---
## Exercício 8 - Média Final 🧾
```Kotlin
fun main() {
    println("Coloque aqui sua primeira nota")
    var nota1 = readLine()!!.toDouble()
    
    println("Coloque aqui sua segunda nota")
    var nota2 = readLine()!!.toDouble()
    
    println("Coloque aqui sua terceira nota")
    var nota3 = readLine()!!.toDouble()
    
    var media = (nota1 + nota2 + nota3) / 3 
    println("Media: $media")
}
```
---
## Exercício 9 - Duração do Evento 🎉
```Kotlin
fun main() {
    println("Digite o tempo do evento em segundos:")
    val totalSegundos = readLine()!!.toInt()

    val horas = totalSegundos / 3600
    val restoHoras = totalSegundos % 3600

    val minutos = restoHoras / 60
    val segundos = restoHoras % 60

    println("$horas horas, $minutos minutos e $segundos segundos")
}
```
---
## Exercício 10 - Distância 🏎️
```Kotlin
import kotlin.math.sqrt
import kotlin.math.pow

fun main() {
    println("Digite o valor de x1")
    val x1 = readLine()!!.toDouble()
    
    println("Digite o valor para y1")
    val y1 = readLine()!!.toDouble()
    
    println("Digite o valor para x2")
    val x2 = readLine()!!.toDouble()
    
    println("Digite o valor para y2")
    val y2 = readLine()!!.toDouble()
    
    val distancia = sqrt((x2 - x1).pow(2) + (y2 - y1).pow(2))
    println("A distância entre os pontos é $distancia")
}
```
---
## Exercício 11 - Valor Inteiro 🔢
```Kotlin
import kotlin.math.pow

fun main() {
    println("Digite o valor de A (inteiro e positivo):")
    val A = readLine()!!.toInt()
    
    println("Digite o valor de B (inteiro e positivo):")
    val B = readLine()!!.toInt()
    
    println("Digite o valor de C (inteiro e positivo):")
    val C = readLine()!!.toInt()
    
    val R = (A + B).toDouble().pow(2)
    val S = (B + C).toDouble().pow(2)
    
    val D = (R + S) / 2
    
    println("O valor de D é $D")
}
```
---
## Exercício 12 - Custo ao Consumidor 🏭
```Kotlin
fun main() {
    print("Digite o custo de fábrica do carro: ")
    val custoFabrica = readLine()!!.toDouble()

    val percentualDistribuidor = 0.28
    val percentualImpostos = 0.45

    val custoConsumidor = custoFabrica * (1 + percentualDistribuidor + percentualImpostos)
    println("O custo ao consumidor é: R$ %.2f".format(custoConsumidor))
}
```
---
## Exercício 13 - Equações Lineares ➗
```Kotlin
fun main() {
    print("Digite o valor de a: ")
    val a = readLine()!!.toDouble()
    print("Digite o valor de b: ")
    val b = readLine()!!.toDouble()
    print("Digite o valor de c: ")
    val c = readLine()!!.toDouble()
    print("Digite o valor de d: ")
    val d = readLine()!!.toDouble()
    print("Digite o valor de e: ")
    val e = readLine()!!.toDouble()
    print("Digite o valor de f: ")
    val f = readLine()!!.toDouble()

    val denominador = a * e - b * d

    if (denominador == 0.0) {
        println("O sistema não tem solução única.")
    } else {
        val x = (c * e - b * f) / denominador
        val y = (a * f - c * d) / denominador

        println("Valor de x = $x")
        println("Valor de y = $y")
    }
}
```
---
## Exercício 14 - Salário Atual 💰
```Kotlin
fun main() {
    println("informe seu salario atual")
    var salarioAtual = readLine()!!.toDouble()
    
    var salarioNovo = salarioAtual * 1.25
    
    println("novo salario: $salarioNovo")
}
```
---
## Exercício 15 - Novo salário 💵
```Kotlin
fun main() {
    println("Informe o salário atual do funcionário:")
    val salarioAtual = readLine()!!.toDouble()

    println("Informe o percentual de aumento (%):")
    val percentualAumento = readLine()!!.toDouble()

    val salarioNovo = salarioAtual * (1 + percentualAumento / 100)

    println("Novo salário: $salarioNovo")
}
```
---
## Exercício 16 - Idade 📅
```Kotlin
fun main() {
    println("Digite seu ano de nascimento:")
    val anoNascimento = readLine()!!.toInt()

    println("Digite o ano atual:")
    val anoAtual = readLine()!!.toInt()

    val idadeAnos = anoAtual - anoNascimento
    val idadeMeses = idadeAnos * 12
    val idadeSemanas = idadeAnos * 52
    val idadeDias = idadeAnos * 365 

    println("Idade da pessoa em anos: $idadeAnos")
    println("Idade da pessoa em meses: $idadeMeses")
    println("Idade da pessoa em semanas: $idadeSemanas")
    println("Idade da pessoa em dias (aproximado): $idadeDias")
}
```
---
## Exercício 17 - Ração 🐈‍⬛
```Kotlin 
fun main() {
    println("Digite o peso do saco de ração (em kg):")
    val pesoSacoKg = readLine()!!.toDouble()

    println("Digite a quantidade de ração diária para cada gato (em gramas):")
    val racaoPorGato = readLine()!!.toDouble()

    val numeroGatos = 2
    val dias = 5

    val pesoSacoGramas = pesoSacoKg * 1000

    val consumoTotal = racaoPorGato * numeroGatos * dias

    val restante = pesoSacoGramas - consumoTotal

    println("Ração restante após $dias dias: $restante gramas")
}
```
---
## Exercício 18 - Troca 🔂
```Kotlin 
fun main() {
    println("Digite o valor da variavel A")
    var variavelA = readLine()!!.toDouble()
    
    println("Digite o valor da variavel B")
    var variavelB = readLine()!!.toDouble()
    
    println("Antes da troca: a = $variavelA, b = $variavelB")
     
    val temp = variavelA
    variavelA = variavelB
    variavelB = temp
    
    println("Depois da troca: a = $variavelA, b = $variavelB")
}
```
---
## Exercício 19 - Volume 📐
```Kotlin 
fun main() {
    println("Digite o valor do comprimento")
    var comprimento = readLine()!!.toDouble()
    
    println("Digite o valor da altura")
    var altura = readLine()!!.toDouble()
    
    println("Digite o valor da largura")
    var largura = readLine()!!.toDouble()
    
    var volume = comprimento * altura * largura
    println("volume: $volume")
    
}
```
---
## Exercício 20 - Quadrado da Diferença ➖
```Kotlin 
fun main() {
    print("Digite o valor de A: ")
    val a = readLine()!!.toInt()

    print("Digite o valor de B: ")
    val b = readLine()!!.toInt()

    val resultado = (a - b) * (a - b)

    println("O quadrado da diferença de A em relação a B é: $resultado")
}
```
---
## Exercício 21 - Conversão 💵
```Kotlin 
fun main() {
    var valor_dolar = 50
    val cotaçao_dolar = 5.60
    var converçao_real = valor_dolar * cotaçao_dolar

    println(converçao_real)
}
```
---
## Exercício 22 - Soma do Quadrado 🟥
```Kotlin 
fun main() {
    println("Insira o primeiro valor inteiro")
    var valorA = readLine()!!.toDouble()
    
    println("Insira o segundo valor inteiro")
    var valorB = readLine()!!.toDouble()
    
    println("Insira o terceiro valor")
    var valorC = readLine()!!.toDouble()
    
    var soma = valorA + valorB + valorC
    var resultado = soma * soma
    
    println("A soma quadrada é: $resultado")
}
```
---
## Exercício 23 - Quatro Operações 🔢
```Kotlin 
fun main() {
    println("Insira o primeiro valor real")
    var valorReal1 = readLine()!!.toDouble()
    
    println("insira o segundo valor real")
    var valorReal2 = readLine()!!.toDouble()
    
    var soma = valorReal2 + valorReal1
    var subtracao = valorReal1 - valorReal2
    var multiplicacao = valorReal1 * valorReal2
    var divisao = if (valorReal2 != 0.0) valorReal1 / valorReal2 else "Divisão por zero não é permitida"
    
    println("Soma: $soma")
    println("Subtração: $subtracao")
    println("Multiplicação: $multiplicacao")
    println("Divisão: $divisao")
}
```
---
## Exercício 24 - Raio da Esfera 🔴
```Kotlin 
fun main() {
    println("Digite o valor do raio da esfera:")
    val raio = readLine()!!.toDouble()

    val pi = 3.14159
    val volume = (4.0 / 3.0) * pi * (raio * raio * raio)

    println("O volume da esfera é: $volume")
}
```
---
## Exercício 25 - Antecessor e Sucessor ⬅️➡️
```Kotlin 
fun main() {
    
    println("Insira um valor numerico inteiro")
    var valor = readLine()!!.toDouble()
    
    var antecessor = valor - 1
    var sucessor = valor + 1
    
    println("Antecessor: $antecessor")
    println("Sucessor: $sucessor")
}
```
