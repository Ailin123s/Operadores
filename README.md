# Operadores
Operadores if y when

package com.example.myapplication

fun main(){
    //verifAge()
    //gradoEscolar()
    //GradoEscolar()
    //Triangulo()
    tipoDeDato()
}
fun verifAge(){
    print ("Ingrese edad y precione enter(escribe solo el numero):")
    val age = readLine()?.toInt()

    if(age==18){
        println("Ya eres mayor de edad¡")
    }
    if(age!! >18){
        println("Ya eres mayor de edad")
    }
    else if (age!! == 18){
        println("Acabas de cumplir la mayoria de edad")

    }
    else{
        println("Eres menor de edad")
    }

}
fun gradoEscolar(){
    print("Ingrese edad y presiona enter(Escribe solo el numero):")
    val age = readLine()?.toInt()
    when(age){
        0->println("Apenas eres recien nacido")
        1->println("Solo tienes un año de edad")
    }
}
fun GradoEscolar() {
    println("Ingresa tu edad:")
    val age=readLine()?.toInt()
    when (age) {
        0 -> println("Apenas eres recien nacido")
        1 -> println("Tienes un año de edad")
        in 2..5 -> println("Estas en prescolar")
        in 6..12 -> println("Estas en primaria")
        in 13..16 -> println("Estas en secundaria")
        in 17..20 -> println("Estas en preparatoria")
        in 21..25 -> println("Estas en universidad")
    }

}

fun Triangulo() {

    println("Ingresa el valor del lado 1\n")
    val lado1 = readLine()?.toInt()
    println("Ingresa el valor del lado 2\n")
    val lado2 = readLine()?.toInt()
    println("Ingresa el valor del lado 3\n")
    val lado3 = readLine()?.toInt()

    if (lado1 == lado2 && lado2 == lado3) {
        println("El triangulo es equilatero")
    } else if (lado1 == lado2 && lado2 != lado3 || lado3 == lado1 && lado2 != lado1) {
        println("El triangulo es isoceles")
    } else {
        println("El triangulo es escaleno")
    }
}

fun tipoDeDato(dato: Any){

    when(dato){
        is String -> println("Es una String")
        is Int -> println("Es un Entero")
        is Double -> println("Es un Double")
        else -> println("Tipo de dato no soportado")

    }
}
