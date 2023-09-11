# Tutorial: Setup Rota 2030  
1- Ligar o inversor

<img src="media\Inversor_ROTA2030.jpg"
width="200px"/>

2- Ligar o benjamim

<img src="media\Benjamin_ROTA203-.jpg"
width="200px"/>

3 - Ligar a Jetson
 
<img src="media\Jetson_ROTA2030.jpg"
width="200px"/>

4 - Conectar o cabo em baixo do volante

<img src="media\Cabo_ROTA2030"
width="200px"/>

5 - Ligar o PCAN Router (da esquerda para a direita)

<img src="media\PCANRouter_ROTA2030"
width="200px"/>

# Tutorial: Terminal jetson Rota 2030

Passo 1: Ligar as coisas

    Verifique as conexões de alimentação em todos os dispositivos mencionados (benjamim, Jetson, caixa de alimentação, carro). Certifique-se de que eles estão conectados corretamente e que estão recebendo energia.

    Ligue o inversor, se necessário, para fornecer energia aos dispositivos.

    Ligue o carro.

    Conecte o OBD2 ao carro.

    Conecte o PCAN USB ao seu sistema.

Passo 2: Configurar o ambiente de software

    Abra um terminal.

    Entrar no WS.

    Divida a tela em três terminais diferentes para facilitar a execução dos comandos.

    Source run.sh em todas as telas

    Sudo ip link set can0 up type can bitrate 500000

Após configurar a interface CAN, você pode executar o seguinte comando em um dos terminais para iniciar um lançamento do ROS (Robotic Operating System):

    roslaunch radar_rviz_pkg launch_das.launch

No segundo terminal, execute o seguinte comando para executar o software principal:

    rosrun radar_rviz_pkg main.py


Observações:

    Certifique-se de que todos os pacotes e dependências do ROS necessários estão instalados no seu ambiente.

    Os comandos e caminhos para os arquivos podem variar dependendo da sua configuração e do local dos arquivos no seu sistema. Ajuste-os de acordo com a estrutura do seu projeto.

    Certifique-se de ter as permissões adequadas para executar os comandos, especialmente os que requerem privilégios de superusuário (sudo).

    Certifique-se de que o hardware (Jetson, OBD2, PCAN USB, etc.) está configurado corretamente e todos os drivers estão instalados.







