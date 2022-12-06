# Semana03Lunes.md
Semana 03 - Día Lunes - 06/12/2022

# Calculadora

Algoritmo Calculadora
	
	//Solicitar dos números y validar que son enteros
	
	RestoX <- 0
	RestoZ <- 0
	
	Repetir
		
		Si RestoX <> 0 O RestoZ <> 0
			
			Limpiar Pantalla
			Imprimir " Introduzca nuevamente ambos valores "
			Imprimir "                                   "
			
		FinSi
		
		Imprimir " Introduzca el primer valor entero "
		Leer X
		Imprimir " Introduzca el segundo valor entero "
		Leer Z
		
		RestoX <- X - Trunc(X)
		RestoZ <- Z - Trunc(Z)

	Hasta Que RestoX = 0 & RestoZ = 0
	
	Repetir
		
		Imprimir " Indique la operación que desea realizar: "
		Imprimir "                   "
		Imprimir " Operaciones válidas: Suma + "
		Imprimir " Operaciones válidas: Resta - "
		Imprimir " Operaciones válidas: Multiplicación * "
		Imprimir " Operaciones válidas: División / "
		
		Leer OP
		
		Si OP = "+" O OP = "-" O OP = "*" O OP = "/"
			
			Entonces
			
				Si OP = "+"
				
					Resul <- X + Z
					Imprimir " El resultado de la suma es ", Resul
					
				FinSi
				
				Si OP = "-"
					
					Resul <- X - Z
					Imprimir " El resultado de la resta es ", Resul
					
				FinSi
				
				Si OP = "*"
					
					Resul <- X * Z
					Imprimir " El resultado de la multiplicación es ", Resul
					
				FinSi
				
				Si OP = "/"
					
					Resul <- X / Z
					Imprimir " El resultado de la división es ", Resul
					
				FinSi
					
			Sino
				
				Limpiar Pantalla
				Imprimir " La operación no existe, introduzcala nuevamente  "
				Imprimir "                   "
				
		FinSi
			
	
	Hasta Que OP = "+" O OP = "-" O OP = "*" O OP = "/"
	
FinAlgoritmo


