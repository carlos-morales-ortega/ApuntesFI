Como ya vimos los criptosistemas se clasifican de acuerdo al tiempo en que fueron desarrollados en:
- Sistema de Cifrado Clásico
- Sistemas de Cifrado Modernos

# Técnicas básicas
## Sustitución
Los caracteres o letras se modifican o sustituyen por otro elementos o lentras en la cifra. Es decir, caracteres distintos a los que tenía el mensaje

## Transposición o permutación
Los caracteres se redistriubyen sin modificarlos y según unas reglas dentro del criptograma.

#### Clasificación sistemas
> Agregar imagen

## Escítala
*Cifrado por transposición*. Una cinta de cuero se enrollaba en un bastón y se escribía el mensaje, al deserrollarlo las letras aparecía desordenas. 
La *"llave"* era el diámetro del bastón y según el bastón era solo de altos mandos.

## Polybios
*Cifrado por sustitución*.
- Usualmente se pide una matriz de 5x5 y se acomodan las letras del alfabeto adentro
	- De 5x5 pq se aproximan más a las 26 letras
- La IJ se ponen juntas 
- **Desventaja**, duplica el tamaño del texto.
- Nosotros escogemos el alfabeto cifrado (C), pueden ser números o letras.

## Cifrado del César
*Cifrado por sustitución monoalfabético* módulo n, siendo n el número de elementos del alfabeto
- Se usa el módulo 27 para el alfabeto
- **Cifrado**: Consiste en desplazar tres letras hacia la derecha los caracteres del texto claro (M).
	- Cifrado: $$ C_i = M_i + 3 mod 27$$
- **Descifrado**: Para descifrar solo se desplaza hacia la izquierda el texto cifrado (C).
	- Descifrado: $$ M_i = C_i - 3 mod 27$$
- ==La llave radica en el #3 

Desventajas: 
La letras cifradas siempre serán iguales. Lo convierte muy vulnerable

## Cifrado por sustitución afín mod 27
Cifrado: $$ C_i = a * M_i + b mod 27$$
Cifrado: $$ M_i = (C_i - b) * a^{-1}  mod 27$$
dónde $$a^{-1}= inv (a,27)$$
- El factor de multi´licación "a" deberá ser **primo relativo** con el cuerpo "n" (En este caso 27) para que exista el inverso de *a*.
- 