# PWM de la RP2040
- Hasta 8 pwm
- Modulación 0-65535

## 'Damo_PWM_Base'
- Varia intensidad del les P25
- Frecuencia base 50 khz
- Modulación rangos de 256

## Estructura
1. Habilita Pin, PWM sleep
2. PW0 = PWM(pin25)
3. While
	1. Modulación = 0
	2. For 
	   PWM.dutu_V16(Modulación INCR 256
	3. PWM apagada 1 seg