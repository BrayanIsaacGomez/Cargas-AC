# Cargas-AC
PCB capaz de controlar el modo ON/OFF de 3 cargas AC, estimar el consumo de voltaje y corriente AC de una de las cargas

El dispositivo contiene:

- ESP32
- NeoPixeles
- Buzzer
- SHT30
- Control de cargas AC

# ¿Cómo funciona?



# ¿Qué podemos hacer?




# Descripción de pines 

### Pantalla OLED SSD 1306, Temperatura y Humedad – Comunicación I2C
| SSD 1306 | --- | SHT30 |
ESP32            | SCL IO22 | --- | SCL IO22 |
| SSD 1306| --- | SHT30 | 
| SCL IO22 | -- | SCL IO22 |
| SDA IO23 | -- | SDA IO23 |

### Control Cargas AC 
Referencia --- | CARGA 1 | --- | CARGA 2 | --- | CARGA 3 |
ESP32          |  IO25   | --- |  IO26   | --- |  IO27   | 

### LED Neopixel - Comunicación SPI
Referencia --- | WS2812B | 
ESP32            |   SD3   |
5V | VCC 

GND | GND


### Control Cargas AC 
Referencia --- | SCT 013 | --- | Voltaje AC |
ESP32          |  IO15   | --- |     IO2    |
               | ADC2_2  | --- |   ADC2_3   |
# Licencia

Hardware License: CERN OHL v1.0 para más información visitar el siguiente [Link][CERN_v1].

[CERN_v1]: https://ohwr.org/project/cernohl/wikis/Documents/CERN-OHL-version-1.2

Software License: GPL v3

Documentation License: CC BY 4.0 International
