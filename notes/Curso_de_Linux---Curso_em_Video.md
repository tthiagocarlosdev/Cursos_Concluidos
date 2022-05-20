# Curso de Linux - Curso em vídeo - 3143

[Link do curso](https://www.youtube.com/watch?v=6nN2EglOqCM&list=PLHz_AreHm4dlIXleu20uwPWFOSswqLYbV)

**Professores: Gustavo Guanabara e Ricardo Pinheiro**

## 	1. Curso de Linux - Primeiros Passos – Trailer;

## 	2. Onde o Linux pode ser usado? - Curso Linux #01;

## 	3. De onde veio o Linux? O que é software livre? - Curso Linux #02;

## 	4. Licenças e Liberdades: é importante saber - Curso Linux #03;

## 	5. Instalando Linux Mint - Curso Linux #04;

​	Acesse https://linuxmint.com/download_lmde.php escolha 64-bits e será direcionado para a próxima tela. Escolha o país **Brasil** e **Universidade Federal do Paraná.** Depois acesse o https://www.pendrivelinux.com/yumi-multiboot-usb-creator/ e baixe o **YUMI MultiBoot USB**, para criar um pendrive bootável. Você precisará de um pendrive de pequena capacidade, **4G** já é suficiente.

​	Coloque o pendrive na máquina e execute o YUMI. Em “**Select the Driver Letter of your USB Device**” escolha a unidade do pendrive que você irá utilizar. Marque a opção “**We Will Fat32 Format:**”. Em “**Select a Distribution to put on**” escolha o sistema operacional que será instalado. Marque a opção “**Show All ISOs?**”, clique em “**Browser**” e escolha a ISO do linux Mint que você baixou. Após, clique em “**Create**” e depois em “**Sim**”, pronto o seu pendrive bootável estará sendo criado. Quando terminar a instalação, clique em “**Next**”, abrirá uma caixa perguntado se você quer instalar outra ISO, clique em “**Sim**”, para instalar outra ISO, ou em “**Não**” para encerrar a instalação. Por fim, clique em “**Finish**”.

​	Após a preparação do Pendrive, coloque-o na máquina que receberá o Linux e faça o Boot pelo Pendrive. O YUMI abrirá, escolha a opção “**Linux Distribuitions**” e logo em seguida a opção “**lmde cinnamon-64-bit**” e tecle enter.

​	Após o Boot, abrirá a Interface do **Linux Mint**. No lado esquerdo na área de trabalho terá um link com o nome “**Install Linux Mint**”, execute o link. Escolha a linguagem de preferência e clique em “**Próximo**”. Escolha o Fuso horário e “**Próximo**”. Teste as teclas do seu teclado, caso esteja tudo certo, clique em “**Próximo**”, caso contrário, escolha o teclado adequado e clique em “**Próximo**”. Em “**Informações do Usuário**”, escolha a imagem do usuário, nome completo, nome do usuário, sua senha e o nome do computador, clique em “**Próximo**”.

​	Em “**Ferramenta de Instalação**” clique em “**Sim**” para formata seu computador e ser criado uma nova repartição e depois clique em “**Próximo**”. Em “**Opções avançadas**” deixe a opção “**Instalar o GRUB**” marcada e clique em “**Próximo**”. Na tela resumo. Será informado o que será feito e clique em “**Instalar**”. Após a instalação, você reinicia o computador e retira o pendrive.

## 6. Pendrive Linux com Etcher - Curso Linux #04.2;

Recuperando o Pendrive instalável:

1. Acesse a barra de pesquisa do linux Mint e digite “**Synaptic**” para acessar o “**Gerenciador de pacotes Synaptic**”;
2. Digite a senha de sua máquina e clique em autenticar para ele abrir o gerenciador;
3. Ao abrir o **Gerenciador de pacotes Synaptic** clique em “**Pesquisa**” na parte superior central da tela, e na tela “**Localizar**” que abrirár, digite “**gparted**” e clique em pesquisar;
4. Clique com o botão direito do ícone da ferramenta **gparted** e depois clique em “**marcar para instalação**” e depois na próxima tela que abrir, clique em “**marcar**”;
5. Clique no botão “**Aplicar**” no canto direito superior do programa e depois em “**Apply**”; 
6. Após a instalação do **gparted**, feche o **Gerenciador de pacotes Synaptic**;
7. Após isso, pegue o pendrive que usou para instalar o linux e plug em sua máquina e depois na barra de pesquisa do linux mint, abra o **gparted**;
8. Se aparecer a mensagem: “**The driver descriptor says physical block size is 2048 bytes, but Linux says it is 512 bytes**” apenas cancele esta mensagem;
9. No canto superior direito, selecione a unidade usb que irá recuperar;
10. Clique no menu “**Dispositivo**” e depois em “**Criar tabela de partição**”;
11. Em **Criar tabela de partição** na opção “**Selecionar novo tipo de tabela de partições**” selecione a opção “**msdos**” e clique em aplicar, pode aparecer uma mensagem de “**Erro da Libparted**”, clique em ignorar;
12. Assim que o **Gparted** terminar a sua execução, tire o pendrive da máquina e recoloque;
13. No **Gparted**, vá até o menu **GParted** e clique em “**Atualizar dispositivos**” e depois no ícone “**Criar uma nova repartição**”. Abrirá uma nova janela “**Criar nova partição**” e em “**sistema de arquivos**” selecione “**fat32**” e clique em adicionar; Depois clique em “**Aplicar todas as operações**” abrirá uma nova janela pedindo confirmação, clique em “**aplicar**”. Após o processo, clique em “**fechar**” e já está pronto.

## 7. Conhecendo o Ambiente do Linux Mint - Curso Linux #05

Na tela de “**Bem-vindo ao Linux Mint**” desative a opção no canto inferior direito “**Exibir ao iniciar**” e feche a tela.

A interface ao **Linux Mint** é bem semelhante ao do **Windows**. O menu é organizado por categoria. Já está instalado o **LibreOffice**. O **Firefox** também já vem instalado.

No canto direito inferior terá um escudo que ao colocar o cursor do mouse sobre ele irá aparecer “**Bem-vindo ao Gerenciador de Atualizações**”. Clique nele para abrir esse gerenciador. A primeira atualização irá atualizar todos os aplicativos do sistema.

## 8. Instalação básica de programas no Linux - Curso Linux #06.1

Instalando programas: Vá até o menu Mint e digite “**gerenciador de programas**” irá abrir a “loja” de aplicativos do Linux Mint.

Os programas serão separados por categoria, mas você pode procurar por programas na “**barra de pesquisa**” no canto superior direito.

Para instalar um programa, selecione o mesmo e clicando para acessá-lo. No canto superior direito terá um botão verde “**Instalar**”, clique nele coloque a senha do seu usuário e o programa será instalado.

Para baixar o **Google Chrome**, vá no navegado FireFox e acesse a página do Google. Depois pesquise por “**Google Chrome**” entre no link e terá a opção para fazer o **Download**. Ao clicar no botão “**Fazer o download**” o site já vai identificar qual é o seu sistema, leia os termos de serviço e clique no botão “**Aceitar e instalar**”.

O Firefox irá perguntar se você quer abrir  com o instalador de pacotes **Gdebian**, clique em “**OK**”. Quando abrir o instalador de pacotes, clique em “**Instalar Pacote**”. Após a instalação é só executar o programa.

## 9. Instalação avançada de programas no Linux - Curso Linux #06.2

**Instalação pelo Synaptic**:

Clique no símbolo do Mint e digite **Synaptic** para abrir o “**Gerenciador de pacotes Synaptic**”. Clique no Botão “**Pesquisa**” e digite “**chromium**”, clique com o botão direito do mouse sobre o arquivo e depois clique sobre “M**arcar para instalação**” e depois em “**Marcar**”. Depois clique em “**Aplicar**”. Uma tela de resumo com o que será feito abrirá, basta clicar no botão “**Aplique**”.

### Instalação pelo Terminal:

Abra o terminal “**Ctrl+Alt+T**” e digite os comandos:

- Para conhecer o apt:

```shell
apt
```

- Surpresa rsrsrsrs:

```shell
apt moo
```

- Para limpar a tela:

```shell
clear
```

- Para instalar o programa de monitoramento do sistema htop:

```shell
apt install htop
```

- Para abrir o programa htop:

```shell
htop
```

- Para instalar o Chromium:

```shell
apt install chromium
```

- Para remover o programa Chromium:

```shell
apt remove chromium
```

OBS.: Ele vai sugerir para remover alguns pacotes que não serão mais necessários através do seguinte comando:

```shell
sudo apt autoremove “nome do pacote”
```

### Instalação através do navegador:

Abra o navegador, pesquise por “Visual Studio Code”, acesse a página do programa, acesse o link “**Downloads**” e clique na versão do seu sistema para baixar o arquivo executável. Após baixar o arquivo, execute o mesmo para a instalação, coloque a senha do seu computador e a instalação será realizada.

### No terminal:

- Para manipular pacotes:

```shell
dpkg
```

Acesse a página onde o arquivo do pacote foi baixado/instalado e digite:

- Para remover o pacote:

```shell
sudo dpkg --remove “nome do pacote”
```

Na mesma página para instalar digite o comando:

- Para instalar o pacote:

```shell
sudo dpkg --install “nome do pacote”
```

- Para procurar por um pacote:

```shell
apt search “nome do pacote”
```

- Para limpar o cache:

```shell
sudo apt clean
```

- Para apagar pacotes que não estão sendo mais usados:

```shell
sudo apt autoremove
```

## 10. Terminal no Linux - Introdução - Curso Linux #07.1

- Comando para verificar a versão do GNU bash:

```shell
bash --version
```

- Comando para listar as pastas e arquivos do diretório em que você está:

```shell
ls
```

OBS.:

- Os comando sempre devem serem digitados em minúsculo;
- Os parâmetros modificam a forma como os comandos irão apresentar seu resultado. Os parâmetros sempre são executados com um traço e uma letra (-l) ou dois traços e uma palavra(--long). Exemplo:

- Para listar o conteúdo de um diretório apresentando mais informações sobre cada arquivo e pasta que está dentro do diretório:

```shell
ls -l
```

Resultado:

```shell
drwxr-xr-x  2 thiagocarlos thiagocarlos 4096 Jan 31 15:08 Desktop
```

**drwxr** – tipo de arquivo.

**xr-x** – permissões.

**2** – quantas pastas tem dentro do diretório.

**thiagocarlos** – usuário proprietário.

**thiagocarlos** – grupo proprietário.

**4096** – tamanho do diretório.

**Jan 31 15:08** – data da criação ou modificação do diretório.

**Desktop** – nome do diretório.

- Acessa o diretório:

```shell
cd + “nome do diretório”
```

Acessa o diretório Downloads:

```shell
cd Downloads/
```

- Para listar o conteúdo de um diretório apresentando mais informações em MEGA, GIGA sobre cada arquivo e pasta que está dentro do diretório:

```shell
ls -l -h
```

- Vai para o diretório do usuário do computador:

```shell
cd ~
```

- Mostra todos os arquivos do diretório, inclusive os ocultos:

```shell
ls -a
```

- Mostra todos os arquivos do diretório, inclusive os ocultos:

```shell
ls --all
```

**OBS.:** No Linux todo arquivo que o nome começa com ponto fica oculto.

PAREI

**$ ls -la** – Para listar o conteúdo de um diretório, inclusive os arquivos e pastas ocultos, apresentando mais informações sobre cada arquivo e pasta que está dentro do diretório.

**$ ls -lah** – Para listar o conteúdo de um diretório, inclusive os arquivos e pastas ocultos,  apresentando mais informações em MEGA, GIGA sobre cada arquivo e pasta que está dentro do diretório.



**$ cd ..** – volta para o diretório anterior.

**$ cd /** – volta para o diretório raiz do sistema.



No diretório raiz são apresentadas todas as pastas do sistema, inclusive a pasta “bin” que contém todos os comandos que são executados no programa.



**$ ls/bin** – lista todos o conteúdo da pasta bin sem acessar a pasta.



**$ cat /****proc/cpuinfo** – apresenta informações sobre o processador de forma detalhada.

**$ lscpu** – apresentar informações sobre o processador de forma mais resumida.



**$ pwd** – mostra o caminho onde está acessando no momento, o caminho absoluto.



**$ mkdir + “nome do diretório”** – cria uma pasta/diretório. Ex.:

**$ mkdir Linux** – cria uma pasta com o nome Linux.



**$ touch + “nome do arquivo.extensão”** – para criar um arquivo. Ex.:

**$ touch oi.txt** – cria um arquivo com o nome oi de extensão de texto.



**$ nano + “nome do arquivo.extensão”** - abrir o arquivo de texto por um editor no terminal. Ex.:

**$ nano oi.txt** – abre o arquivo oi.txt no nano.



1. ​	**Terminal no Linux - Manipulando diretórios - Curso Linux #07.2**

**$ ls--help** – para abrir o manual do comando ls.

**$ man ls** – para abrir o manual mais completo do comando ls.

**$ history** – mostra todo histórico de comando já digitados.

**$ ! + número da lista** – Para executar algum comando da lista. Ex.:

**$ !1068** – vai executar o comando history de acordo com a lista.

**$ mkdir -p Cursos/Hardware/Módulo\ 1/** – Comando para criar o diretório “Cursos”, dentro deste o diretório “Hardware” e dentro deste o diretório “Módulo 1”. Criação de diretório dentro de diretório. Também podemos usar o seguinte comando:

**$ mkdir -p** “**Cursos/Hardware/Módulo 2/”** - Para criar a mesma sequencia de diretórios.

**OBS.:** A diferença entre um e outro é que no primeiro comando usamos a contra barra para que o terminal entenda que estamos criando um diretório “Módulo 1”, caso contrário ele iria criar o diretório “Módulo” e o diretório “1”. No segundo comando retiramos a contra barra, mas colocamos a sequencia de diretórios que iremos criar entre aspas, e assim também será entendido que iremos criar o diretório “Módulo 2” no final.

**$ ls -R** – para listar todos os diretórios dentro do diretório o qual foi executado o comando e também listar todos os arquivos dentro de cada diretório.

Posso também encadear os parâmetros. Ex.:

**$ ls -R -l -a** – Para listar todos os diretórios e arquivos, inclusive os ocultos.

**$ ls -Rla** – também realiza a mesma função do anterior.



**$ touch Cursos/Hardware/Módulo\ 1/exercício.txt** – Este comando irá criar um arquivo chamado “exercício.txt” dentro do diretório “Módulo 1” sem precisar navegar até acessar o diretório “Módulo 1”.

**$ cat + nome do arquivo** – mostra o conteúdo do arquivo na tela do terminal. Ex.:

**$ cat exercício.txt –** mostra o conteúdo do arquivo “exercício.txt” na tela do terminal.



**$ mrdir + nome do diretório** – para apagar o diretório. Ex.:

**$ mrdir Linux/** – vai apagar o diretório “Linux/”.

OBS.: Se dentro do diretório conter arquivos que tenham conteúdo, este comando não será executado. Para isto, será preciso executar comando “rm” para apagar o arquivo e depois utilizar o “rmdir” para apagar o diretório.

**$ rm + nome do diretório + nome do arquivo** – Apaga o arquivo dentro do diretório. Ex.:

**$ rm Linux/oi.txt** – apaga o arquivo “oi.txt” dentro do diretório “Linux”.



**$ rm -rf + nome do diretório** – irá apagar todos os diretórios e arquivos que estão dentro do diretório o qual foi colocado no comando. **MUITO CUIDADO**, este comando deleta todos os diretórios e arquivos **DEFINITIVAMENTE**. Ex.:

**$ rm -rf Linux/** – apaga o diretório “Linux” e todo o seu conteúdo, sejam outros diretórios ou arquivos que tenham conteúdo.



**$ rm -i + nome do diretório** – irá apagar o diretório e seus arquivos mas irá perguntar em cada arquivo e diretório se você tem certeza de que quer apagar.

**$ rm -I + nome do diretório** – caso tenha ate três arquivos, ele apagar tudo automaticamente, caso tenha mais de três arquivos, ele irá perguntar se você tem certeza de que quer apagar tudo, caso confirmando, ele apaga.

**$ alias** – com este comando, enquanto o terminal estiver aberto, você poderá criar um padrão para comandos. Ex.:

**$ alias rm=”rm -I”** – toda vez que chamar o comando “**rm**”, ele será executado com o parâmetro “**-I**”. Se executar apenas o comando “alias”, ele mostrará quais os comandos que estão com parâmetros predefinidos.



1. ​	**Terminal Linux - Referência Global - Curso Linux #08**

**Referência Global \*, ?, [], {}**

***** é usado para referenciar todos os arquivos que estão no diretório e acrescentando um parâmetro a frente, realizará uma filtragem. Ex.:

**$ ls /****etc/\*.conf** – listará todos os arquivos que sejam de extensão “**.conf**” no diretório “**etc**”.

**$ ls /etc/\*x\*** – para listar todos os documentos que tenham a letra “x” em alguma parte do seu nome.

**$ ls /etc/****f******* – para listar todos os arquivos que iniciam com a letra “**f**”.

**$ ls /etc/?as\*** – para listar todos os arquivos que comecem com qualquer letra “**?**”, mas a segunda e terceira letra terá que ser “as” e da quarta em diante, qualquer letra.

**$ ls /etc/???a\*** – para listar todos os arquivos que tenha como quarta letra, a letra “**a**”.



**$ ls /etc/****f[a-i]\*** – para listar arquivos em que a primeira letra é  “**f**”, a segunda letra pode ser “**a**, **b**, **c**, **d**, **e**, **f**, **g**, **h**, **i**” e da terceira letra em diante, pode ser qualquer letra.

**$ ls /etc/****p[a-c,e]\*** – para listar arquivos em que a primeira letra será “**p**” a segunda pode ser de “**a**” até “**c**” e “**e**” e da terceira em diante qualquer letra.

**$ ls /etc/****p[a-c]\*** – para listar arquivos em que a primeira letra é “**p**”, a segunda será ou “**a**”, ou “**c**” e da terceira em diante qualquer letra.

**$ ls /etc/\*[a-r]\*** – para listar arquivos em que tenham como primeira letra, qualquer letra entre o intervalo de “**a**” até “**r**”.

**$ ls /etc/?****[a,e,i,o,u]******* – para listar arquivos em que a primeira letra será qualquer letra e segunda letra será vogal.

**$ ls /etc/?[a,e,i,o,u]???** – primeira letra será qualquer letra, a segunda será vogal e da terceira até a quinta será qualquer caractere. Detalhe que o nome do arquivo só terá cinco caracteres.



A referência global pode ser usada para manipular arquivos e diretórios em geral.

Chaves são usadas para fazer referência a padrões de strings e caracteres.



**$ ls /etc/?{am,ul}\*** – o primeiro caractere será qualquer letra e o segundo e terceiro será “**am**” ou “**ul**”

**$ ls /etc/\*{tab,swd}** – arquivos que terminam com “**tab**” ou “**swd**”.

**$ ls /etc/\*{tab,swd}\*** – arquivos que contenham “**tab**” ou “**swd**” em qualquer lugar do arquivo.

**$ ls /etc/\*.{conf,db}** – arquivos que sejam de extensão “**.conf**” ou “**.db**”.

1. ​	**Manipulação de Arquivos com Linux - Curso Linux #09**



**$ cat + “nome do arquivo”** – para visualizar o conteúdo do arquivo na tela.

**$ less + “nome do arquivo”** – para visualizar o arquivo de forma paginada.

**$ man + “nome do parâmetro ou comando”** – do parâmetro ou comando. O “**man**” utiliza do “**less**” para mostrar os manuais.

**$ t****ac** **+ “nome do arquivo”** – imprime o arquivo de trás para a frente.



**$ cp + nome do arquivo/diretório + nome do diretório** – para copiar o arquivo/diretório para o diretório informado. Ex.:

**$ cp aulalinux.txt Faculdade/** – para copiar o arquivo “**aulalinux.txt**” para o diretório “**Faculdade**”.



**$ rm + nome do arquivo** – para remover o arquivo. Ex.:

**$ rm aulalinux.txt** – para remover o arquivo “**aulalinux.txt**”



**$ mkdir PHP Linux Redes** – para criar três diretórios. Um “**PHP**”, um “**Linux**” e outro “**Redes**”.



**$ mv + nome do arquivo/diretório + diretório de destino** – para remover um arquivo/diretório para o diretório de destino.

**$ mv aulalinux.txt linux/** – para mover o arquivo “**aulalinux.txt**” para o diretório “**Linux**”.



**$ cp /****etc/\*.conf temporário/** – para copiar os que terminam com “**.conf**” do diretório “**etc**” par a o diretório “temporário”.



O comando “**mv**” também pode ser usado para renomear um diretório/arquivo. Basta usar o seguinte comando:

**$ mv + nome do diretório/arquivo + novo nome do arquivo/diretório**. Ex.:

**$ mv temporario/ Temp** – para renomear o diretório temporario para Temp.