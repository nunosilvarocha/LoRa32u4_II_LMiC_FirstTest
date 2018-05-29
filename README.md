# Primeiro teste com LoRA
####  Material utilizado
##### Lora32u4 II 
[![Lora32u4_II PinOut](Lora32u4_II "Lora32u4_II PinOut")](https://github.com/nunosilvarocha/LoRa32u4_II_com_LMiC/blob/master/Img/Lora32u4_II.jpg "Lora32u4_II PinOut")
[Datasheet](https://docs.bsfrance.fr/documentation/11355_LORA32U4II/Datasheet_LoRa32u4II_1.1.pdf "Datasheet")
[Página do fabricante](https://bsfrance.fr/lora-long-range/1345-LoRa32u4-II-Lora-LiPo-Atmega32u4-SX1276-HPD13-868MHZ-EU-Antenna.html "Página do fabricante")
>  
- Microcontrolador
  - ATmega32u4 @ 8MHz
 - 32 K Flash, 2 K  RAM
 - Regulador 3.3V, 600mA (peak current output)
 - Porta USB com FTDI para programação de debug
 - Ligação para bateria (carregador integrado) 
- Modulo LoRa 
 - LoRa SX1276 HPD13 
 - Frequencia de 868MHZ (Norma Europeia)
 - Interface SPI



# LoRa32u4_II_com_LMiC

> ##Baseado em:
>https://github.com/matthijskooijman/arduino-lmic

## LMiC_raw
É um emplo para ser usado em dois LoRa32u4 II.
Os dois enviam e aguardam mensagens.

! É preciso altera o ficheiro config.h
Abilitar o #define DISABLE_INVERT_IQ_ON_RX
