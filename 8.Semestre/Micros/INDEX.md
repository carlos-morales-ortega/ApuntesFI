# Comparación


| (A - B)   | Resultado | C   | Z   |
| --------- | --------- | --- | --- |
| A mayor B | Positivo  | 1   | 0   |
| A = B     | Cero      | 1   | 1   |
| A menor B | Negativo  | 0   | 0   |
## Registros iguales
```c
	BTFSS STATUS, Z //Skip if Set, Salta si es 1
GOTO NO_IGUALES				//Salta si son iguales
IGUALES:
	
```

## Registro A mayor o igual que B
```c
	BTFSS STATUS, C //Skip if Set, Salta si es 1
GOTO A_NO_MAYOR_O_IGUAL				//Salta si son iguales
MAYOR_O_IGUALES:
	
```