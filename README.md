# ATMEGA328-Software-Serial
For Atmel Studio:
Software serial library for Atmel ATmega328 microcontroller. The serial communication works at 9600 baud.


#Note: This library based on https://github.com/dadez87/SWseriale, But I only modified it to work from ATMEL Studio with Atmega328 directly without Arduino

This is a Software serial library for Arduino (equipped with Atmel ATmega328 microcontroller and similar).
In its standard configuration, the serial communication works at 9600 baud using PIND3 (RX) and PIND4 (TX). 
It makes use of INT1 interrupt and Timer2 8 bit timer.
Both sending and receiving operations use Timer2 for the bit timing: it is not possible to send and receive at the same time. Therefore, the communication can be only half-duplex.
