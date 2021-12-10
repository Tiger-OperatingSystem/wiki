# Guia de instalação do Tiger0S

O TigerOS é disponibilizado ao público na forma de uma [imagem ISO](https://pt.wikipedia.org/wiki/Imagem_ISO), que deve ser gravada em um Pendrive ou ainda, DVD. Essa imagem ISO funciona de 2 formas: Live e Instalação.

## Modo Live 

Nesse modo você pode rodar todo o TigerOS de maneira funcional e sem precisar instalar, podendo testar se todo o hardware está funcionando.
O modo Live também permite que se acesse um HD com Windows e se recupere arquivos.

## Modo Instalação

Nesse modo que é acionado através do modo live ciclando no ícone de instalação na área de trabalho:

<!-- Adicionar imagem do modo indicando como iniciar a instalação a partir do live aqui -->

Nesse modo o Tiger OS é efetivamente instalado no computador

# Processo de instalação

### 1. Baixando o Tiger OS

No momento atual, o TigerOS possui apenas uma versão, a Enterprise Desktop, que pode ser [baixada através desse link](link pra baixar o Tiger OS)

### 2. Criando um pendrive para o modo live

> Nota: Para criar um Live Pendrive, é necessário um programa específico chamado Ventoy. Nesse caso, usaremos o Ventoy, mas existem outros, como Rufus.
> O download pode ser feito [a partir desse link](https://github.com/ventoy/Ventoy/releases/latest)
> 
> Basta clicar na opção para Windows e iniciar o download.
> 
> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/01.png)
> Não se preocupe se os números não forem os mesmo quando você entrar nessa página.
> 
> Quando concluir o processo de download, vá para a pasta na qual o arquivo foi salvo e descompacte-o
> 
> ![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/02.png)

#### Passo 1 - O dispositivo USB
Caso seu pendrive já não esteja conectado a uma porta USB, faça-o agora.

> **Nota:** tenha em mente que o dispositivo USB será formatado durante o processo, lembre-se de fazer backup de arquivos importantes

#### Passo 2 - Iniciando o Ventoy

Dentro da pasta do Ventoy para Windows, existe outra ainda com o nome e a versão do programa.  Clique em Ventoy2Disk.
Veja que em device (1), aparece detalhes sobre meu pendrive, inclusive o tamanho dele

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/03.PNG)

> Clique em Install, note que esse processo ira apagar todos os dados no dispositivo USB (pendrive)

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/04.PNG)

Terminado o processo, que deve demorar menos de 1 minuto, a seguinte mensagem aparecerá:

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/05.PNG)

Isso significa que a partir de agora, seu dispositivo agora é um _**live pendrive**_ estando apto a receber o TigerOS. Você pode fechar a janela agora

#### Passo 3 - Adicionando o Tiger OS ao pendrive

Vá até a pasta que salvou a ISO do TigerOS e, clicando com o botão direito, selecione copiar.

Agora, na barra da esquerda, procure por Ventoy e cole o arquivo dentro do live pendrive.

![Processo de cópia da ISO](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/07.png)


Essa mensagem informa que o pendrive deve ser removido e qualquer tecla pressionada para prosseguir com a reinicialização.

Agora vemos a tela de dual boot, que permite escolher se inicializará pelo TigerOS ou w10.

Vemos que aqui mostra o nome de usuário cadastrado durante o processo de instalação, agora basta digitar a senha e clicar em Iniciar sessão.

Pronto, TigerOS 21 instalado e funcionando!

No canto inferior direito, temos a opção de configurar a Internet. Basta clicar com o botão esquerdo mesmo do mouse e escolher qual a sua rede, digitar a senha e pronto.

Mas aqui vemos que, além do painel de boas-vindas, também temos outra informação, sobre atualizações de segurança do sistema.

As informações sobre atualização em sua máquina deverão ser diferentes dessa imagem, mas não se preocupe com isso, basta clicar em Ok.

Solicitada a senha de admin, que é aquela cadastrada na instalação, basta digitá-la.

Aqui você vê tudo que será atualizado, bastando confirmar e aguardar.



## Pós-instalação

Drivers de hardware
Codecs Multimídia
Suporte a idiomas
Snapshots do Sistema

## Solução de problemas

Opções de Boot

## Dúvidas frequentes

Inicialização múltipla (Multi-boot)
Particionando
Pre-instalando o Tiger0S 
Onde encontrar ajuda
