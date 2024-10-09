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

### Configuração do ESP32

#### Instalação do Driver para o ESP32

1. **Baixe e Instale o Driver:**

    - Antes de conectar o ESP32 ao seu computador, é necessário instalar o driver adequado para garantir que o dispositivo seja reconhecido corretamente. Você pode encontrar o driver específico para o ESP32 no seguinte link: [Instalação do Driver para ESP32 - RoboCore](https://www.robocore.net/tutoriais/instalando-driver-do-nodemcu)
    - Siga as instruções no site para baixar e instalar o driver correspondente ao seu sistema operacional.
    - Caso o driver seja instalado e a porta COM do ESP ainda não aparecer identifique se o cabo possui transferencia de dados ou se apenas serve para carregamento.
      
2. **Conectar o ESP32 ao Computador:**

    - Após a instalação do driver, conecte o ESP32 ao computador usando um cabo USB. Se tudo estiver correto, o dispositivo deverá ser reconhecido e uma nova porta COM será listada no seu sistema.

#### Configuração no Arduino IDE

3. **Instale o Arduino IDE:**

    - Se ainda não instalou, baixe e instale o Arduino IDE diretamente do site oficial: [Arduino - Software](https://www.arduino.cc/en/software)

4. **Adicione a URL de Gerenciamento de Placas do ESP32:**

    - Abra o Arduino IDE.
    - Vá em **Arquivo > Preferências**.
    - No campo "URLs Adicionais de Gerenciadores de Placas", adicione a seguinte URL para permitir a instalação do pacote do ESP32:

		```
	  https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
		```

5. **Instale o Pacote do ESP32:**

    - Acesse **Ferramentas > Placa: > Gerenciador de Placas**.
    - Na barra de pesquisa, digite "ESP32".
    - Localize "esp32 by Espressif Systems" e clique em "Instalar".

6. **Selecionar a Placa ESP32 e a Porta COM:**

    - Após a instalação do pacote, vá em **Ferramentas > Placa** e selecione o modelo do seu ESP32 na lista sob o título "NodeMCU-32S".
    - Vá em **Ferramentas > Porta** e selecione a porta COM que aparece (associada ao ESP32).

### Instalação das bibliotecas necessárias no Arduino IDE

Para instalar todas as bibliotecas necessárias, abra o Arduino IDE, vá em Sketch > Incluir Biblioteca > Gerenciar Bibliotecas, e procure e instale as seguintes bibliotecas:

- L298N-DC-Motor by Robojax


### Upload do código para o ESP32

7. **Baixe o arquivo presente no repositório e abra-o no Arduino IDE**

8. **Selecione a placa como descrito na etapa 6 e clique na seta voltada para esquerda para realizar o upload**

*Neste ponto o ESP32 deve estar ligado e com o código já carregado nele*

### Pareamento com o celular

9. **Ligue o Bluetooth do celular e pareie com o ESP32 "BT_Node12"**

### Download do aplicativo de controle dos motores

10. **No celular, abra a loja de aplicativos e busque pelo app Arduino Bluetooth Control**

### Conexão e configuração do aplicativo com o ESP32

11. **Abra o aplicativo, conecte com o BT_Node12**

12. **Abra a aba "Buttons & Slider"**

13. **Clique no rostinho de robô no canto superior direito**

14. **Desça até a seção BUTTONS AND SLIDER > Command buttons configuration**

*Coloque as letras em maiúsculo para que o controlador entenda*

15. **Clique em Button A e insira a letra F *Para ir para frente*** 

16. **Clique em Button B e insira a letra B *Para ir para trás***

17. **Clique em Button B e insira a letra R *Para ir para direita***

18. **Clique em Button B e insira a letra L *Para ir para esquerda***

19. **Clique em Button B e insira a letra S *Para parar***

*Outros modos de comandos podem ser utilizados, porém configurando com as mesmas letras*

Divirta-se !!!
