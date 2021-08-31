# Guia de instalação do Tiger0S

O Tiger0S vem na forma de uma imagem ISO (um arquivo .iso) que pode ser usado para criar um DVD inicializável ou um dispositivo USB inicializável.

Este guia irá ajudá-lo a baixar a imagem ISO, criar uma mídia inicializável e instalar o Tiger0S no seu computador.

## Baixar ISO

Para se fazer o download da ISO do TigerOS, o procedimento é bem simples, bastando acessar o site oficial ou a sessão de downloads do canal de cursos:

Em ambos os canais, temos uma versão única do sistema, para 64 bits, não oferecendo dificuldades na hora da escolha. Para quem quer saber mais do sistema, como requisitos de hardware, basta conferir as informações nesta sessão.

Temos aqui o botão de Download que, como diz o nome, lhe permitirá baixar a ISO oficial do sistema.


Essa é a tela do gDrive:
Clique agora no botão azul parta confirmar o download.


Agora faremos a gravação de um live-pendrive para procedermos com a instalação. Para isso precisaremos de 1 pendrive de 4gb ou mais, preferencialmente, que não tenha nenhum arquivo ou que tenha sido feito backup.

Existem diversos programas para realizar o procedimento, porém, destacarei aqui o Rufus. Como alternativa, temos também o Ventoy e o...

Acesse esse site para baixarmos o Rufus, programa que fará o processo de gravação da ISO no pendrive.

Você pode mudar o site, e por tabela, o programa para nosso idioma clicando nessa parte no canto superior direito.

Terminado o download, duplo clique no programa, que estando aberto, selecione seu pendrive nesse campo aqui.

Em disco ou imagem ISO, vá até a pasta em que salvou o arquivo e selecione-o.

Em esquema de partição, se sua máquina tem 6 anos ou mais, selecione GPT, mas se for mais antiga, a opção MBR deve funcionar.
Em sistema de arquivos é possível escolher entre Fat32 ou NTFS, mas a sugestão automática costuma funcionar normalmente.

Então basta clicar em iniciar.

No w10, clicando sobre a barra de tarefas, procure pela opção Gerenciamento de disco, que abre esse programa.

Temos aqui algumas opções de particionamento já feitos para essa instalação do Windows, que pode ser diferente da sua máquina.

Mas vamos nos atentar aqui ao disco C:
Clicando com o botão direito do mouse, selecione a opção Diminuir volume.

Dependendo do tamanho do seu HD e também da quantidade de arquivos e programas já instalados, você pode considerar deixar aí uns 30 gb ou mais para o TigerOS.

Uma conta rápida: 1024 x 30gb = 30720, o tamanho exato da partição.
Sim, vc pode colocar 30.000 ou outro valor.

Na terceira opção: diminuir o espaço em MB: digite o valor de 30720.

Clique então em Diminuir.

Agora aguarde o processo de redimensionamento ser efetuado, o que pode ser demorado em sua máquina.

Pelos poderes do Kdenlive, aqui ficou pronto.

Veja que agora temos uma nova partição, como Não alocada, que é o local em que o TigerOS será instalado.

Clicando nessa nova partição com o botão direito, selecione a opção Novo volume simples.

Em rótulo de volume, digite TigerOS 21.

Só fechar esse programa e abrir o windows explorer para conferir se a partição já está aparecendo.

Está!

Até aqui ocorreu tudo bem, mas agora vamos olhar se o Rufus terminou o processo de criação do live Pendrive.

Também está terminado, então agora faremos uma parte bem chata, que é a configuração da BIOS.

O problema dessa parte em específico é q não existe apenas UM tipo de BIOS, ou mesmo UMA forma de acessá-la.

Na tela vc vê diversos tipos delas, sendo que a mesma marca, pode ter vários tipos de BIOS.

Uma coisa beeem chata é você conseguir descobrir como acessar essa BIOS, uma vez que não existe um padrão.
Em algumas máquinas até aparece essa informação, ainda que rapidamente na inicialização, mas outras, é na base da pesquisa na Google ou tentativa.

Em minha máquina, por ex, ao aparecer esse texto, pressionei a tecla Pause/Break, para conseguir ter certeza do que preciso fazer.

Como mostra aqui, basta teclar F2 para acessar o BIOS.

Aqui começaremos procurando pela opção de segurança, no qual será desabilitado e Secure Boot, mudando a opção Enable para Disable.

Agora encontraremos a opção de Inicialização, para podermos configurar a ordem de boot.

Na opção UEFI/Legacy Boot, certifique-se de selecionar a opção Legacy.
Em algumas BIOS a opção de colocar como automático está disponível, podendo ser a escolhida.

É verdade que o tigerOS funciona com o UEFI, mas pode ser que apresente problemas. Então, num primeiro momento, selecione Legacy ou automático.

Agora configurarei a ordem de boot, para que ele acesse o pendrive na hora que reiniciar a máquina.

De novo: o nome exato pode mudar em sua máquina, mas se vocẽ seguir a lógica, não deve ter dificuldades.

Procure por algo como Boot Priority Order.

Você está vendo algumas opções de nomes.

Aqui aparece para mim a opção USB HDD, que será colocada como primeira.
De novo: não existe uma forma única de proceder, em minha BIOS, uso as setas de + e - para alterar a ordem.

Pronto!

Agora será necessário salvar as configurações para reiniciar a máquina. Para isso, basta pressionar a tecla f10 e confirmar a gravação.

Sua máquina reinicializará pronta para acessar o pendrive e mostrar a tela de boot do TigerOS.

Caso não funcione, e isso infelizmente pode ocorrer, é possível usar as teclas de atalho para alterar a ordem de boot, usando a tecla f12 ou f11.
De novo: se não funcionar nenhuma das duas, basta pesquisar.

Pronto, essa é a tela de boas-vindas do TigerOS. acredito que a primeira opção deva funcionar normalmente, mas caso vocẽ tenha uma placa de vídeo 3d mais exótica, a segunda opção pode ser necessária.

Agora aguarde a inicialização do TigerOS 21.



## Inicializando no modo live

Inicialização do Tiger0S

## Instalação

No canto superior direito, só clicar na opção Instalar o TigerOS 21.

Eis que o instalar abre no idioma inglês, mas com uma lista de diversos outros.
Clique 1 vez em qualquer um deles e em seguida, clica na letra R.

Isso é pelo fato de o português do Brasil ser o último da letra P, então agora basta selecioná-lo e clicar em Continuar.

Em layout do teclado, o padrão mais comum do Brasil já é pré-selecionado, mas caso sua máquina venha com teclado americano, basta dar uma pesquisada na lista aqui.

Por garantia, teste a acentuação nesse campo aqui, principalmente a questão da ç.

Só clicar em clicar em Continuar.

Em instalação de outros softwares, deixarei desmarcado aqui a opção de atualizar enquanto instala, na parte final desse vídeo.

Mas destaco que é importante selecionar a segunda opção, para garantir que a placa de vídeo e wifi funcionem corretamente.

Agora só clicar em continuar.

Parte importantíssima, pois é aqui que confirmaremos todos os detalhes para a instalação do TigerOS.

Selecione a opção Avançada e clique em continuar.

Selecione esse espaço livre, criado anteriormente, de 30gb, dando duplo clique nele.

As 3 primeiras opções podem ser deixadas como estão, mas a opção Usar como, deve ser alterada de Ext4, para BTRFS.

E em ponto de montagem, selecione essa /

Clique em Ok para confirmar as configurações.

Só clicar em Instalar agora

É solicitada a confirmação da instalação, bastando clicar em continuar.

Agora é perguntado sobre a região em que a pessoa se encontra, com relação ao fuso horário.

Então configurarei meu usuário, colocando meu nome, o nome do computador para ser localizado, caso esteja numa rede local, além do nome do meu usuário.

Nessa parte aqui destaco o fato de não poder usar letras maiúsculas ou números. Os detalhes aparecem aqui em vermelho.

Sugiro que escolha uma senha caprichada para cadastrar. Você não conseguirá avançar daqui sem ter escolhido uma senha, como acontece no Windows.

Aqui a recomendação é a de selecionar a opção de Solicitar minha senha para entrar, mesmo que não haja nenhum problema de outras pessoas também acessarem essa máquina, mesmo sem sua presença.

Só clicar em continuar e aguardar o procedimento. 

Aqui o tempo varia muito de um computador para outro, mas deve ser algo em torno de 20 mins.

Está pronto!

Como sugerido, basta clicar em Reiniciar agora.

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
