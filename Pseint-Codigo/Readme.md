## Ejercicio 1

Algoritmo TieneTresDigitos
    
    Definir numero Como Entero

   
    Escribir "Ingresa un número: "
    Leer numero

    // Verificar si el número tiene tres dígitos
    Si numero >= 100 Y numero <= 999 O numero <= -100 Y numero >= -999 Entonces
        Escribir "El número tiene tres dígitos."
    Sino
        Escribir "El número no tiene tres dígitos."
    FinSi
    
FinAlgoritmo

## Ejercicio 2

Algoritmo EsNegativo
    
    Definir numero Como Entero

    
    Escribir "Ingresa un número entero: "
    Leer numero

    // Verificar si el número es negativo
    Si numero < 0 Entonces
        Escribir "El número es negativo."
    Sino
        Escribir "El número no es negativo."
    FinSi

FinAlgoritmo

## Ejercicio 3

Algoritmo TerminaEnCuatro
    
    Definir numero Como Entero

   
    Escribir "Ingresa un número: "
    Leer numero

    // Verificar si el número termina en 4
    Si numero MOD 10 = 4 Entonces
        Escribir "El número termina en 4."
    Sino
        Escribir "El número no termina en 4."
    FinSi
FinAlgoritmo

## Ejercicio 4

Algoritmo OrdenarNumeros
    
    Definir num1, num2, num3 Como Entero

   
    Escribir "Ingresa el primer número: "
    Leer num1
    Escribir "Ingresa el segundo número: "
    Leer num2
    Escribir "Ingresa el tercer número: "
    Leer num3

    // Verificar el orden de los números y mostrarlos de menor a mayor
    Si num1 <= num2 Y num1 <= num3 Entonces
        Si num2 <= num3 Entonces
            Escribir "El orden es: ", num1, ", ", num2, ", ", num3
        Sino
            Escribir "El orden es: ", num1, ", ", num3, ", ", num2
        FinSi
    Sino
        Si num2 <= num1 Y num2 <= num3 Entonces
            Si num1 <= num3 Entonces
                Escribir "El orden es: ", num2, ", ", num1, ", ", num3
            Sino
                Escribir "El orden es: ", num2, ", ", num3, ", ", num1
            FinSi
        Sino
            Si num1 <= num2 Entonces
                Escribir "El orden es: ", num3, ", ", num1, ", ", num2
            Sino
                Escribir "El orden es: ", num3, ", ", num2, ", ", num1
            FinSi
        FinSi
    FinSi

FinAlgoritmo

## Ejercicio 5

Algoritmo DescuentoZapatos
   
    Definir cantidadZapatos, precioUnitario, totalCompra, descuento, totalFinal Como Real

   
    precioUnitario <- 80

   
    Escribir "Ingresa la cantidad de zapatos que vas a comprar: "
    Leer cantidadZapatos

    
    totalCompra <- cantidadZapatos * precioUnitario

    // Verificar el tipo de descuento según la cantidad de zapatos
    Si cantidadZapatos > 30 Entonces
        descuento <- totalCompra * 0.40  // Descuento del 40%
    Sino
        Si cantidadZapatos > 20 Entonces
            descuento <- totalCompra * 0.20  // Descuento del 20%
        Sino
            Si cantidadZapatos > 10 Entonces
                descuento <- totalCompra * 0.10  // Descuento del 10%
            Sino
                descuento <- 0  // No hay descuento
            FinSi
        FinSi
    FinSi

    // Calcular el total final después de aplicar el descuento
    totalFinal <- totalCompra - descuento

    
    Escribir "El descuento aplicado es: $", descuento
    Escribir "El total final a pagar es: $", totalFinal

FinAlgoritmo

## Ejercicio 6

Algoritmo SueldoSemanal
    
    Definir horasTrabajadas, sueldoBase, sueldoFinal, horasExtras Como Real

    la semana: "
    Leer horasTrabajadas

    // Si el trabajador trabaja 40 horas o menos
    Si horasTrabajadas <= 40 Entonces
        sueldoBase <- horasTrabajadas * 20  // Pago por hora normal
        sueldoFinal <- sueldoBase
    Sino
        // Si el trabajador trabaja más de 40 horas
        horasExtras <- horasTrabajadas - 40  // Calcular las horas extras
        sueldoBase <- 40 * 20  // Pago por las primeras 40 horas
        sueldoExtra <- horasExtras * 25  // Pago por las horas extras
        sueldoFinal <- sueldoBase + sueldoExtra  // Sueldo total
    FinSi

    // Mostrar el sueldo final
    Escribir "El sueldo final del trabajador es: $", sueldoFinal

FinAlgoritmo

## Ejercicio 7

Algoritmo DescuentoTiendaHelado
    
    Definir tipoMembresia Como Caracter
    Definir montoCompra, descuento, montoFinal Como Real
	
    
    Escribir "Ingresa el tipo de membresía (A, B o C): "
    Leer tipoMembresia
	
    
    Escribir "Ingresa el monto de la compra: "
    Leer montoCompra
	
    // Calcular el descuento según el tipo de membresía
    Si tipoMembresia = "A" Entonces
        descuento <- montoCompra * 0.10  // Descuento del 10%
    Sino
        Si tipoMembresia = "B" Entonces
            descuento <- montoCompra * 0.15  // Descuento del 15%
        Sino
            Si tipoMembresia = "C" Entonces
                descuento <- montoCompra * 0.20  // Descuento del 20%
            Sino
                Escribir "Tipo de membresía no válido."
			
		FinSi
	FinSi
FinSi

// Calcular el monto final después del descuento
montoFinal <- montoCompra - descuento

// Mostrar el monto de descuento y el monto final
Escribir "El descuento aplicado es: $", descuento
Escribir "El monto final a pagar es: $", montoFinal
FinAlgoritmo
## Ejercicio 8

Algoritmo PromedioNotas
   
    Definir nota1, nota2, nota3, promedio Como Real

    
    Escribir "Ingresa la primera nota: "
    Leer nota1
    Escribir "Ingresa la segunda nota: "
    Leer nota2
    Escribir "Ingresa la tercera nota: "
    Leer nota3

    // Calcular el promedio de las tres notas
    promedio <- (nota1 + nota2 + nota3) / 3

    // Mostrar el promedio
    Escribir "El promedio de las tres notas es: ", promedio

    // Determinar si el estudiante aprobó o no
    Si promedio >= 6 Entonces
        Escribir "El estudiante aprobó."
    Sino
        Escribir "El estudiante no aprobó."
    FinSi

FinAlgoritmo

## Ejercicio 9

Algoritmo AumentoDeSalario
    
    Definir salario, aumento Como Real

    
    Escribir "Ingresa el salario del trabajador: "
    Leer salario

    // Verificar el salario y calcular el aumento
    Si salario > 2000 Entonces
        aumento <- salario * 0.05  // Aumento del 5%
    Sino
        aumento <- salario * 0.10  // Aumento del 10%
    FinSi

    // Calcular el salario con el aumento
    salario <- salario + aumento

    // Mostrar el aumento y el nuevo salario
    Escribir "El aumento es: $", aumento
    Escribir "El nuevo salario es: $", salario
FinAlgoritmo

## Ejercicio 10

Algoritmo ParOImpar
    // Declarar la variable para el número ingresado
    Definir numero Como Entero

    // Solicitar al usuario que ingrese un número
    Escribir "Ingresa un número: "
    Leer numero

    // Verificar si el número es par o impar
    Si numero % 2 = 0 Entonces
        Escribir "El número ", numero, " es par."
    Sino
        Escribir "El número ", numero, " es impar."
    FinSi
FinAlgoritmo


## Ejercicio 11

Algoritmo MayorDeTresNumeros
    
    Definir numero1, numero2, numero3 Como Entero

    
    Escribir "Ingresa el primer número: "
    Leer numero1
    Escribir "Ingresa el segundo número: "
    Leer numero2
    Escribir "Ingresa el tercer número: "
    Leer numero3

    // Comparar los tres números
    Si numero1 > numero2 Y numero1 > numero3 Entonces
        Escribir "El número ", numero1, " es el mayor."
    Sino
        Si numero2 > numero1 Y numero2 > numero3 Entonces
            Escribir "El número ", numero2, " es el mayor."
        Sino
            Escribir "El número ", numero3, " es el mayor."
        FinSi
    FinSi
FinAlgoritmo

## Ejercicio 12

Algoritmo MayorDeDosNumeros
    
    Definir numero1, numero2 Como Entero

    
    Escribir "Ingresa el primer número: "
    Leer numero1
    Escribir "Ingresa el segundo número: "
    Leer numero2

    // Comparar los dos números
    Si numero1 > numero2 Entonces
        Escribir "El número ", numero1, " es el mayor."
    Sino
        Si numero2 > numero1 Entonces
            Escribir "El número ", numero2, " es el mayor."
        Sino
            Escribir "Los dos números son iguales."
        FinSi
    FinSi
FinAlgoritmo

## Ejercicio 13

Algoritmo EsVocal
    
    Definir letra Como Caracter
	
    
    Escribir "Ingresa una letra: "
    Leer letra
	
    // Convertir la letra a minúscula manualmente
    Si letra = "A" Entonces
        letra <- "a"
    Sino
        Si letra = "E" Entonces
            letra <- "e"
        Sino
            Si letra = "I" Entonces
                letra <- "i"
            Sino
                Si letra = "O" Entonces
                    letra <- "o"
                Sino
                    Si letra = "U" Entonces
                        letra <- "u"
                    FinSi
                FinSi
            FinSi
        FinSi
    FinSi
	
    // Verificar si la letra es una vocal
    Si letra = "a" O letra = "e" O letra = "i" O letra = "o" O letra = "u" Entonces
        Escribir "La letra ", letra, " es una vocal."
    Sino
        Escribir "La letra ", letra, " no es una vocal."
    FinSi
FinAlgoritmo


## Ejercicio 14

Algoritmo NumeroPrimo
    // Declarar la variable
    Definir numero, i Como Entero
    Definir esPrimo Como Logico
	
    // Solicitar al usuario que ingrese un número entre 1 y 10
    Escribir "Ingresa un número entero entre 1 y 10: "
    Leer numero
	
    // Inicializar la variable esPrimo como verdadero (suponemos que es primo)
    esPrimo <- Verdadero
	
    // Verificar si el número es menor que 2, en cuyo caso no es primo
    Si numero < 2 Entonces
        esPrimo <- Falso
    Sino
        // Comprobar si el número tiene algún divisor aparte de 1 y él mismo
        Para i <- 2 Hasta numero - 1 Con Paso 1
            Si numero Mod i = 0 Entonces
                esPrimo <- Falso
            FinSi
        FinPara
    FinSi
	
    // Mostrar el resultado
    Si esPrimo Entonces
        Escribir "El número ", numero, " es un número primo."
    Sino
        Escribir "El número ", numero, " no es un número primo."
    FinSi
FinAlgoritmo

## Ejercicio 15

Algoritmo ConvertirUnidades
    
    Definir centimetros, pulgadas, libras, kilogramos Como Real

    Escribir "Ingresa la longitud en centímetros: "
    Leer centimetros

    // Convertir centímetros a pulgadas
    pulgadas <- centimetros * 0.393701

    // Solicitar al usuario ingresar el peso en libras
    Escribir "Ingresa el peso en libras: "
    Leer libras

    // Convertir libras a kilogramos
    kilogramos <- libras * 0.453592

    // Mostrar los resultados de las conversiones
    Escribir "La longitud en pulgadas es: ", pulgadas
    Escribir "El peso en kilogramos es: ", kilogramos
FinAlgoritmo

## Ejercicio 16

Algoritmo DiaDeLaSemana
    
    Definir numero Como Entero

    
    Escribir "Ingresa un número entre 1 y 7 para conocer el día de la semana: "
    Leer numero

   
    Segun numero Hacer
        Caso 1:
            Escribir "El día correspondiente es: Lunes"
        Caso 2:
            Escribir "El día correspondiente es: Martes"
        Caso 3:
            Escribir "El día correspondiente es: Miércoles"
        Caso 4:
            Escribir "El día correspondiente es: Jueves"
        Caso 5:
            Escribir "El día correspondiente es: Viernes"
        Caso 6:
            Escribir "El día correspondiente es: Sábado"
        Caso 7:
            Escribir "El día correspondiente es: Domingo"
        De Otro Modo:
            Escribir "Número inválido. Por favor ingresa un número entre 1 y 7."
    FinSegun

FinAlgoritmo

## Ejercicio 17

Algoritmo HoraSiguiente
   
    Definir hora, minuto, segundo, nuevaHora, nuevoMinuto, nuevoSegundo Como Entero

    
    Escribir "Ingresa la hora actual (formato 24 horas): "
    Leer hora
    Escribir "Ingresa los minutos actuales: "
    Leer minuto
    Escribir "Ingresa los segundos actuales: "
    Leer segundo

    // Sumar un segundo a la hora
    nuevoSegundo <- segundo + 1

    // Verificar si los segundos superan los 59, si es así, reseteamos los segundos y aumentamos el minuto
    Si nuevoSegundo >= 60 Entonces
        nuevoSegundo <- 0
        nuevoMinuto <- minuto + 1
    Sino
        nuevoMinuto <- minuto
    FinSi

    // Verificar si los minutos superan los 59, si es así, reseteamos los minutos y aumentamos la hora
    Si nuevoMinuto >= 60 Entonces
        nuevoMinuto <- 0
        nuevaHora <- hora + 1
    Sino
        nuevaHora <- hora
    FinSi

    // Verificar si la hora supera las 23 (es decir, pasa al siguiente día)
    Si nuevaHora >= 24 Entonces
        nuevaHora <- 0
    FinSi

    // Mostrar la nueva hora
    Escribir "La hora dentro de un segundo será: ", nuevaHora, ":", nuevoMinuto, ":", nuevoSegundo

FinAlgoritmo

## Ejercicio 18

Algoritmo VentaCDs
   
    Definir cantidadCDs, precioUnitario, precioTotal, ganancia Como Real

    
    Escribir "Ingresa la cantidad de CDs a vender: "
    Leer cantidadCDs

  
    Si cantidadCDs >= 1 Y cantidadCDs <= 9 Entonces
        precioUnitario <- 10
    Sino
        Si cantidadCDs >= 10 Y cantidadCDs <= 99 Entonces
            precioUnitario <- 8
        Sino
            Si cantidadCDs >= 100 Y cantidadCDs <= 499 Entonces
                precioUnitario <- 7
            Sino
                Si cantidadCDs >= 500 Entonces
                    precioUnitario <- 6
                FinSi
            FinSi
        FinSi
    FinSi

    // Calcular el precio total para el cliente
    precioTotal <- precioUnitario * cantidadCDs

    // Calcular la ganancia para el vendedor (8,25% del precio total)
    ganancia <- precioTotal * 0.0825

    // Mostrar el precio total y la ganancia del vendedor
    Escribir "El precio total a pagar por el cliente es: $", precioTotal
    Escribir "La ganancia para el vendedor es: $", ganancia
FinAlgoritmo

## Ejercicio 19

Algoritmo CalculoPagoEmpleado
   
    Definir idEmpleado, diasTrabajados, salarioDiario, pagoTotal Como Entero
    
   
    Escribir "Ingresa el número identificador del empleado (1-4): "
    Leer idEmpleado
    
    Escribir "Ingresa la cantidad de días trabajados (máximo 6): "
    Leer diasTrabajados
    
   
    Si diasTrabajados < 1 O diasTrabajados > 6 Entonces
        Escribir "El número de días debe estar entre 1 y 6."
    Sino
        // Asignar el salario diario según el identificador del empleado
        Segun idEmpleado Hacer
            Caso 1:
                salarioDiario <- 56  // Cajero
            Caso 2:
                salarioDiario <- 64  // Servidor
            Caso 3:
                salarioDiario <- 80  // Preparador de mezclas
            Caso 4:
                salarioDiario <- 48  // Mantenimiento
            De Otro Modo:
                Escribir "Identificador de empleado no válido."
                
        FinSegun
        
        // Calcular el pago total
        pagoTotal <- salarioDiario * diasTrabajados
        
        // Mostrar el pago total que debe recibir el empleado
        Escribir "El pago total del empleado con identificador ", idEmpleado, " es: $", pagoTotal
    Fin Si
FinAlgoritmo


## Ejercicio 20

Algoritmo OperacionesConCuatroNumeros
   
    Definir num1, num2, num3, num4, mayor, suma Como Entero
    Definir cantidadPares Como Entero
    Definir media, cuadradoSegundo Como Real
    
   
    Escribir "Ingresa el primer número: "
    Leer num1
    Escribir "Ingresa el segundo número: "
    Leer num2
    Escribir "Ingresa el tercer número: "
    Leer num3
    Escribir "Ingresa el cuarto número: "
    Leer num4
    
   
    cantidadPares <- 0
    mayor <- num1  // Suponemos que el primer número es el mayor inicialmente
    suma <- num1 + num2 + num3 + num4
    
    // Verificar cuántos números son pares
    Si num1 MOD 2 = 0 Entonces
        cantidadPares <- cantidadPares + 1
    Fin Si
    Si num2 MOD 2 = 0 Entonces
        cantidadPares <- cantidadPares + 1
    Fin Si
    Si num3 MOD 2 = 0 Entonces
        cantidadPares <- cantidadPares + 1
    Fin Si
    Si num4 MOD 2 = 0 Entonces
        cantidadPares <- cantidadPares + 1
    Fin Si
    
    // Encontrar el mayor de los 4 números
    Si num2 > mayor Entonces
        mayor <- num2
    Fin Si
    Si num3 > mayor Entonces
        mayor <- num3
    Fin Si
    Si num4 > mayor Entonces
        mayor <- num4
    Fin Si
    
    
    Si num3 MOD 2 = 0 Entonces
        cuadradoSegundo <- num2 * num2
        Escribir "El cuadrado del segundo número es: ", cuadradoSegundo
    Fin Si
    
   
    Si num1 < num4 Entonces
        media <- suma / 4
        Escribir "La media de los 4 números es: ", media
    Fin Si
    
   
    Si num2 > num3 Entonces
        Si num3 >= 50 Y num3 <= 700 Entonces
            Escribir "La suma de los 4 números es: ", suma
        Fin Si
    Fin Si
    
   
    Escribir "Cantidad de números pares: ", cantidadPares
    Escribir "El mayor número es: ", mayor
FinAlgoritmo

## Ejercicio 21

Algoritmo CalcularFactorial
   
    Definir numero, factorial, i Como Entero
    
    
    Escribir "Ingresa un número entero no negativo:"
    Leer numero
    
    
    Si numero < 0 Entonces
        Escribir "El número debe ser no negativo."
    SiNo
        // Inicializar el factorial
        factorial <- 1
        
        // Calcular el factorial usando un ciclo
        Para i <- 1 Hasta numero Hacer
            factorial <- factorial * i
        Fin Para
        
        // Mostrar el resultado
        Escribir "El factorial de", numero, "es :", factorial
    Fin Si
FinAlgoritmo

## Ejercicio 22 

Algoritmo SumaPrimerosNumeros
    
    Definir n, suma, i Como Entero
    
    
    Escribir "Ingresa un número entero positivo (n):"
    Leer n
    
    
    Si n <= 0 Entonces
        Escribir "El número debe ser mayor que 0."
    SiNo
        // Inicializar la suma
        suma <- 0
        
        // Calcular la suma de los primeros n números
        Para i <- 1 Hasta n Hacer
            suma <- suma + i
        Fin Para
        
        
        Escribir "La suma de los primeros", n, "números es:", suma
    Fin Si
FinAlgoritmo

## Ejercicio 23

Algoritmo SumaImparesMenoresIguales
    
    Definir n, suma, i Como Entero
    
    
    Escribir "Ingresa un número entero positivo (n):"
    Leer n
    
    
    Si n <= 0 Entonces
        Escribir "El número debe ser mayor que 0."
    SiNo
        // Inicializar la suma
        suma <- 0
        
        
        Para i <- 1 Hasta n Con Paso 2 Hacer
            suma <- suma + i
        Fin Para
        
        
        Escribir "La suma de los números impares menores o iguales a", n, "es:", suma
    Fin Si
FinAlgoritmo

## Ejercicio 24

Algoritmo SumaParesHasta1000
    
    Definir suma, i Como Entero
    
    
    suma <- 0
    
    // Calcular la suma de los números pares desde 1 hasta 1000
    Para i <- 2 Hasta 1000 Con Paso 2 Hacer
        suma <- suma + i
    Fin Para
    
    
    Escribir "La suma de todos los números pares hasta 1000 es:", suma

FinAlgoritmo

## Ejercicio 25

Algoritmo FactorialConMientras
    
    Definir numero, factorial, i Como Entero
    
    
    Escribir "Ingresa un número entero no negativo:"
    Leer numero
    
   
    Si numero < 0 Entonces
        Escribir "El número debe ser no negativo."
    SiNo
        // Inicializar el factorial
        factorial <- 1
        i <- 1
        
        // Calcular el factorial usando un ciclo Mientras
        Mientras i <= numero Hacer
            factorial <- factorial * i
            i <- i + 1
        Fin Mientras
        
        
        Escribir "El factorial de", numero, "es:", factorial
    Fin Si
FinAlgoritmo

## Ejercicio 26

Algoritmo CocienteYRestoPorRestas
    
    Definir dividendo, divisor, cociente, resto Como Entero
    
   
    Escribir "Ingresa el dividendo (número mayor):"
    Leer dividendo
    Escribir "Ingresa el divisor (número mayor que 0):"
    Leer divisor
    
    
    Si divisor <= 0 Entonces
        Escribir "El divisor debe ser mayor que 0."
    SiNo
        // Inicializar cociente y resto
        cociente <- 0
        resto <- dividendo
        
        // Calcular cociente y resto mediante restas sucesivas
        Mientras resto >= divisor Hacer
            resto <- resto - divisor
            cociente <- cociente + 1
        Fin Mientras
        
        
        Escribir "El cociente es:", cociente
        Escribir "El resto es:", resto
    Fin Si
FinAlgoritmo


## Ejercicio 27

Algoritmo MediaListaIndefinida
   
    Definir numero, suma, contador Como Real
    
    
    suma <- 0
    contador <- 0
    
   
    Escribir "Ingresa números positivos para calcular la media."
    Escribir "Para terminar, ingresa un número negativo."
    
    Repetir
        Escribir "Ingresa un número:"
        Leer numero
        
        Si numero >= 0 Entonces
            suma <- suma + numero
            contador <- contador + 1
        Fin Si
    Hasta Que numero < 0
    
    // Verificar si se ingresaron números válidos
    Si contador > 0 Entonces
        Escribir "La media de los números ingresados es:", suma / contador
    SiNo
        Escribir "No se ingresaron números positivos."
    Fin Si

FinAlgoritmo

## Ejercicio 28

Algoritmo SumaPrimerosCienRepetir
   
    Definir suma, i Como Entero
    
   
    suma <- 0
    i <- 1
    
    // Ciclo para calcular la suma de los primeros 100 números
    Repetir
        suma <- suma + i
        i <- i + 1
    Hasta Que i > 100
    
   
    Escribir "La suma de los primeros 100 números es:", suma
FinAlgoritmo


## Ejercicio 29

Algoritmo SumaPrimerosCienMientras
    
    Definir suma, i Como Entero
    
    
    suma <- 0
    i <- 1
    
    // Ciclo para calcular la suma de los primeros 100 números
    Mientras i <= 100 Hacer
        suma <- suma + i
        i <- i + 1
    Fin Mientras
    
   
    Escribir "La suma de los primeros 100 números es:", suma
FinAlgoritmo

## Ejercicio 30

Algoritmo SumaPrimerosCienPara
    
    Definir suma, i Como Entero
    
    
    suma <- 0
    
    // Ciclo para calcular la suma de los primeros 100 números
    Para i <- 1 Hasta 100 Hacer
        suma <- suma + i
    Fin Para
    
    
    Escribir "La suma de los primeros 100 números es:", suma

FinAlgoritmo

## Ejercicio 31

Algoritmo MediaParesEImpares
   
    Definir numero, sumaPares, sumaImpares, contadorPares, contadorImpares Como Entero
    
   
    sumaPares <- 0
    sumaImpares <- 0
    contadorPares <- 0
    contadorImpares <- 0
    
    // Ciclo para ingresar 10 números
    Para i <- 1 Hasta 10 Hacer
        Escribir "Ingresa el número", i, ":"
        Leer numero
        
        // Verificar si el número es par o impar
        Si numero MOD 2 = 0 Entonces
            sumaPares <- sumaPares + numero
            contadorPares <- contadorPares + 1
        SiNo
            sumaImpares <- sumaImpares + numero
            contadorImpares <- contadorImpares + 1
        Fin Si
    Fin Para
    
    // Calcular las medias
    Si contadorPares > 0 Entonces
        mediaPares <- sumaPares / contadorPares
        Escribir "La media de los números pares es:", mediaPares
    SiNo
        Escribir "No se ingresaron números pares."
    Fin Si
    
    Si contadorImpares > 0 Entonces
        mediaImpares <- sumaImpares / contadorImpares
        Escribir "La media de los números impares es:", mediaImpares
    SiNo
        Escribir "No se ingresaron números impares."
    Fin Si

FinAlgoritmo

## Ejercicio 32

Algoritmo CiudadConMayorPoblacion
   
    Definir provincias, ciudades, ciudadMayorPoblacion Como Cadena
    Definir poblacion, maxPoblacion Como Entero
    Definir i, j Como Entero
    
    
    maxPoblacion <- 0
    ciudadMayorPoblacion <- ""
    
    // Ciclo para ingresar los datos de las provincias y ciudades
    Para i <- 1 Hasta 3 Hacer  // 3 provincias
        Escribir "Ingrese el nombre de la provincia ", i, ":"
        Leer provincias
        
        Para j <- 1 Hasta 11 Hacer  // 11 ciudades por provincia
            Escribir "Ingrese el nombre de la ciudad ", j, " en la provincia ", provincias, ":"
            Leer ciudades
            
            Escribir "Ingrese la población de la ciudad ", ciudades, ":"
            Leer poblacion
            
            // Comparar si esta ciudad tiene la población más alta
            Si poblacion > maxPoblacion Entonces
                maxPoblacion <- poblacion
                ciudadMayorPoblacion <- ciudades
            Fin Si
        Fin Para
    Fin Para
    
    
    Escribir "La ciudad con la mayor población es:", ciudadMayorPoblacion, " con una población de ", maxPoblacion
FinAlgoritmo

## Ejercicio 33

Algoritmo ContinuarPrograma
  
    Definir continuar Como Cadena

    
    Escribir "Bienvenido al programa."

    Repetir
        
        Escribir "El programa está en ejecución. Realizando tareas..."
        
        
        Escribir "¿Deseas continuar con el programa? (si/no):"
        Leer continuar
        
       
        Si continuar = "si" Entonces
            Escribir "Continuando con el programa..."
        SiNo
            Escribir "Fin del programa. ¡Hasta luego!"
        Fin Si
    Hasta Que continuar = "no"
FinAlgoritmo

## Ejercicio 34

Algoritmo TablaDeMultiplicar
   
    Definir i, j Como Entero
    
    // Imprimir la tabla de multiplicar del 1 al 9
    Para i <- 1 Hasta 9 Hacer
        Escribir "Tabla de multiplicar del ", i
        Para j <- 1 Hasta 10 Hacer
            Escribir i, " x ", j, " = ", i * j
        Fin Para
        Escribir ""  // Salto de línea después de cada tabla
    Fin Para

FinAlgoritmo

## Ejercicio 35

Algoritmo MayorYMenor
   
    Definir numero, mayor, menor Como Entero
    Definir i Como Entero
    
   
    Escribir "Ingresa el primer número: "
    Leer numero
    mayor <- numero
    menor <- numero
    
    // Ingresar 19 números más y comparar
    Para i <- 2 Hasta 20 Hacer
        Escribir "Ingresa el número ", i, ": "
        Leer numero
        
        
        Si numero > mayor Entonces
            mayor <- numero
        Fin Si
        
        Si numero < menor Entonces
            menor <- numero
        Fin Si
    Fin Para
    
    
    Escribir "El número mayor es: ", mayor
    Escribir "El número menor es: ", menor

FinAlgoritmo

## Ejercicio 36

Algoritmo SerieFibonacci
   
    Definir n, a, b, siguiente, i Como Entero
    
    
    Escribir "Ingresa el número de términos de la serie de Fibonacci: "
    Leer n
    
    // Inicializar los primeros dos términos de la serie
    a <- 0
    b <- 1
    
    Escribir "Serie de Fibonacci hasta el término ", n, ":"
    
    // Imprimir la serie
    Si n >= 1 Entonces
        Escribir a  // Primer término
    Fin Si
    
    Si n >= 2 Entonces
        Escribir b  // Segundo término
    Fin Si
    
    Para i <- 3 Hasta n Hacer
        siguiente <- a + b  // La suma de los dos términos anteriores
        Escribir siguiente   // Imprimir el siguiente término
        a <- b              // Actualizar a al valor de b
        b <- siguiente      // Actualizar b al valor del siguiente término
    Fin Para
FinAlgoritmo

## Ejercicio 37

Algoritmo MCD_Euclides
    
    Definir a, b Como Entero
    
   
    Escribir "Ingresa el primer número (a):"
    Leer a
    Escribir "Ingresa el segundo número (b):"
    Leer b
    
    // Aplicar el algoritmo de Euclides
    Mientras b <> 0 Hacer
        // Guardar el valor de b en una variable temporal
        temp <- b
        
        // Realizar la operación de módulo
        b <- a MOD b
        
        // Actualizar a
        a <- temp
    Fin Mientras
    
    // El MCD es el valor de a
    Escribir "El MCD de los dos números es: ", a

FinAlgoritmo

## Ejercicio 38

Algoritmo NumeroPerfecto
    
    Definir numero, suma, i Como Entero
    
   
    Escribir "Ingresa un número para verificar si es perfecto: "
    Leer numero
    
    // Inicializar la suma de los divisores
    suma <- 0
    
    // Encontrar los divisores propios y sumarlos
    Para i <- 1 Hasta numero - 1 Hacer
        Si numero MOD i = 0 Entonces
            suma <- suma + i
        Fin Si
    Fin Para
    
    // Verificar si el número es perfecto
    Si suma = numero Entonces
        Escribir "El número ", numero, " es un número perfecto."
    SiNo
        Escribir "El número ", numero, " no es un número perfecto."
    Fin Si

FinAlgoritmo

## Ejercicio 39

Algoritmo AproximacionPi
    
    Definir n, i, signo Como Entero
    Definir aproximaciont, termino Como Real
    
   
    aproximaciont <- 0
    signo <- 1  // Usado para alternar entre sumar y restar
    
    // Solicitar al usuario cuántos términos desea usar
    Escribir "Ingresa el número de términos para aproximar pi: "
    Leer n
    
    // Calcular la aproximación de pi usando la serie de Gregory-Leibniz
    Para i <- 0 Hasta n-1 Hacer
        termino <- 4 / (2*i + 1)  // Calculamos el siguiente término de la serie
        aproximaciont <- aproximaciont + signo * termino  // Sumar o restar el término según el signo
        signo <- -signo  // Alternar el signo entre +1 y -1

    Fin Para
    
   
    Escribir "La aproximación de pi con ", n, " términos es: ", aproximaciont

FinAlgoritmo

## Ejercicio 40

Algoritmo AproximacionPiNilakantha
   
    Definir n, i, signo Como Entero
    Definir aproximacionPi, termino Como Real
    
    
    aproximacionPi <- 3  // El valor inicial de la aproximación es 3
    signo <- 1  // Usado para alternar entre sumar y restar
    
    // Solicitar al usuario cuántos términos desea usar
    Escribir "Ingresa el número de términos para aproximar pi: "
    Leer n
    
    // Calcular la aproximación de pi usando la serie de Nilakantha
    Para i <- 1 Hasta n Hacer
        // Calcular el término actual (4 / (n * (n+1) * (n+2)))
        termino <- 4 / ( (2*i) * (2*i+1) * (2*i+2) )
        
        // Sumar o restar el término según el signo
        aproximacionPi <- aproximacionPi + signo * termino
        
        // Alternar el signo
        signo <- -signo
    Fin Para
    
    
    Escribir "La aproximación de pi con ", n, " términos es: ", aproximacionPi

FinAlgoritmo

