
# Primeiro teste com LoRA
##  Material utilizado
### Lora32u4 II 
![enter image description here](https://raw.githubusercontent.com/nunosilvarocha/LoRa32u4_II_com_LMiC/master/Img/Lora32u4_II.jpg?token=AgTL5uf7T2hwvR9SZYJILOTP81oJ04Msks5bFw5IwA%3D%3D)
[Datasheet](https://docs.bsfrance.fr/documentation/11355_LORA32U4II/Datasheet_LoRa32u4II_1.1.pdf "Datasheet")
[Página do fabricante](https://bsfrance.fr/lora-long-range/1345-LoRa32u4-II-Lora-LiPo-Atmega32u4-SX1276-HPD13-868MHZ-EU-Antenna.html "Página do fabricante")

>  Microcontrolador
>- ATmega32u4 @ 8MHz
>- 32 K Flash, 2 K  RAM
>- Regulador 3.3V, 600mA (peak current output)
>- Porta USB com FTDI para programação de debug
>- Ligação para bateria (carregador integrado) 
> 
> Modulo LoRa 
>- LoRa SX1276 HPD13 
>- Frequência de 868MHZ (Norma Europeia)
>- Interface SPI
#### Arduino IDE
> Versão [1.8.5](https://www.arduino.cc/en/Main/Software)
>  *Possivelmente funciona com outras versões, esta foi a que eu usei.*
#### Biblioteca LMIC
> [LMIC](https://github.com/matthijskooijman/arduino-lmic)


## Preparação
### LoRa32u4 II Drivers

 > - Download e instalação dos [drivers](https://github.com/adafruit/Adafruit_Windows_Drivers/releases/download/2.2.0/adafruit_drivers_2.2.0.0.exe)

### Arduino IDE setup
 > - Download e instalação do [Arduino IDE](https://www.arduino.cc/en/Main/Software)<p>
 >
 > - Ficheiro > Preferências
 > - URL Adicionais do Gestor de Placas > Adicionar o link abaixo `https://adafruit.github.io/arduino-board-index/package_adafruit_index.json`<p>
 >
 > - Ferramentas > Placa > Gestor de Placas...
 > - Selecionar o tipo "Contribuído"
 > - Pesquisar por "Adafruit AVR Boards"<p>
 >
 > - Ferramenstas > Board > Adafruit Feather 32u4
 > - Ferramentas > Porta > Selecionar a porta<p>
 >
 > - Fazer download da biblioteca [LMIC](https://github.com/matthijskooijman/arduino-lmic)
 > - Rascunho > Incluir Biblioteca > Adicionar Biblioteca .ZIP
 > - Selecionar o .ZIP do ficheiro descarregado

## LMiC_raw
É um emplo para ser usado em dois LoRa32u4 II.
Os dois enviam e aguardam mensagens.

! É preciso altera o ficheiro config.h
Abilitar o #define DISABLE_INVERT_IQ_ON_RX
