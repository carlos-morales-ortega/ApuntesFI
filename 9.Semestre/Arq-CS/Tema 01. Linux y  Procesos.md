# Introducción a Linux


---
# Procesos
Un proceso es una instancia de un programa ejecutable. Se compone de:
- Segmento de texto: Instrucciones para la CPU
- Segmento de datos: datos que son cargados al inicio del proceso
- Segmento de pila: serie de bloques lógicos *Marcos de Pila* similar al (SP).
Linux es multi proceso, el planificador se encarga de gestionar CPU y determinar que proceso pasa por el CPU.

Son creados tras la llamada **fork()**, todo los procesos excepto *init()* son creados con fork. El proceso que llama a fork se conoce como padre y el que se crea como hijo.

Cada proceso es identificado por un *ID de proceso o PID*. Número entero positivo que es asignado cada que un nuevo proceso es creado. 

---
# Desarrollo
## Número de procesos

```C
#include<stdio.h>
#include<unistd.h>

int main()
{
  printf("El process id es %d\n", getpid());
  printf("El parent process id es %d\n", getppid());
  return 0;
}
```
Al ejecutar desde una terminal el proceso padre no cambia porque se ejecuta desde el mismo shell, pero se observa que el proceso hijo si cambia.

Además del PID y PPID, cada proceso tiene los siguientes:

| Atributo            | Tipo  | Función       |
| ------------------- | ----- | ------------- |
| ID proceso          | pid_t | getpid(void)  |
| ID proceso padre    | pid_t | getppid(void) |
| ID real de usuario  | uid_t | getuid(void)  |
| ID efectivo usuario | uid_t | geteuid(void) |
| ID real de grupo    | gid_t | getgid()      |
| ID efectivo egrupo  | gid_t | getegid()     |
