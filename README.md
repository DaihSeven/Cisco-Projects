# Cisco-Projects
Projetos iniciais usando Cisco Packet Tracer
# Definir o cenário: 
Neste projeto, estou trabalhando para o show da banda de Miguel e preciso configurar uma rede de computadores para a equipe de produção. 
Cada membro da equipe tem um computador que precisa estar conectado à rede para se comunicar com os outros.
# Montar a topologia: 
Usei o Cisco Packet Tracer para criar uma topologia de rede estrela. Primeiro, criei uma nova topologia no programa. 
Em seguida, arrastei um switch para o centro da área de trabalho. Depois, arrastei quatro PCs e posicionei-os ao redor do switch. 
Cada PC representa um membro da equipe de produção.
![Topologia](/Projeto%20cisco-%20Miguel/prints/Captura%20de%20tela%202024-06-13%20195116.png)

# Conectar os dispositivos: 
Foi necessário conectar cada PC a uma porta diferente no switch usando cabos ethernet. Isso formou uma estrela com os computadores da 
equipe de produção ao redor do switch central.
# Configurar os endereços IP: 
Cada computador precisa ter um nome e um número de endereço IP. Configurei os endereços IP para as interfaces dos PCs e do switch. 
Todos eles devem estar na mesma sub-rede.
![Endereço IP](/Projeto%20cisco-%20Miguel/prints/Captura%20de%20tela%202024-06-13%20141913.png)

# Testar a comunicação: 
Para verificar se todos os computadores estão configurados corretamente, acessei um dos PCs da equipe, abri o prompt de comando e fiz um ping para o endereço IP do computador de outro membro da equipe. E fiz o mesmo com os outros dois restantes.

Cliquei no PC que iria usar para o teste (neste caso, o PC com o endereço IP 192.168.10.3).
Na janela que se abre, cliquei em Desktop e depois em Command Prompt.
No prompt de comando, digitei o seguinte comando: ping 192.168.10.2 e pressionei Enter.

## O que ocorre:

O comando ping envia um pacote de dados para o endereço IP especificado (neste caso, 192.168.10.2) e aguardará uma resposta. Se o PC com o endereço IP 192.168.10.2 estiver configurado corretamente e conectado à rede, ele responderá ao ping e você verá a resposta no prompt de comando.
Se você receber uma resposta, isso significa que a comunicação entre os dois PCs está funcionando corretamente. Se você não receber uma resposta, pode haver um problema com a configuração da rede ou com o PC que você está tentando alcançar.

## Quando você executa o comando ping no prompt de comando, a resposta que você recebe normalmente se parece com isto:

Pinging 192.168.10.2 with 32 bytes of data:
Reply from 192.168.10.2: bytes=32 time<1ms TTL=128
Reply from 192.168.10.2: bytes=32 time<1ms TTL=128
Reply from 192.168.10.2: bytes=32 time<1ms TTL=128
Reply from 192.168.10.2: bytes=32 time<1ms TTL=128

Ping statistics for 192.168.10.2:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms

Isso significa que o computador com o endereço IP 192.168.10.2 está respondendo aos pings, indicando que a comunicação entre os dois computadores está funcionando corretamente.

## Se o computador não estiver respondendo, você verá uma mensagem como esta:

Pinging 192.168.10.2 with 32 bytes of data:
Request timed out.
Request timed out.
Request timed out.
Request timed out.

Ping statistics for 192.168.10.2:
    Packets: Sent = 4, Received = 0, Lost = 4 (100% loss),

Isso indica que o computador com o endereço IP 192.168.10.2 não está respondendo, o que pode significar que há um problema com a configuração da rede ou com o próprio computador.

# Teste e Resposta do meu prompt
![Prompt](/Projeto%20cisco-%20Miguel/prints/Captura%20de%20tela%202024-06-13%20141841.png)
![Prompt](/Projeto%20cisco-%20Miguel/prints/Captura%20de%20tela%202024-06-13%20142243.png)
![Prompt](/Projeto%20cisco-%20Miguel/prints/Captura%20de%20tela%202024-06-13%20142642.png)


