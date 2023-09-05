# Tutorial: Setup Rota 2030  
1- Ligar o inversor

<!-- ![inversor](https://github.com/BrunoMalena/documentation/blob/main/media/Inversor_ROTA2030.jpg) -->

<img src="media\Inversor_ROTA2030.jpg"
width="200px"/>

2- Ligar o benjamim

<!-- ![benjamim](https://github.com/BrunoMalena/documentation/blob/main/media/Benjamin_ROTA203-.jpg) -->

<img src="media\Benjamin_ROTA203-.jpg"
width="200px"/>

3 - Ligar a Jetson

<!-- ![jetson](https://github.com/BrunoMalena/documentation/blob/main/media/Jetson_ROTA2030.jpg) -->

<img src="media\Jetson_ROTA2030.jpg"
width="200px"/>

4 - Conectar o cabo em baixo do volante

<!-- ![cabo](https://github.com/BrunoMalena/documentation/blob/main/media/Cabo_ROTA2030) -->

<img src="media\Cabo_ROTA2030"
width="200px"/>

5 - Ligar o PCAN Router (da esquerda para a direita)

<!-- ![pcan](https://github.com/BrunoMalena/documentation/blob/main/media/PCANRouter_ROTA2030) -->

<img src="media\PCANRouter_ROTA2030"
width="200px"/>

# Tutorial: Terminal jetson Rota 2030

Abra o terminal do Terminator.

Pressione Ctrl + R para abrir o histórico de comandos.

Digite o seguinte comando e pressione Enter para navegar até a pasta "ros_ws" (ou o diretório que você mencionou): bash cd Documents/ros_ws

Abra outras duas janelas do Terminator (botão direito - dividir verticalmente ou horizontalmente).

Terminal 1:

No primeiro terminal, pressione Ctrl + R novamente e comece a digitar o comando. Quando encontrar o comando "sudo IP link...", execute-o.

Aguarde sem fechar o terminal.

Terminal 2:

No segundo terminal, digite o seguinte comando e pressione Enter: source run.sh

Ele solicitará a senha da Jetson, que é "rota2030"

Terminal 3:

No terceiro terminal, digite o seguinte comando e pressione Enter: roscore

Aguarde até que os componentes do ROS sejam inicializados

Terminal 2 (novamente):

No segundo terminal, pressione Ctrl + R novamente e comece a digitar o comando: roslaunch

Pressione Enter. Isso iniciará um código que exibirá "fuzzy: 0" na tela

Terminal 3 (novamente):

No terceiro terminal, pressione Ctrl + R novamente e digite o seguinte comando: rosrun

Uma janela aparecerá, mas volte sua atenção para este terminal. Ele está pedindo que você insira o nome da pessoa, o número de repetições e o tipo de alerta. Para o tipo de alerta, insira apenas "v", "h" ou "hv". Preencha as informações necessárias

Feche a janela da interface que está aberta, verifique se as imagens foram salvas e outros detalhes.

Terminal 3 (novamente):

Volte para o terminal 3, pressione Ctrl + R novamente e digite: rosrun







