# Frequency-response
This application gives the frequency responce of a system where the input signal is between 50 Hz and 1 KHz.

For measuring the output spectrum of a system with input signal frequency between 50 Hz and 1 Khz I use Tiva TM4C123GH6PM microcontroller. 
  First thing I make is to generate PWM signals with different duty cycles representing a sine wave. After that I use a low-pass filter to   filter the high frequencies of a PWM's and actually make a smooth sine wave. After  I make a sine wave with a desired frequency I start   change the frequency with a fixed step. After that I sample the output signal of the system with a TIVA TM4C123GH6PM ADC and calculate     at which frequencies the amplitude of the signal goes down with 3 dB.
