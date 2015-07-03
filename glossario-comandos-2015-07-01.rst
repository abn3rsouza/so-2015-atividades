======================
Glossário de comandos
======================

:Disciplina: Fundamentos de Sistemas Operacionais
:Professor: Jurandy Soares
:Nome: Abner Souza
:Matrícula: 20121144010133
:Data: 01/07/2015

cat
 Esse comando serve para exibir um arquivo, criar um arquivo ou concatenar arquivos.
 cat [opções] arquivo ou cat arquivo = imprime na tela o conteúdo do arquivo
 cat > arquivo =  cria um arquivo recebendo o texto digitado logo após o comando. Para sair do arquivo criado utilize  Ctrl + D.
 cat arquivo1 >> arquivo2 = esse comando faz com que o arquivo2 receba o conteúdo do arquivo1. Obs.: as informações    contidas no arquivo2 são sobrescritas pelas do arquivo1. 

cd
 Muda de diretório.
 "cd /" para ir ao diretório raiz.
 "cd" para ir ao seu diretório pessoal.
 "cd .." para acessar um diretório de nível acima do atual.
 ”cd -” para voltar ao diretório que se encontrava antes de mudar. Para navegar através múltiplos níveis de diretórios em só comando, use por exemplo, "cd /var/www", que o levará diretamente ao sub-diretório /www do diretório /var. 

cowsay
 Programa de troca de mensagens a partir de animações em ASCII.
    cowsay -l = ver todas as variações de animações.
	  cowsay “mensagem” = manda a mensagem para o seu próprio terminal em configuração default, ou seja, uma vaca.
	  cowsay –f kiss “mensagem” = manda a mensagem para o seu próprio terminal em configuração kiss, ou seja, de um beijo.   Atenção: o kiss pode ser substituído pelas outras variações.
    cowsay –f kiss “mensagem” | write colega = manda a mensagem para o terminal do seu colega em configuração kiss, ou seja, de um beijo. Atenção: o kiss pode ser substituído pelas outras variações.

echo
 Mostra os argumentos na saída.
 echo /* = exibe todos os nomes de arquivos de um diretório em ordem alfabética.
 echo "$VARIAVEL" = verifica o conteúdo da variável de ambiente VARIAVEL. 

env
 Lista as variáveis de ambiente. 
  env

exit
 Sair do local atual.
 exit ou Ctrl + D


help
  Descrição do comando


HISTTIMEFORMAT="%d/%m/%y
  Descrição do comando


hostname
  nome da máquina em que vc está


ifconfig
 Permite configurar as interfaces de rede, sendo o comando utilizado na inicialização do sistema para configuração destas interfaces. Caso nenhum argumento seja passado junto ao comando, o mesmo apenas irá exibir o estado das interfaces atualmente definidas.
 ”sudo ifconfig eth0” para exibir o estado e informações da interface de rede eth0.
 ”sudo ifconfig eth1 down” para desativar a interface de rede eth1.
 ”sudo ifconfig eth1 up” para ativar a interface de rede eth1.
 ”sudo ifconfig eth0 192.168.3.1 netmask 255.255.255.0 up” para configurar a interface de rede eth0 com endereço IP 192.168.3.1 e máscara da rede 255.255.255.0, ativando-a.
 ”sudo ifconfig eth1 hw ether 00:D0:D0:67:2C:05” para alterar o endereço MAC (MAC Address) da interface de rede eth1 para “ 00:D0:D0:67:2C:05”. É necessário que a placa de rede esteja desativada “sudo ifconfig eth1 down” para esta operação.
 ”sudo ifconfig eth0:1 10.0.0.2 netmask 255.255.255.0 up” para adicionar um segundo endereço de rede, com IP 10.0.0.2 e máscara 255.255.255.0 a interface eth0. 


last
 Mostra todas informações referente as entradas (login) e saídas (logout) de usuários do sistema.
 ”last -a” para exibir estas informações mostrando o nome da maquina de onde foi efetuado os logins.
 ”last -d” para exibir estas informações mostrando o endereço IP da maquina de onde foi efetuado os logins.
 ”last reboot” para exibir um registro de todas as reinicializações efetuadas no sistema. 


lastb
  Descrição do comando


ls
 Lista arquivos e/ou diretórios; E.:
 *Comando utilizado para listar o conteúdo de um diretório. Usado com certas opções, é possível ver o tamanho dos arquivos, quando foram criados, e as permissões de cada um.
 "ls ~" para mostrar os arquivos que estão em seu diretório pessoal.
 ”ls -hal ~” para mostrar os arquivos que estão em seu diretório pessoal, inclusive os ocultos (-a) em forma de uma listagem (-l) e com as informações de tamanho mais amigável a nós seres humanos (-h). 
  
  
mv
 Este comando move arquivos e diretórios, sendo muito usado também para renomear um determinado arquivo. 


mkdir
 Criar diretório; Ex.: mkdir -p /var/www/html/so/.antigo/${USER}/; Ex.: mKdir fusca;
 Comando cuja finalidade é permitir a criação de um ou mais diretórios.
       "mkdir musicas" para criar um diretório chamado “musicas” dentro do diretório corrente. 
 nome="fulano


passswd
 Altera a senha de um usuário exibindo um prompt para que a nova senha seja fornecida, e logo depois repetida para confirmação. O usuário logado pode alterar a própria senha digitando apenas ”passwd”. 


pwd
 O comando pwd lhe permite saber em qual diretório você está no momento, onde pwd significa "print working directory".
  Executando "pwd" no diretório Desktop mostrará "~/Desktop". Observe que o Terminal do Gnome também mostra esta        informação na barra de títulos da janela. Veja a imagem de exemplo no topo desta página. 


set
  Descrição do comando


tree
  Descrição do comando


tty
  Descrição do comando


vim
  Descrição do comando


wait
  Descrição do comando


wall
  Descrição do comando


which
  Descrição do comando


while
  Descrição do comando


who
 Semelhante ao comando w mostra quais usuários estão logados no sistema.
 ”who -m” para mostrar o nome do usuário logado no sistema.
 ”who -q” para mostrar a quantidade total e nomes dos usuário conectados ao sistema. 


whoami
  Este comando fornece o mesmo resultado do comando ”who -m”.


    write
        Descrição do comando
        
        
    Dicas e Truques

        Teclas de controle e atalhos
        Ctrl + f
	 Move o cursor uma palavra para frente
        Ctrl + b
	 Move o cursor uma palavra para trás
        Ctrl + a
	 Para ir ao início da linha de comando
        Ctrl + e
	 Para ir ao final da linha de comando
        Ctrl + t
	 Inverte o caractere sob o cursor com o anterior
        Ctrl + u
	 Limpa a linha de comando corrente
        Ctrl + y
	 Re-insere o último trecho de comando apagado
        Ctrl + r
	 Faz uma busca incremental no histórico de comandos utilizados
        Ctrl + c
	 Termina a execução do comando corrente
        Ctrl + d
	 Encerra entrada de dados pelo teclado fazendo logout
        Ctrl + m
	 Equivalente a tecla Enter
        Ctrl + l
	 Limpa a tela, equivalente ao comando clear
        Ctrl + s
	 Inibe a exibição de informações na tela de saída
       Ctrl + q
	Ativa a exibição de informações na tela de saída, inibida pelo Ctrl + s
       Ctrl + z
	Põe o processo corrente em background (segundo plano) 

