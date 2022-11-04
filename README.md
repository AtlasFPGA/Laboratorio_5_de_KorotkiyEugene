# Laboratorio_5_de_KorotkiyEugene

como se muestra en el siguiente vídeo creamos un reproductor de PCM a PWM:
https://www.youtube.com/watch?v=PxQIcnW ... v&index=25
Los ficheros de audio para este taller tienen las siguientes características:

Formato: PCM
Canales: Mono
Bitrate: 176Kbps
Frecuencia de Muestreo: 22050Hz
Tamaño de muestra: 8bit

Ficheros wav:
https://github.com/KorotkiyEugene/digit ... pAway8.wav
https://github.com/KorotkiyEugene/digit ... ack_02.wav
Kit lolailo:
https://mega.nz/file/fPx2lbra#B38eZ4uET ... Ev4YjJhCb8
Indentificamos 8bit 2 bit de parada:
La aplicación que me ha funcionado en windows es SmarTTY:
https://sysprogs.com/SmarTTY/
Con la siguiente configuración: 

Envío de datos en Hexadecimal
bits: 230400
data bits: 8
parity: mark
stop bits: 2
flow control: none

os comandos en linux son: 
stty -F /dev/ttyUSB0 230400 cs8 cstopb -parenb

cat nombre_fichero* > /dev/ttyUSB0

