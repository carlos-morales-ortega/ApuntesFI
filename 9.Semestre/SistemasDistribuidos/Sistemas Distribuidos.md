-
# High Performance Computing
- Cómputo de Alto Rendimiento
- Cómputo de Alto Desempeño
### Introducción
- Técnicas Computacionales que ayudan a solucionar problemas compleos (comunmente científicos, ingenieriles o de negocios), más rápidos utilizando la informátia típica.
- Ejecución serial/secuencial. Tareas instrucciones a la vez.
- Ejecución paralela. Varias tareas instrucciones ejecutadas simultaneamente 
- Memoria compartida: las diferentes unidades de computo CPU comparten una memoria común a la cual tienen acceso en igualdad de condiciones.
- Memoria distribuida: las dif. CPU tienen memoria propia, a la cual los demás no tienen accesso directo.

---
# Pseudocódigos
### Hola mundo
``` java
public void main(){
	println("Hola mundo");

}
```

### Programa que realiza la suma de 2 variables
```java
public void main(){
	int a = 3;
	int b = 2;
	int c = a+b;
	println(c);
}
```

### Programa que hace la suma en una función
``` java
public void main(){
	int c = suma(2,3);
	println(c);
}

public int suma(int a, int b){
	return a+b;
}
```

### Arreglo de 5 posiciones incializadas con i
```java
/*public void main(){
	int a[]={1,2,3,4,5}
}*/

public void main(){
	int [] a = new int[5]
	for (int i=0; i=5; i++){
		a[i] = i+1;
	}
}
````

### Ahora sumando el arreglo
```java
/*public void main(){
	int a[]={1,2,3,4,5}
}*/

public void main(){
	int [] a = new int[5];
	int suma = 0;
	for (int i=0; i=5; i++){
		a[i] = i+1;
		suma+= i+1; //
	}
}
````