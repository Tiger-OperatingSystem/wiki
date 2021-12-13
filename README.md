> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/capa.png)

O TigerOS é disponibilizado ao público na forma de uma [imagem ISO](https://pt.wikipedia.org/wiki/Imagem_ISO), que deve ser gravada em um Pendrive ou ainda, DVD. Essa imagem ISO funciona de 2 formas: Modo Live e Instalação.

## Modo Live 

Nesse modo você pode rodar todo o TigerOS de maneira funcional, sem precisar instalar, podendo testar se todo o hardware está funcionando.
O modo Live também permite que se acesse um HD com Windows e se recupere arquivos.

## Modo Instalação

Nesse modo que é acionado através do modo live clicando no ícone de instalação na área de trabalho:

<!-- Adicionar imagem do modo indicando como iniciar a instalação a partir do live aqui -->

Nesse modo o Tiger OS é efetivamente instalado no computador

# Processo de instalação

### 1. Baixando o Tiger OS

No momento atual, o TigerOS possui apenas uma versão, a Enterprise Desktop, que pode ser [baixada através desse link](https://bit.ly/3xAtKsB)

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/000.png)


### 2. Criando um pendrive para o modo live

> Nota: Para criar um Live Pendrive, é necessário um programa específico chamado Ventoy. Mas existem outros, como Rufus.
> O download pode ser feito [a partir desse link](https://github.com/ventoy/Ventoy/releases/latest)
> 
> Basta clicar na opção para Windows e iniciar o download.
> 
> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/01.png)
> 
> Não se preocupe se os números não forem os mesmo quando você entrar nessa página.
> 
> Quando concluir o processo de download, vá para a pasta na qual o arquivo foi salvo e descompacte-o
> 
> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/02.png)

#### Passo 1 - O dispositivo USB

Caso seu pendrive já não esteja conectado a uma porta USB, faça-o agora.

> **Nota:** tenha em mente que o dispositivo USB será formatado durante o processo, lembre-se de fazer backup de arquivos importantes

#### Passo 2 - Iniciando o Ventoy

Dentro da pasta do Ventoy para Windows, existe outra ainda com o nome e a versão do programa.  Clique em Ventoy2Disk.
Veja que em device (1), aparece detalhes sobre meu pendrive, inclusive o tamanho dele

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/03.PNG)

> Clique em Install, note que esse processo ira apagar todos os dados no dispositivo USB (pendrive)

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/04.PNG)

Terminado o processo, que deve demorar menos de 1 minuto, a seguinte mensagem aparecerá:

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/05.PNG)

Isso significa que a partir de agora, seu dispositivo agora é um _**live pendrive**_ estando apto a receber o TigerOS. Você pode fechar a janela agora

#### Passo 3 - Adicionando o Tiger OS ao pendrive

Vá até a pasta que salvou a ISO do TigerOS e, clicando com o botão direito, selecione copiar.

Agora, na barra da esquerda, procure por Ventoy e cole o arquivo dentro do live pendrive.

![Processo de cópia da ISO](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/07.png)

Agora basta aguardar o fim da cópia do arquivo que esta parte estará pronta.

#### Passo 4 - Redimensionar HD com Windows 10 para Dual Boot

Terminada a criação do Live Pendrive, caso você queira manter o Windows e adicionar o TigerOS, passa a ser necessário agora, reduzir a partição do Windows 10, para o caso de dual boot, para em seguida, configurar a BIOS de sua máquina, para que seja possível detectar o dispositivo na inicialização.

No w10, clicando sobre a barra de tarefas, procure pela opção Gerenciamento de disco.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/redimensionarHD/01.png)

O seguinte programa será aberto:

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/redimensionarHD/02.png)

Temos aqui algumas opções de particionamento já feitos para essa instalação do Windows, que pode ser diferente da sua máquina.

Vamos nos atentar aqui ao disco C:
Clicando com o botão direito do mouse, selecione a opção Diminuir volume.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/redimensionarHD/03.PNG)

Dependendo do tamanho do seu HD e também da quantidade de arquivos e programas já instalados, você pode considerar deixar aí uns 30 gb ou mais para o TigerOS.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/redimensionarHD/04.PNG)

Uma conta rápida: 1024 x 30gb = 30720, o tamanho exato da partição.
Sim, você pode colocar 30.000 ou outro valor.

Na terceira opção: diminuir o espaço em MB: digite o valor de 30720.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/redimensionarHD/05.PNG)

Clique então em Diminuir.

Agora aguarde o processo de redimensionamento ser efetuado, o que pode ser demorado em sua máquina.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/redimensionarHD/06.PNG)

Agora será necessário configurar a BIOS da máquina para conseguir acessar o pendrive gravado anteriormente, conseguindo assim, então, instalar o TigerOS.

Antes de mais nada tenho que destacar aqui: devem existir centenas de BIOS diferentes, então óbvio, não tenho como mostrar cada 1 delas. A forma de acessar, também varia, embora as mais comuns sejam pelas teclas F2 ou Del.

Algumas BIOS possuem particularidades para poder desabilitar o Secure Boot, sendo que dependendo do caso, você terá que pesquisar e testar.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/bios/01.png)

Nessa imagem, por exemplo, informa que é necessário pressionar F2.

Porém, nessa outra BIOS, entre diversas informações, descobrimos que é necessário pressionar a tecla Del

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/bios/02.png)

Aqui começaremos procurando pela opção de segurança, no qual será desabilitado e Secure Boot, mudando a opção Enable para Disable.

Na opção UEFI/Legacy Boot, certifique-se de selecionar a opção Legacy.
Em algumas BIOS a opção de colocar como automático está disponível, podendo ser a escolhida.

É verdade que o TigerOS funciona com o UEFI, mas pode ser que apresente problemas. Então, num primeiro momento, selecione Legacy ou automático.

Agora configuraremos a ordem de boot, para que ele acesse o pendrive na hora que reiniciar a máquina.
De novo: o nome exato pode mudar em sua máquina, mas se vocẽ seguir a lógica, não deve ter dificuldades.

Procure por algo como Boot ou ainda, Boot Priority Order.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/bios/03.png)

Aqui aparece a opção USB, que foi colocada como primeira. Usei as setas de F5 e F6 para alterar a ordem.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/bios/04.png)

Mas de novo: não existe uma forma única de proceder.

Agora será necessário salvar as configurações para reiniciar a máquina. Para isso, basta pressionar a tecla f10 e confirmar a gravação.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/bios/05.png)

Sua máquina reinicializará pronta para acessar o pendrive e mostrar a tela de boot do TigerOS.

Caso não funcione, e isso infelizmente pode ocorrer, é possível usar as teclas de atalho para alterar a ordem de boot, usando a tecla f12 ou f11.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/bios/06.png)

De novo: se não funcionar nenhuma das duas, basta pesquisar.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/bios/07.png)

Nesta imagem vemos que a opção de USB já está selecionada, mas caso o USB estivesse em outra posição, seria preciso selecionar, usando as setas do teclado.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/01.png)

Pronto, essa é a tela de grub do TigerOS. Como não foi detectada nenhuma placa de vídeo diferente da básica, apenas foi informado o nome e a versão do sistema, com a confirmação de que se está no modo Live.

Caso você tenha uma placa de vídeo 3d mais exótica, uma segunda opção no menu pode aparecer.

Agora aguarde a inicialização do TigerOS 21, no modo Live.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/02.png)
Essa tela chama-se plymouth.


Se a gravação do live pendrive funcionou corretamente, o TigerOS carregará e mostrará essa tela:

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/03.png)

Antes de mais nada, vamos verificar se a sua conexão com a internet está ok.

Nesta imagem, no canto inferior direito, vemos que o TigerOS detectou e se conectou a uma rede cabeada.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/04.png)

Já nesta imagem, vemos que não há conexão nenhuma. 

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/05.png)

Logo, se sua máquina tiver uma placa wireless, ao clicar nesse ícone, as opções de rede devem aparecer.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/06.png)

Caso não apareça NADA, pode ser que a placa esteja desativada ou ainda, que precisa de um driver. Nesse caso, consulte o guia mais detalhado para resolver esse problema.
Nessa lista vemos uma relação de todas as redes wireless que foram detectadas, além de uma pequena escala da qualidade do sinal de cada uma.

Basta clicar no nome de sua rede para que apareça a opção de digitar sua senha.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/07.png)

Tendo digitado corretamente a senha, além da confirmação no canto superior direito, vemos que o ícone mudou:

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/08.png)

Apenas em casos extremamente específicos, o TigerOS não detectará sua placa de rede cabeada, mas existem umas poucas placas wireless que são chatas para funcionar, ou mesmo não funcionarão.
O alerta aqui é: se a placa wireless não funcionar, mas é possível usar por cabo, você deve ponderar se ainda assim vale a pena instalar o TigerOS.

Agora iremos instalar o TigerOS na partição criada anteriormente.
Caso não queira fazer dual boot, mas usar apenas o TigerOS, 99% dos passos são os mesmos.

No canto superior direito, só clicar na opção Instalar o TigerOS.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/09.png)

Eis que o instalar abre no idioma português, mas com uma lista de diversos outros.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/10.png)
Clique então em continuar.

Em layout do teclado, o padrão mais comum do Brasil já é pré-selecionado, mas caso sua máquina venha com teclado americano, basta dar uma pesquisada na lista do lado esquerdo.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/11.png)

Por garantia, teste a acentuação nesse campo aqui, principalmente a questão da ç.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/12.png)
Só clicar em clicar em Continuar.

Em instalação de outros softwares, deixarei desmarcado aqui a opção de atualizar enquanto instala, para mostrar os alertas que o sistema faz.
> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/13.png)

Mas destaco que é importante selecionar a segunda opção, para garantir que a placa de vídeo e wifi funcionem corretamente, mesmo que a internet já tenha sido testada e funcione.
Agora só clicar em continuar.
Parte importantíssima, pois é aqui que confirmaremos todos os detalhes para a instalação do TigerOS.
Selecione a opção Avançada e clique em continuar.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/14.png)

Selecione esse espaço livre, criado anteriormente, de 30gb, dando duplo clique nele.
As 3 primeiras opções podem ser deixadas como estão, mas a opção Usar como, deve ser alterada de Ext4, para BTRFS.
E em ponto de montagem, selecione essa /
Clique em Ok para confirmar as configurações.
Só clicar em Instalar agora
É solicitada a confirmação da instalação, bastando clicar em continuar.
Agora é perguntado sobre a região em que a pessoa se encontra, com relação ao fuso horário.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/15.png)

Embora eu more em Curitiba, selecione a região de SP e clique em continuar.
Então configurarei meu usuário, colocando meu nome, o nome do computador para ser localizado, caso esteja numa rede local, além do nome do meu usuário.

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/16.png)

Destaco o fato de não poder usar letras maiúsculas ou números no nome do usuário.
Sugiro que escolha uma senha caprichada para cadastrar. Você não conseguirá avançar daqui sem ter escolhido uma senha, como acontece no Windows.
Recomendo selecionar a opção de Solicitar minha senha para entrar, mesmo que não haja nenhum problema de outras pessoas também acessarem essa máquina, mesmo sem sua presença.

Só clicar em continuar e aguardar o procedimento. 

> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/boot%2Binstall/17.png)
