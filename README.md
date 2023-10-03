# Operadores
Operadores if y when

package com.example.myapplication

fun main(){
    //verifAge()
    //gradoEscolar()
    //GradoEscolar()
    
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


