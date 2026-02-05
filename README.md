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
