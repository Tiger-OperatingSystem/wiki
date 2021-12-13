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
