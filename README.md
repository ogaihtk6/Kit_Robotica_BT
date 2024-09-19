# Kit Robótica Bluetooth

Este kit acompanha os seguintes componentes:
- 1x ESP32S
- 1x Conector de bateria 9V
- 1x L298N
- 4x Jumpers Fêmea X Fêmea
- 1x Jumper Fêmea X Macho
- 1x Cabo microUSB
  
Para o devido funcionamento siga o circuito indicado abaixo.

Circuito:
![Circuito kit_bt](https://github.com/user-attachments/assets/e581a6c2-ff92-47bf-b90a-26fdebba327b)


Para utilizar o kit siga o seguinte passo a passo:

1 - Instale a Arduino IDE: https://www.arduino.cc/en/software

2 - Dentro da IDE, vá em Arquivos > Preferências e na caixa de texto insira o link: https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json

3 - Extraia a pasta compactada presente no repositório para a pasta das bibliotecas da Arduino IDE

4 - Abra o código presente na pasta kit_bt

5 - Conecte o ESP32S no computador

6 - Selecione a placa NodeMCU-32S com a porta COM que aparecer e faça o upload

*Neste ponto o ESP32 deve estar ligado e com o código já carregado nele*

7 - Ligue o Bluetooth do celular e pareie com o ESP32 "BT_Node12"

8 - No celular, abra a loja de aplicativos e busque pelo app Arduino Bluetooth Control

9 - Abra o aplicativo, conecte com o BT_Node12 

10 - Abra a aba "Buttons & Slider"

11 - Clique no rostinho de robô no canto superior direito

12 - Desça até a seção BUTTONS AND SLIDER > Command buttons configuration

*Coloque as letras em maiúsculo para que o controlador entenda*

13 - Clique em Button A e insira a letra F *Para ir para frente* 

14 - Clique em Button B e insira a letra B *Para ir para trás*

15 - Clique em Button B e insira a letra R *Para ir para direita*

16 - Clique em Button B e insira a letra L *Para ir para esquerda*

17 - Clique em Button B e insira a letra S *Para parar*

*Outros modos de comandos podem ser utilizados, porém configurando com as mesmas letras*

Divirta-se !!!
