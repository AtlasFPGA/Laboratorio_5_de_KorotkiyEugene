# Laboratorio_5_de_KorotkiyEugene

como se muestra en el siguiente vídeo creamos un reproductor de PCM a PWM:



Los ficheros de audio para este taller tienen las siguientes características:


Formato: PCM
Canales: Mono
Bitrate: 176Kbps
Frecuencia de Muestreo: 22050Hz
Tamaño de muestra: 8bit

https://github.com/KorotkiyEugene/digital_lab/blob/master/Lab5/hw/audio_pcm_pwm/SleepAway8.wav

https://github.com/KorotkiyEugene/digital_lab/blob/master/Lab5/hw/audio_pcm_pwm/ac-dc_-_back-in-black_02.wav


Kit lolailo:
https://mega.nz/file/fPx2lbra#B38eZ4uET7x01lmnOk46nwCdXx95EIvU4Ev4YjJhCb8

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

