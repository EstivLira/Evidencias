# Evidencias
Área de un circulo

Área de un circulo

import kotlin.math.PI

fun main() { // Define el radio del círculo val radio = 5.0

// Calcula el área del círculo
val area = PI * radio * radio

// Imprime el resultado
println("El área del círculo con radio $radio es: $area")
}


import kotlin.math.PI

fun main() { // Define el radio del círculo val radio = 5.0

// Calcula el área del círculo
val area = PI * radio * radio

// Imprime el resultado
println("El área del círculo con radio $radio es: $area")
}
const val PI = 3.1416f
const val PHI = 1.618f

fun main(){
    val radius= 4f
    val area= circleArea(radius)
    //println( "El area es: $area")
    //println(getPi())
    //printPhi()
    val userValidated = login("Juanito", "Navaja")
    //println("Usuario Logeado? $userValidated")
   // println("Area con valores por defecto ${rectangleArea()}")
    //println("Area con valores por defecto ${Areaprismarec()}")
   // imprimir("Remmplazo del primer valor")
    //imprimir("Remplazo del primer valor", "Remplazo del segundo valor")
}

fun circleArea(radius:Float): Float{
    return PI*radius.pow(2)
}

fun getPi(): Float{
    return PI
}
fun printPhi(){
    println("El numero aureo vale $PHI")
}
// Funcion local: Funcion que vive dentro de otra funcion
//El aclance de esa funcion solo es para la funcion que la contiene
//Se declara como una funcion normal
//Mantiene limpio el codigo
//Agrega reusabilidad al codigo

fun login(user:String, password:String): Boolean{
    fun validate(input: String):Boolean{
        if(input.isEmpty()){
            return false
        }
        return true
    }
    val userValidated = validate(user)
    val passValidated = validate(password)

    return userValidated && passValidated
}
fun rectangleArea(base:Double=20.0, height: Double= 30.0): Double{
    return base*height
}

fun Areaprismarec(base1:Double=20.0,height1:Double=30.0, profun:Double=40.0 ): Double{
    return base1*height1*profun
}

fun imprimir(
    valor:String= "Este es el primer valor por defecto",
    valor2:String= "Este es el segundo valor por defecto"){
    println(valor)
    println(valor2)
}

fun promedio(cal1: Float= 8f, cal2: Float=8f, cal3:Float):Float{
    return (cal1+cal2+cal3)/3f
}
