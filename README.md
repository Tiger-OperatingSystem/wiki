# Guia de instalação do Tiger0S

O TigerOS é disponibilizado ao público na forma de uma imagem ISO, que deve ser gravada em um Pendrive ou ainda, DVD. Essa imagem ISO funciona de 2 formas: Live e Instalação.

Modo Live significa que você pode rodar todo o TigerOS de uma das 2 mídias de maneira funcional e sem precisar instalar, podendo testar se todo hardware de sua máquina está funcionando.
O modo Live também permite que se acesse um HD com Windows e se recupere arquivos.

O TigerOS possui apenas uma versão, a Enterprise Desktop, baixável logo na primeira parte do site.

Para criar um Live Pendrive, é necessário um programa específico para isso. Nesse caso, usaremos o Ventoy, mas existem outros, como Rufus.

Esse é o site para fazer o download do Ventoy

https://github.com/ventoy/Ventoy/releases

Nesta página você verá mais informações sobre o Ventoy e no final dela, embaixo de Assets, você finalmente encontrará o arquivo para download. Basta clicar na opção para Windows e iniciar o download.

!![download ventoy](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/01.png)

Não se preocupe se os números não forem os mesmo quando você entrar nessa página.

Quando concluir o processo de download, vá para a pasta na qual o arquivo foi salvo e descompacte-o

![pasta ventoy aberta](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/ventoy/02.png)

Caso seu pendrive já não esteja conectado a uma porta USB, faça-o agora.

Dentro da pasta do Ventoy para Windows, existe outra ainda com o nome e a versão do programa.  Clique em Ventoy2Disk.
Veja que em device (1), aparece detalhes sobre meu pendrive, inclusive o tamanho dele

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/03.PNG)

Antes de clicar em Install, verifique se não existem arquivos no pendrive, pois ele será formatado, como informa a imagem:

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/04.PNG)

Se estiver tudo ok com o pendrive, então clique em Install.

Terminado o processo, que deve demorar menos de 1 minuto, a seguinte mensagem aparecerá:

![Legenda flutuante](https://raw.githubusercontent.com/Tiger-OperatingSystem/wiki/main/05.PNG)

Isso significa que a partir de agora, seu dispositivo agora é um live pendrive estando apto a receber o TigerOS ou o Windows.

Depois de clicar em OK e fechar o Ventoy, vá até a pasta que salvou a ISO do TigerOS e, clicando com o botão direito, selecione copiar.

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
