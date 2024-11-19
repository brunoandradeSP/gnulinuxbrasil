# Guia com mais de 500 "comandos do Linux" (Explicados)

![Imagem1](https://github.com/user-attachments/assets/6f4de205-c54d-47df-a803-fcae7861d59b)

Por: [Bruno Andrade](https://www.linkedin.com/in/brunobredaandrade/) (GNU/Linux - Brasil)

## Introdução

Neste documento, você encontrará mais de 500 comandos via terminal do Linux, todos bem explicados, detalhando como funcionam e o que executam. Está totalmente em português, com uma linguagem simples e objetiva, que pode ser compreendida por todos os usuários, desde os níveis mais simples até os mais avançados.

Esta é uma oportunidade para não usar somente a interface gráfica para executar os comandos, mas sim para dominar o terminal, aumentando ainda mais o seu conhecimento no universo Linux. Afinal, em certos momentos, precisamos de um conhecimento a mais para executarmos determinadas tarefas.

O Linux já está presente nas grandes empresas, e dominá-lo significa ter um diferencial em relação a outros colaboradores da empresa.

Mesmo com a prática diária, é improvável que você guarde todos os comandos do terminal; porém, a ideia desta lista é trazer os comandos primordiais para o terminal Linux, pois sua quantidade é vasta.

Esta apostila é de distribuição gratuita e pode ser compartilhada e baixada por qualquer pessoa, pois o objetivo principal é sua divulgação e distribuição, sem qualquer fim lucrativo.

É útil para iniciantes, curiosos, pessoas de nível intermediário que procuram se aprofundar e para quem já é avançado e deseja relembrar algum dos comandos.

Porém, antes de executarem os comandos no terminal, lembrem-se da famosa frase do modo root: _"Com grandes poderes, vêm grandes responsabilidades"_ - Stan Lee.

## Disclaimer

Se você é novo no mundo do Linux, saiba que o Linux não é um sistema operacional; ele é um kernel. No entanto, costumamos chamar o “Linux” de sistema operacional para simplificar as coisas.

Quando você usa comandos no Linux, o que você realmente está fazendo é escrever instruções em uma linha de comando que serão interpretadas por um shell (como o Bash, Zsh, etc.). O shell então interpreta esses comandos e, com base neles, executa programas ou scripts específicos.

Portanto, o processo envolve três partes principais:

* **Shell:** Ele interpreta a linha de comando que você insere.
* **Linha de comando**: Esse é o conjunto de instruções que você digita, que podem incluir comandos e argumentos.
* **Programas executados:** São os aplicativos ou scripts que realizam as tarefas solicitadas.

A linha de comando, por exemplo, `ls -la /home`, é interpretada pelo shell, que então chama o programa `ls` com as opções e argumentos especificados `(-la /home)` e exibe o resultado.

## Sumário

### Introdução

### Disclaimer

### 1. Guia de referência – Lista de comandos para Linux
  ### 1.1 Conhecendo a hierarquia do sistema
  ### 1.2 Atalhos globais
  
### 2. Dicas úteis para o aprendizado

### 3. Lista de comandos

### 4. Guia de referência completo – Comandos avançados do terminal Linux
  ### 4.1. Informações do sistema Linux
  ### 4.2. Desligar (Reinicialização do sistema ou logout)
  ### 4.3. Arquivos e diretórios
  ### 4.4. Encontrar arquivos
  ### 4.5. Trabalhando com sistema de arquivos
  ### 4.6. Espaço em disco
  ### 4.7. Usuários e grupos
  ### 4.8. Permissões de arquivos (+ = Adiciona e - = Remove permissões)
  ### 4.9. Atributos especiais de arquivo: (+ = Adiciona e - = Remove permissões)
  ### 4.10. Arquivos e arquivos compactados
  ### 4.11. Pacotes RPM (Red Hat, Fedora e derivados)
  ### 4.12. Pacotes YUM Updater (Red Hat, Fedora e derivados)
  ### 4.13. Pacotes DEB (Debian, Ubuntu e derivados)
  ### 4.14. Atualizador de pacotes APT (Debian, Ubuntu e derivados)
  ### 4.15. Exibir o conteúdo de um arquivo
  ### 4.16. Manipulação de texto
  ### 4.17. Estabelecer o formato de conversão de arquivos
  ### 4.18. Análise de sistemas de arquivos
  ### 4.19. Formatar sistemas de arquivos
  ### 4.20. Backups
  ### 4.21. CD-ROM
  ### 4.22. Redes (LAN e Wi-Fi)
  ### 4.23. Redes Microsoft Windows (SAMBA)
  ### 4.24. Firewall (iptables)
  ### 4.25. Monitoramento e depuração
  ### 4.26. Dicas e comandos úteis

### 5. Bibliografia

### 6. Redes sociais

## 1.	Guia de referência – Lista de comandos para Linux

### 1.1 Conhecendo a hierarquia do sistema

![Imagem1](https://github.com/user-attachments/assets/825aae89-966e-4806-9b0a-15e2f737dc32)

### 1.2 Atalhos globais

**`Ctrl+C`**
> Cancela o comando atual em funcionamento

**`Ctrl+Z`**
> Pausa o comando atual, retorna com "fg" em primeiro plano Linux ou "bg" em segundo plano.

**`Ctrl+D`**
> Faz o logout da sessão atual (similar ao comando "exit").

**`Ctrl+W`**
> Apaga uma palavra na linha atual.

**`Ctrl+U`**
> Apaga a linha inteira.

**`Ctrl+R`**
> Tecle para Exiber um comando recente.

**`!!`**
> Repete o último comando.

**`exit`**
> Faz o logout da sessão atual

## 2.	Dicas úteis para o aprendizado

1. **Digite qualquer comando seguido de `–-help` (Dois traços e a palavra _help_)** para ver a uma descrição detalhada do comando.
(EX: `wget –help`)

2. Outra forma de conseguir documentação oficial dos comandos Linux é o comando `man` (manual), _Digite `man` seguido do nome do comando_ que você precisa de informação.
(EX: `man wget`)

3. Se por algum motivo você preferir guardar as informações do `man` (manual) de algum comando em um pendrive ou smartphone em PDF para estudos complementares utilize este comando.
(EX: **`man -t wget | ps2pdf – wget.pdf`**)

## 3. Lista de comandos

**`ls`**
> _Lista de diretórios._

**`ls -al`**
> _Lista de diretórios com exibição de arquivos ocultos._

**`cd dir`**
> _Muda do diretório atual para o especificado (substituir a variável_ **`dir`** _pelo nome da pasta)._

**`cd`**
> _Muda para o diretório /home (arquivos pessoais)._

**`Pwd`**
> _Exibe o caminho do diretório atual._

**`mkdir dir*`**
> _Cria um diretório especificado (substituir a variável_ **`dir`** _pelo nome da pasta)._

**`rm arq`**
> _Apaga o arquivo especificado (substituir a variável_ **`arq`** _pelo nome do arquivo que se quer excluir)._

**`rm -r dir`**
> _Apaga o diretório especificado (substituir a variável_ **`dir`** _pelo nome da pasta)._

**`rm -f arq`**
> _Apaga o arquivo especificado forçadamente (_ **`-f`** _de force) (substituir a variável_ **`arq`** _pelo nome do arquivo que se quer excluir)._

**`rm -rf dir`**
> _Apaga o diretório especificado forçadamente (substituir a variável_ **`dir`** _pelo nome da pasta)._
> **Utilize esse comando com extrema atenção!**

**`cp -r arq1 arq2`**
> _Copia o **“arquivo1”** para o **“arquivo2”** (substituir a variável_ **`arq`** _pelo nome do arquivo)._

**`cp -r dir1 dir2`**
> _Copia o “diretório1” para o **“diretório2”**; cria o **“diretório2”** caso não exista (substituir a variável_ **`dir`** _pelo nome do diretório)._

**`mv arq1 arq2`**
> _Dupla função: Pode ser usado para renomear ou mover o **“arquivo1”** para **“arquivo2”**. Se o arquivo2 for um diretório existente, move **“arquivo1”** para dentro do diretório **“arquivo2”** (substituir a variável_ **`arq`** _pelo nome do arquivo)._

**`ln -s arq link`**
> _Cria um link (atalho) simbólico para o arquivo (substituir a variável_ **`arq`** _pelo nome do arquivo e_ **`link`** _pelo nome que terá o atalho)._

**`touch arq`**
> _Cria ou atualiza o arquivo (substituir a variável_ **`arq`** _pelo nome do arquivo)._

**`cat > arq`**
> _Direciona a entrada padrão para um arquivo (substituir a variável_ **`arq`** _pelo nome do arquivo)._

**`more arq`**
> _Exibe o conteúdo de um arquivo (substituir a variável_ **`arq`** _pelo nome do arquivo)._

**`head arq`**
> _Exibe as primeiras 10 linhas de um arquivo (substituir a variável_ **`arq`** _pelo nome do arquivo)._

**`tail arq`**
> _Exibe as últimas 10 linhas de um arquivo (substituir a variável_ **`arq`** _pelo nome do arquivo)._

**`tail -f arq`**
> _Exibe o conteúdo de um arquivo enquanto ele é atualizado (aumenta de tamanho), iniciando com as últimas 10 linhas (substituir a variável_ **`arq`** _pelo nome do arquivo)._

**`ps`**
> _Exibe os processos dos usuários ativos em tempo real._

**`top`**
> _Exibe todos os processos rodando em tempo real._

**`kill pid`**
> _Mata um processo específico pelo número ID (substituir_ **`pid`** _pelo número do processo)._

**`killall proc`**
> _Mata todos os processos com o nome especificado em **“proc”** (substituir_ **`proc`** _pelo nome do processo)._

**`bg`**
> _Lista trabalhos parados, em segundo plano ou pode continuá-los também._

**`fg`**
> _Traz o trabalho mais recente para o primeiro plano_

**`fg trab`**
> _Traz o trabalho **“trab”** para o primeiro plano (substituir_ **`trab`** _pelo nome do processo)._

**`chmod octal arq`**
> _Muda as permissões do arquivo **“arq”** para os valores especificados em octal, que podem ser atribuídos separadamente para **“usuário”**, **“grupo”** e **“outros”**. Os valores em octal são representados da seguinte forma:_
> * _4 - leitura (r, de_ read);
> * _2 - gravação (w, de_ write);
> * _1 - execução (x, de_ execute).
>
> **Explanação:** _Para definir as permissões, somam-se os valores acima. Por exemplo, para atribuir ao dono do arquivo (**“usuário”**) acesso total de leitura (r), gravação (w) e execução (x), basta somar o valor octal 4 + 2 + 1 = 7. Se você deseja permitir apenas leitura e gravação para membros do **“grupo”**, soma-se 4 + 2 = 6. Para aplicar ambos os exemplos, use `chmod 760`, onde o usuário tem permissão total (rwx), o grupo tem leitura e gravação (**rw-**) e outros não têm nenhuma permissão (**`0`**)._
>
> **Outros exemplos:**
>
> * **`chmod 777`**
> > _leitura (r), gravação (w) e execução (x) para todos (**“usuário”**, **“grupo”** e **“outros”**)._
> * **`chmod 755`**
> > _leitura (r), gravação (w) e execução (x) para o **“usuário”** **(dono)**, e leitura e execução **(r-x)** para **“grupo”** e **“outros”**._
>
> Para mais informações, digite no terminal: **`man chmod`**

**`ssh usuário@host`**
> _Conecta ao host como usuário (exemplo: **`ssh gnulinuxbrasil@meuservidor`**)._

**`ssh -p porta usuário@host`**
> _Conecta ao host na porta especificada (substituir **`porta`** pelo número da porta configurada)._

**`ssh-copy-id usuário@host`**
> _Adiciona a sua chave para o host e usuário daquele host; serve para ativar logins sem senha com uso de chaves._

**`grep sequência arquivos`**
> _Pesquisa pela sequência nos arquivos (substituir a **`sequência e arquivos`** pelos valores correspondentes à pesquisa)._

**`grep -r sequência dir`**
> _Pesquisa pela sequência nos arquivos (substituir a **`sequência e arquivos`** pelos valores correspondentes à pesquisa)._

**`grep -r sequência dir`**
> _Pesquisa recursivamente pela **`sequência`** LinuxLinuxLinux no diretório **`dir`**_

**`comando | grep sequência`**
> _Pesquisa pela sequência na saída do comando (substituir **`comando`** e **`sequência`** de acordo com os valores a serem buscados)._

**`locate arq`**
> _Encontra todas as instâncias de um arquivo (substituir a variável **`arq`** pelo nome do arquivo)._

**`date`**
> _Exibe a data e hora atual._

**`cal`**
> _Exibe um calendário do mês atual._

**`uptime`**
> _Exibe o tempo de atividade do sistema._

**`w`**
> _Exibe quem está online._

**`whoami`**
> _Exibe como quem você está logado._

**`finger`**
> _Exibe informações do usuário._

**`uname -a`**
> _Exibe informações do kernel._

**`cat /porc/cpuinfo`**
> _Exibe informações da CPU._

**`cat /proc/meminfo`**
> _Exibe informações da memória._

**`man comando`**
> _Abre o manual do comando especificado (substituir a variável **`comando`** pelo nome do comando que se quer conhecer)._

**`df`**
> _Exibe o uso do disco_

**`du`**
> _Exibe o uso do espaço em um diretório._

**`free`**
> _Exibe o uso da memória e swap._

**`whereis aplicação`**
> _Exibe possíveis localizações do aplicativo (substituir **`aplicação`** pelo nome do programa)._

**`which aplicação`**
> _Exibe que a aplicação irá rodar por omissão (substituir **`aplicação`** pelo nome do programa)._

**`tar cf pacote.tar arqs`**
> _Cria um pacote TAR (nomeado **`pacote.tar`**) com os arquivos especificados (substituir a variável **`arqs`** pelo nome do arquivo)._

**`tar xf pacote.tar`**
> _Extrai os arquivos de **“pacote.tar”** (substituir a variável **`pacote.tar`** pelo nome do arquivo)._

**`tar czf pacote.tar.gz arqs`**
> _Cria um pacote TAR (nomeado **`pacote.tar.gz`**) com compressão GZip._

**`tar xzf pacote.tar.gz`**
> _Extrai um pacote TAR (nomeado **`pacote.tar.gz`**) com compressão GZip._

**`tar cjf pacote.tar.bz2`**
> _Cria um pacote TAR (nomeado **`pacote.tar.bz2`**) com compressão BZip2._

**`tar xjf pacote.tar.bz2`**
> _Extrai um pacote TAR (nomeado **`pacote.tar.gz`**) com compressão BZip2._

**`gzip arq`**
> _Compacta um arquivo e o renomeia para arq.gz (substituir a variável **`arq`** pelo nome do arquivo)._

**`gzip -d arq.gz`**
> _Descompacta arq.gz para um arquivo (substituir a variável **`arq.gz`** pelo nome do arquivo)._

**`ping host`**
> _Envia um pacote ICMP (ping) para o host e Exibe o resultado (substituir a variável **`host`** pelo domínio de um site ou o número IP)._

**`whois domínio`**
> _Retorna informações sobre o domínio (substituir a variável **`domínio`** pelo endereço de um site ou o número IP)._

**`dig host`**
> _Retorna informações de DNS para o domínio (substituir a variável **`host`** pelo domínio de um site ou o número IP)._

**`ListAllCommands | grep searchstr`**
> _Instalação a partir do código fonte; os comandos devem ser digitados na sequência em um terminal, um de cada vez._

**`dig -x host`**
> _Exibe o retorno reverso para um host (substituir a variável **`host`** pelo domínio de um site ou o número IP)._

**`wget arq`**
> _Faz o download do arquivo **“arq”** (substituir a variável **`arq pelo`** endereço online do arquivo)._

**`wget -c arq`**
> _Continua o download interrompido de um arquivo **“arq”** (substituir a variável **`arq`** pelo endereço online do arquivo)._

**Comandos de instaladores**

* ./configure
* make
* make install

**`dpkg -i pacote.deb`**
> _Instala um pacote DEB (distros Debian) (substituir a variável **`pacote.deb`** pelo nome do pacote de programa)._

**`rpm -Uvh pacote.rpm`**
> _Instala um pacote RPM (Distros que utilizam RPM) (substituir a variável **`pacote.rpm`** pelo nome do pacote de programa)._

## 4. Guia de referência completo – Comandos avançados do terminal Linux

### 4.1. Informações do sistema Linux

**`arch`**
> _Exibe a arquitetura da máquina (1)._

**`uname -m`**
> _Exibe a arquitetura da máquina (2)._

**`uname -r`**
> _Exibe versão do kernel usada._

**`dmidecode -q`**
> _Exibe os componentes do sistema (hardware)._

**`hdparm -i /dev/hda`**
> _Exibe as características de um disco rígido._

**`hdparm -tT /dev/das`**
> _Executa teste de leitura em um disco rígido._

**`cat /proc/cpuinfo`**
> _Exibe informações da CPU._

**`cat /proc/interrupts`**
> _Exibe interrupções._

**`cat /proc/meminfo`**
> _Verifica a utilização de memória._

**`cat /proc/swaps:df -h`**
> _Exibe o tamanho dos arquivos e diretórios ordenados por tamanho._

**`ls -lSr |more`**
> _Estima o espaço usado pelo diretório **‘dir1’**._

**`du -sh dir1`**
> _Exibe o tamanho dos arquivos e diretórios ordenados por tamanho._

**`du -sk * | sort -rn`**
> _Exibe o espaço usado por pacotes .rpm instalados e organizados pelo tamanho (Fedora, Red Hat e outros)._

**`rpm -q -a –qf ‘%10{SIZE}t%{NAME}n’ | sort -k1,1n`**
> _Exibe o espaço usado por pacotes instalados, organizado pelo tamanho (Debian, Ubuntu e outros)._

**`dpkg-query -W -f=’${Installed-Size;10}t${Package}n’ | sort -k1,1n`**
> _Exibe arquivos de swap._

**`cat /proc/version`**
_Exibe a versão do kernel._

**`cat /proc/net/dev`**
> _Exibe estatísticas e adaptadores de rede._

**`cat /proc/mounts`**
> _Exibe o sistema de arquivos montado._

**`lspci -tv`**
> _Exibe os dispositivos PCI._

**`lsusb -tv`**
> _Exibe os dispositivos USB._

**`date`**
>  _Exibe a data do sistema._

**`cal 2024`**
> _Visualiza o calendário de 2024._

**`cal 10 2016`**
> _Exibe o calendário para o mês de outubro de 2024._

**`date 041217002016.00`**
> _Define manuelmente o mês, dia, hora, minuto, ano e opcionalmente os segundos com o formato específico **`MMDDhhmmAAAA.ss`**._

**`clock -w`**
> _Salva as alterações para a data na BIOS._

### 4.2. Desligar (Reinicialização do sistema ou logout)

**`shutdown -h now`**
> _Desliga o sistema (1)._

**`shutdown -h minutos`**
> _Desliga o sistema de acordo com o minuto selecionado (EX.: **`shutdown -h 30`** , desliga em 30 minutos)._

**`init 0`**
> _Desliga o sistema (2)._

**`telinit 0`**
> _Desliga o sistema (3)._

**`halt`**
> _Desliga o sistema (4)._

**`shutdown -r mensagem:`**
> _Para enviar uma mensagem aos usuários afetados pelo desligamento, use o comando desta forma: **`sudo shutdown -r 30 "O sistema será reiniciado em 30 minutos”`**

**`shutdown -c`**
> _Cancela um desligamento do sistema planejado._

**`shutdown -r now`**
> _Reinicia (1)._

**`reboot`**
> _Reinicia (2)._

**`logout`**
> _Fecha a sessão._

### 4.3. Arquivos e diretórios

**`cd /home`**
> _Digite o diretório em **`home`**._

**`cd ..`**
> _Volta um nível._

**`cd ../..`**
> _Volta 2 níveis._

**`cd`**
> _Vai para o diretório de raíz._

**`cd ~user1`**
> _Vai para o diretório de **`user1`**._

**`cd –`**
> _Volta para o diretório anterior._

**`pwd`**
> _Exibe o caminho do diretório de trabalho._

**`ls`**
> _Consulta os arquivos em um diretório._

**`ls -F`**
> _Consulta os arquivos em um diretório._

**`ls -l`**
> _Exibe detalhes de arquivos e pastas em um diretório._

**`ls -a`**
> _Exibe arquivos ocultos._

**`ls *[0-9]*`**
> _Exibe arquivos e pastas que contêm números._

**`tree`**
> _Exibe arquivos e pastas em uma árvore a partir da raiz. (1)_

**`lstree`**
> _Exibe arquivos e pastas em uma árvore a partir da raiz. (2)_

**`mkdir dir1`**
> _Cria uma pasta ou diretório com nome **‘dir1’**._

**`mkdir dir1 dir2`**
> _Cria duas pastas ou diretórios simultaneamente (criando dois diretórios ao mesmo tempo)._

**`mkdir -p /tmp/dir1/dir2`**
> _Cria uma árvore de diretório._

**`rm -f file1`**
> _Exclui o arquivo chamado **‘file1’**._

**`rmdir dir1`**
> _Exclui a pasta chamada **‘dir1’**._

**`rm -rf dir1`**
> _Exclui uma pasta chamada **‘dir1’** com seu conteúdo forçadamente._

**`rm -rf dir1 dir2`**
> _Exclui duas pastas (diretórios) com seu conteúdo forçadamente._

**`mv dir1 new_dir`**
> _Renomeia ou move um arquivo ou pasta (diretório)._

**`cp file1`**
> _Copia um arquivo._

**`cp file1 file2`**
> _Copia os dois arquivos ao mesmo tempo._

**`cp dir /*.`**
> _Copia todos os arquivos de um diretório dentro do diretório de trabalho atual._

**`cp -a /tmp/dir1.`**
> _Copia um diretório dentro do diretório de trabalho atual._

**`cp -a dir1`**
> _Copia um diretório._

**`cp -a dir1 dir2`**
> _Faz uma cópia recursiva e preserva a estrutura e atributos dos arquivos no diretório de destino_

**`ln -s file1 lnk1`**
> _Cria um link simbólico para o arquivo ou diretório._

**`ln file1 lnk1`**
> _Cria um vínculo físico para o arquivo ou diretório._

**`touch -t 0712250000 file1`**
> _Modifica as datas de acesso e modificação do arquivo **`file1`** para a data e hora especificadas._

**`file file1`**
> _Exibe o tipo e informações do arquivo **`file1`** na tela._

**`file -i file1`**
> _Exibe o tipo MIME de **`file1`**, como **`text/plain`** ou **`image/jpeg`**._

**`iconv -l`**
> _Listas de cifras conhecidas._

**`iconv -f fromEncoding -t toEncoding inputFile > outputFile`**
> _Cria uma nova forma de arquivo de entrada assumindo que está codificado em fromEncoding e converte para ToEncoding._

**`find . -maxdepth 1 -name *.jpg -print -exec convert ”{}” -resize 80×60 “thumbs/{}” \;`**
> _Agrupa arquivos dimensionados no diretório atual e os envia aos diretórios de visualização em miniaturas (requer o conversor do ImagemagicK)._

### 4.4. Encontrar arquivos

**`find / -name file1`**
> _Busca de um arquivo ou diretório da raiz do sistema._

**`find / -user user1`**
> _Encontra arquivos e diretórios pertencentes ao usuário **‘user1’**._

**`find /home/user1 -name \*.bin`**
> _Procura arquivos com extensão **‘. bin’** no diretório **‘/ home/user1’**._

**`find /usr/bin -type f -atime +100`**
> _Pesquisa arquivos binários não utilizados nos últimos 100 dias._

**`find /usr/bin -type f -mtime -10`**
> _Pesquisa arquivos criados ou alterados nos últimos 10 dias._

**`find / -name \*.rpm -exec chmod 755 ‘{}’ \;`**
> _Procura arquivos com extensão **‘. rpm’** e modifica permissões._

**`find / -xdev -name \*.rpm`**
> _Procura arquivos com extensão **‘. rpm’** ignorando a mídia removível, como CD-ROM, pen-drive, etc…_

**`locate \*.ps`**
> _Encontra arquivos com a extensão **‘. ps’** primeiramente executado com o comando **“updatedb”**._

**`whereis halt`**
> _Exibe a localização de um arquivo binário, a ajuda ou a fonte. Neste caso ele pergunta onde está o comando **‘halt’**._

**`which halt`**
> _Exibe o caminho completo para o executável do comando **`halt`**, se estiver no PATH do usuário._

### 4.5. Trabalhando com sistema de arquivos

**`mount /dev/hda2 /mnt/hda2`**
> _Monta um disco chamado `hda2`. Primeiro, verifique a existência do diretório **`‘/ mnt/hda2’`*; Se você não possuir, você deve criá-lo._

**`umount /dev/hda2`**
> _Remove um disco chamado `hda2`. Em primeiro lugar, do ponto de **`‘ / mnt/hda2`**._

**`fuser -km /mnt/hda2`**
> _Força a remoção quando o dispositivo está ocupado._

**`umount -n /mnt/hda2`**
> _Executa a remoção sem ler o arquivo/etc/MTAB. Útil quando o arquivo é somente leitura ou o disco rígido está cheio._

**`mount /dev/fd0 /mnt/floppy`**
> _Monta um disco flexível (disquete)._

**`mount /dev/cdrom /mnt/cdrom`**
> _Monta um cdrom / dvdrom._

**`mount /dev/hdc /mnt/cdrecorder`**
> _Monta um cd gravável ou um dvdrom._

**`mount /dev/hdb /mnt/cdrecorder`**
> _Monta um cd gravável / dvdrom (um dvd)._

**`mount -o loop file.iso /mnt/cdrom`**
> _Monta um arquivo ou uma imagem iso._

**`mount -t vfat /dev/hda5 /mnt/hda5`**
> _Monta um sistema de comandos em arquivos FAT32._

**`mount /dev/sda1 /mnt/usbdisk`**
> _Monta uma memória ou um pen-drive USB (sem especificar o tipo de sistema de arquivos)._

### 4.6. Espaço em disco

**`df -h`**
> _Exibe o tamanho dos arquivos e diretórios ordenados por tamanho._

**`ls -lSr |more`**
> _Estima o espaço usado pelo diretório **‘dir1’**._

**`du -sh dir1`**
> _Exibe o tamanho dos arquivos e diretórios ordenados por tamanho._

**`du -sk * | sort -rn`**
> _Exibe o espaço usado por pacotes .rpm instalados, organizados pelo tamanho (Fedora, Red Hat e outros)._

**`rpm -q -a –qf ‘%10{SIZE}t%{NAME}n’ | sort -k1,1n`**
> _Exibe o espaço usado por pacotes instalados e organizados pelo tamanho (Debian, Ubuntu e outros)._

**`dpkg-query -W -f=’${Installed-Size;10}t${Package}n’ | sort -k1,1n > g`**
> _Exibe uma lista de todos os pacotes instalados e seus respectivos tamanhos (em KB) em ordem crescente de espaço ocupado, no Debian e derivados, e salva o resultado no arquivo `g`_

### 4.7. Usuários e grupos

**`groupadd nome_do_grupo`**
> _Cria um novo grupo._

**`groupdel nome_do_grupo`**
> _Exclui um grupo._

**`groupmod -n novo_nome_do_grupo viejo_nome_do_novo_grupo`**
> _Renomeia um grupo._

**`useradd -c “Name Surname ” -g admin -d /home/user1 -s /bin/bash user1`**
> _Cria um novo usuário *“admin”* do grupo._

**`useradd user1`**
> _Cria um novo usuário._

**`userdel -r user1`**
> _Exclui um usuário (`‘-r’` elimina o diretório Home)._

**`usermod -c “User FTP” -g system -d /ftp/user1 -s /bin/nologin user1`**
> _Altera os atributos do usuário._

**`passwd`**
> _Altera a senha._

**`passwd user1`**
> _Altera a senha do usuário (apenas pelo root)._

**`chage -E 2024-11-04 user1`**
> _Define um limite de tempo para a senha do usuário. Neste caso, ele diz que a chave expira em 04 de Novembro de 2024._

**Informações do sistema Linux**

* **`pwck`**
> _Verifica a sintaxe correta **‘/ etc/passwd’** arquivo formato e a existência de usuários._

* **`grpck`**
> _Verifica a sintaxe correta e formato do arquivo **‘/ etc/grupo’** e a existência de grupos._

* **`newgrp group_name:`**
> _Registra um novo grupo para alterar o grupo padrão dos arquivos recém-criados._

### 4.8. Permissões de arquivos (+ = Adiciona e - = Remove permissões)

**`ls -lh`**
> _Exibe permissões._

**`ls /tmp | pr -T5 -W$COLUMNS`**
> _Divide o terminal em 5 colunas._

**`chmod ugo+rwx directory1`**
> _Define permissões de leitura (r), gravação (w) e execução (x) para o dono (u), grupo (g) e outros (o) no diretório **‘directory1’**._

**`chmod go-rwx directory1`**
> _Remove as permissões de leitura (r), gravação (w) e execução (x) do grupo (g) e dos outros (o) no diretório **‘directory1’**._

**`chown user1 file1`**
> _Altera o proprietário de um arquivo._

**`chown -R user1 directory1`**
> _Altera o proprietário de um diretório e todos os arquivos e diretórios contidos dentro._

**`chgrp group1 file1`**
> _Altera o grupo de **‘file1’**._

**`chown user1:Grupo1 user1`**
> _Altera o dono (usuário) para **‘user1’** e o grupo para **‘Grupo1’** no arquivo ou diretório **‘user1’**._

**`find / -perm -u+s`**
> _Ver todos os arquivos com sistema SUID configurado._

**`chmod u+s /bin/file1`**
> _Define o bit SUID em um arquivo binário. O usuário que está executando esse arquivo adquire os mesmos privilégios como proprietário._

**`chmod u-s /bin/file1`**
> _Desabilita o bit SUID em um arquivo binário._

**`chmod g+s /home/public`**
> _Define o SGID bit em um diretório – semelhante ao SUID, mas para o diretório._

**`chmod g-s /home/public`**
> _Desativa o bit SGID em um diretório._

**`chmod o+t /home/public`**
> _Conjunto STIKY bit em um diretório. Permite a exclusão de arquivos somente para os legítimos proprietários._

**`chmod o-t /home/public`**
> _Desativa STIKY bit em um diretório._

### 4.9. Atributos especiais de arquivo: (+ = Adiciona e - = Remove permissões)

**`chattr +a file1`**
> _Define o atributo "append-only" (somente acrescentar) no arquivo **‘file1’**._

**`chattr +c file1`**
> Define o atributo de compressão no arquivo **‘file1’**, permitindo que ele seja compactado e descompactado automaticamente._

**`chattr +d file1`**
> _Define o atributo **"no dump"** no arquivo **‘file1’**, instruindo programas de backup a ignorarem esse arquivo._

**`chattr +i file1`**
> _Torna o arquivo inalterado, portanto não pode ser excluído, alterado, renomeado ou vinculado._

**`chattr +s file1`**
> _Permite que um arquivo possa ser excluído com segurança._

**`chattr +S file1`**
> _Define o atributo de **"síncrono"** no arquivo **‘file1’**, garantindo que, sempre que o arquivo for modificado, as alterações sejam imediatamente gravadas no disco de forma síncrona._

**`chattr +u file1`**
> _Define o atributo **"undelete"** no arquivo **‘file1’**, permitindo que o conteúdo do arquivo seja recuperado caso ele seja excluído._

**`lsattr`**
> _Exibe atributos especiais._

### 4.10. Arquivos e arquivos compactados

**`bunzip2 file1.bz2`**
> _Descompacta um arquivo chamado **‘file1.bz2’**._

**`bzip2 file1`**
> _Comprime um arquivo chamado **‘file1’**._

**`gunzip file1.gz`**
> _Descompacta um arquivo chamado **‘file1.gz’**._

**`gzip file1`**
> _Comprime um arquivo chamado **‘file1’**._

**`gzip -9 file1`**
> _Comprime com compressão máxima._

**`rar a file1.rar test_file`**
> _Cria um arquivo com o rar chamado **‘file1.rar’**._

**`rar a file1.rar file1 file2 dir1`**
> _Comprime **‘arquivo1’**, **‘arquivo2’** e **‘dir1’* simultaneamente._

**`rar x file1.rar`**
> _Descompacta o arquivo rar._

**`unrar x file1.rar`**
> _Descompacta o arquivo rar._

**`tar -cvf archive.tar file1`**
> _Cria um tarball descompactado._

**`tar -cvf archive.tar file1 file2 dir1`**
> _Cria um arquivo contendo **‘arquivo1’**, **‘file2’** e **‘dir1’**._

**`tar -tf archive.tar`**
> _Exibi o conteúdo de um arquivo._

**`tar -xvf archive.tar`**
> _Extrai um arquivo tar._

**`tar -xvf archive.tar -C /tmp`**
> _Extrai um tarball em / tmp._

**`tar -cvfj archive.tar.bz2 dir1`**
> _Cria um arquivo tar compactado no bzip2._

**`tar -xvfj archive.tar.bz2`**
> _Descompacta um arquivo compactado do bzip2 tar_

**`tar -cvfz archive.tar.gz dir1`**
> _Cria um arquivo tar compactado em gzip._

**`tar -xvfz archive.tar.gz`**
> _Descompacta um arquivo tar do gzip compactado._

**`zip file1.zip file1`**
> _Cria um arquivo compactado zip._

**`zip -r file1.zip file1 file2 dir1`**
> _Compressão .zip de vários arquivos e diretórios simultaneamente._

**`unzip file1.zip`**
> _Descompacta um arquivo zip._

### 4.11. Pacotes RPM (Red Hat, Fedora e derivados)

**`rpm -ivh package.rpm`**
> _Instala um pacote rpm._

**`rpm -ivh –nodeeps package.rpm`**
> _Instala um pacote rpm e ignora solicitações de dependências._

**`rpm -U package.rpm`**
> _Atualiza um pacote rpm sem alterar a configuração dos arquivos._

**`rpm -F package.rpm`**
> _Atualiza um pacote rpm somente se ele **“Comandos”** estiver instalado._

**`rpm -e package_name.rpm`**
> _Remove um pacote rpm._

**`rpm -qa`**
> _Exibe todos os pacotes rpm instalados no sistema._

**`rpm -qa | grep httpd`**
> _Exibe todos os rpm de pacotes com o nome **“httpd”**._

**`rpm -qi package_name`**
> _Informações sobre um pacote específico instalado._

**`rpm -qg “System Environment/Daemons”`**
> _Exibe um grupo software pacotes rpm._

**`rpm -ql package_name`**
> _Exibe lista de arquivos fornecidos por um pacote rpm instalado._

**`rpm -qc package_name`**
> _Exibe a lista de arquivos, dada por uma configuração de pacote rpm instalado._

**`rpm -q package_name –whatrequires`**
> _Exibe lista de dependências que são solicitados para um pacote rpm._

**`rpm -q package_name –whatprovides`**
> _Exibe a capacidade fornecida por um pacote rpm._

**`rpm -q package_name –scripts`**
> _Exibe scripts começados durante a remoção da instalação._

**`rpm -q package_name –changelog`**
> _Exibe o histórico das revisões de um pacote rpm._

**`rpm -qf /etc/httpd/conf/httpd.conf`**
> _Verifica qual pacote rpm pertence a um determinado arquivo._

**`rpm -qp package.rpm -l`**
> _Exibe a lista de arquivos fornecidos por um rpm do pacote que ainda não foi instalado._

**`rpm –import /media/cdrom/RPM-GPG-KEY`**
> _Importa a assinatura digital chave pública._

**`rpm –checksig package.rpm`**
> _Verifica a integridade de um pacote rpm._

**`rpm -qa gpg-pubkey`**
> _Verifica a integridade de todos os pacotes rpm instalados._

**`rpm -V package_name`**
> _Verifica o tamanho do arquivo, licenças, tipos, proprietário, grupo, exame de integridade, resumo de MD5 e última modificação._

**`rpm -Va`**
> _Verifica todos os pacotes rpm instalados no sistema. Use com cuidado._

**`rpm -Vp package.rpm`**
> _Verifica se um pacote instalado ainda não é rpm._

**`rpm2cpio package.rpm | cpio –extract –make-directories *bin*`**
> _Extrai o arquivo executável de um pacote rpm._

**`rpm -ivh /usr/src/redhat/RPMS/arch/package.rpm`**
> _Instala um pacote construído a partir de um rpm fonte._

**`rpmbuild –rebuild package_name.src.rpm`**
> _Constrói um pacote rpm a partir de um rpm fonte._

### 4.12. Pacotes YUM Updater (Red Hat, Fedora e derivados)

**`yum install package_name`**
> _Baixa e instala um pacote rpm._

**`yum localinstall package_name.rpm`**
> _Irá instalar um RPM e vai tentar resolver todas as dependências para você, usando seus repositórios._

**`yum update package_name.rpm`**
> _Atualiza todos os pacotes rpm instalados no sistema._

**`yum update package_name`**
> _Upgrade / atualiza um pacote rpm._

**`yum remove package_name`**
> _Remove um pacote rpm._

**`yum list`**
> _Lista todos os pacotes instalados no sistema._

**`yum search package_name`**
> _Encontra um pacote no repositório rpm._

**`yum clean packages`**
> _Limpa um cache de rpm, apagando os pacotes baixados._

**`yum clean headers`**
> _Exclui todo o cabeçalho de arquivos que o sistema usa para resolver a dependência._

**`yum clean all`**
> _Remove os arquivos de cache e o cabeçalho do pacote._

### 4.13. Pacotes DEB (Debian, Ubuntu e derivados)

**`dpkg -i package.deb’`**
> _Instala / atualiza um pacote deb._

**`dpkg -r package_name`**
> _Remove um deb para o pacote do sistema._

**`dpkg -l`**
> _Exibe todos os pacotes deb instalados no sistema._

**`dpkg -l | grep httpd`**
> _Exibe todos os pacotes deb com o nome **“httpd”**._

**`dpkg -s package_name`**
> _Informações sobre um pacote específico instalado no seu sistema._

**`dpkg -L package_name`**
> _Exibe lista de arquivos fornecidos por um pacote instalado no sistema._

**`dpkg –contents package.deb`**
> _Exibe uma lista de arquivos fornecidos por um pacote não instalado ainda._

**`dpkg -S /bin/ping`**
> _Verifica qual pacote pertence um determinado arquivo._

### 4.14. Atualizador de pacotes APT (Debian, Ubuntu e derivados)

**`apt-get install package_name`**
> _Instala / atualiza um pacote deb._

**`apt-cdrom install package_name`**
> _Instala / atualiza um pacote deb do cdrom._

**`apt-get update`**
> _Atualiza a lista de pacotes._

**`apt-get upgrade`**
> _Atualiza todos os pacotes instalados._

**`apt-get remove package_name`**
> _Remove a instalação de um pacote deb do sistema._

**`apt-get purge program_name`**
> _Remove a instalação de um programa do sistema._

**`apt-get check`**
> _Verifica se as resoluções das dependências estão corretas._

**`apt-get clean`**
> _Limpa o cache de pacotes baixados._

**`apt-cache search searched-package`**
> _Retorna a lista de pacotes que corresponde à série **‘pacotes’**._

### 4.15. Exibir o conteúdo de um arquivo

**`cat file1`**
> _Exibe o conteúdo de um arquivo a partir da primeira linha._

**`tac file1`**
> _Exibe o conteúdo de um arquivo a partir da última linha._

**`more file1`**
> _Exibe o conteúdo ao longo de um arquivo._

**`less file1`**
> _Semelhante o comando **‘more’** mas permite que você salve o arquivo, bem como o movimento para trás._

**`head -2 file1`**
> _Exibe as duas primeiras linhas de um arquivo._

**`tail -2 file1`**
> _Exibe as duas últimas linhas de um arquivo._

**`tail -f /var/log/messages`**
> _Exibe em tempo real o que foi adicionado ao arquivo._

### 4.16. Manipulação de texto

**`cat file1 file2 .. | command <> file1_in.txt_or_file1_out.txt`**
> _Sintaxe geral para a manipulação de texto usando o tubo, STDIN e STDOUT._

**`cat file1 | command( sed, grep, awk, grep, etc…) > result.txt`**
> _Sintaxe geral para manipular um texto de um arquivo e escrever os resultados para um novo arquivo._

**`cat file1 | command( sed, grep, awk, grep, etc…) » result.txt`**
> _Sintaxe geral para manipular um texto de um arquivo e adicionar o resultado em um arquivo existente._

**`grep Nov /var/log/messages`**
> _Procura as palavras **“Nov”** no arquivo **‘/ var/log/messages’**._

**`grep ^Nov /var/log/messages`**
> _Procura palavras que começam com **“Novembro”** no arquivo **‘/ var/log/messages’**._

**`grep [0-9] /var/log/messages`**
> _Seleciona todas as linhas no arquivo **‘/ var/log/messages’** que contêm números._

**`grep Nov -R /var/log/*`**
> _Encontra a sequência de caracteres **“Nov”** no diretório **‘ / var/log ’** e abaixo._

**`sed ‘s/stringa1/stringa2/g’ example.txt`**
> _Realoca **“string1”** com **“string2”** em ‘**example.txt’**_

**`sed ‘/^$/d’ example.txt`**
> _Remove todas as linhas em branco do **‘example.txt’**_

**`sed ‘/ *#/d; /^$/d’ example.txt`**
> _Exclui comentários e linhas em branco de **‘example.txt’**._

**`sed -e ‘1d’ result.txt`**
> _Elimina a primeira linha do arquivo **‘result.txt’**_

**`sed -n ‘/string1/p’`**
> _Exibi somente as linhas que contêm a palavra **“string1”**._

### 4.17. Estabelecer o formato de conversão de arquivos

**`dos2unix filedos.txt fileunix.txt`**
> _Converte um formato de arquivo de texto do MSDOS para UNIX._

**`unix2dos fileunix.txt filedos.txt`**
> _Converte um formato de arquivo de texto do UNIX para MSDOS._

**`recode ..HTML < page.txt > page.html`**
> _Converte um arquivo de texto para html._

**`recode -l | more`**
> _Exibe todas as conversões de formato disponíveis._

### 4.18. Análise de sistemas de arquivos

**`badblocks -v /dev/hda1`**
> _Verifica os blocos defeituosos no disco hda1._

**`fsck /dev/hda1`**
> _Repara / verificar a integridade do arquivo do sistema Linux no disco hda1._

**`fsck.ext2 /dev/hda1`**
> _Repara / verifica a integridade do sistema de arquivo ext2 no disco hda1._

**`e2fsck /dev/hda1`**
> _Repara / verifica a integridade do sistema de arquivo ext2 no disco hda1._

**`e2fsck -j /dev/hda1`**
> _Repara / verifica a integridade do sistema de arquivo ext3 no disco hda1._

**`fsck.ext3 /dev/hda1`**
> _Repara / verifica a integridade do sistema de arquivo ext3 no disco hda1._

**`fsck.vfat /dev/hda1`**
> _Repara / verifica integridade do arquivo sistema disco fat hda1._

**`fsck.msdos /dev/hda1`**
> _Repara / verifica a integridade de um arquivo a partir do dos no sistema de disco hda1._

**`dosfsck /dev/hda1`**
> _Repara / verifica a integridade de um arquivo a partir do dos no sistema de disco hda1._

### 4.19. Formatar sistemas de arquivos

**`mkfs /dev/hda1`**
> _Verifica os blocos defeituosos no disco hda1._

**`mke2fs /dev/hda1`**
> _Repara / verifica a integridade do arquivo do sistema Linux no disco hda1._

**`mke2fs -j /dev/hda1`**
> _Repara / verifica a integridade do sistema de arquivo ext2 no disco hda1._

**`mkfs -t vfat 32 -F /dev/hda1`**
> _Repara / verifica a integridade do sistema de arquivo ext2 no disco hda1._

**`fdformat -n /dev/fd0`**
> _Repara / verifica a integridade do sistema de arquivo ext3 no disco hda1._

**`mkswap /dev/hda3`**
> _Repara / verifica a integridade do sistema de arquivo ext3 no disco hda1._

### 4.20. Backups

**`dump -0aj -f /tmp/home0.bak /home`**
> _Faz um backup completo e salva do diretório **‘/Home’**._

**`dump -1aj -f /tmp/home0.bak /home`**
> _Faz um Backup incremental do diretório **‘ /home’**._

**`restore -if /tmp/home0.bak`**
> _Restaura um save interativamente._

**`rsync -rogpav –delete /home /tmp`**
> _Sincronização entre diretórios._

**`rsync -rogpav -e ssh –delete /home ip_address`**
> _Rsync através do túnel SSH._

**`rsync -az -e ssh –delete ip_addr`**
> _Sincroniza um diretório local com um diretório remoto via ssh e compressão._

**`rsync -az -e ssh –delete /home/local ip_addr`**
> _Sincroniza um diretório remoto em um diretório local através de ssh e compressão._

**`dd bs=1M if=/dev/hda | gzip | ssh user@ip_addr ‘dd of=hda.gz’`**
> _Faz um backup em um disco rígido de um host remoto através de ssh._

**`dd if=/dev/sda of=/tmp/file1`**
> _Salva o conteúdo de um disco rígido para um arquivo. (Neste caso o disco rígido é **“sda”** e o arquivo **“file1”**)._

**`tar -Puf backup.tar /home/user`**
> _Salva os diretórios/etc e a raiz (excluindo o conteúdo do subdiretório/root/dir1 /) em um arquivo compactado, cujo nome inclui a data e hora atual._

**`( cd /tmp/local/ && tar c . ) | ssh -C user@ip_addr ‘cd /home/share/ && tar x -p’`**
> _Copia o conteúdo de um diretório em um diretório remoto através de ssh._

**`( tar c /home ) | ssh -C user@ip_addr ‘cd /home/backup-home && tar x -p’`**
> _Copia um diretório local em um diretório remoto através de ssh._

**`tar cf – . | (cd /tmp/backup ; tar xf – )`**
> _Copia o local preservando as licenças e links de um diretório para outro._

**`find /home/user1 -name ‘*.txt’ | xargs cp -av –target-directory=/home/backup/ –parents`**
> _Encontra e copia todos os arquivos com extensão **‘.txt’** de um diretório para outro_

**`find /var/log -name ‘*.log’ | tar cv –files-from=- | bzip2 > log.tar.bz2`**
> _Encontra todos os arquivos com extensão **‘. log’** e fazer um arquivo bzip._

**`dd if=/dev/hda of=/dev/fd0 bs=512 count=1`**
> _Faz uma cópia do MRB (Master Boot Record) para um disquete._

**`dd if=/dev/fd0 of=/dev/hda bs=512 count=1`**
> _Restaura a cópia da (MBR Master Boot Record) gravada no disquete._

### 4.21. CD-ROM

**`cdrecord -v gracetime=2 dev=/dev/cdrom -eject blank=fast -force`**
> _Limpa ou apaga um cd regravável (CD-RW)_

**`mkisofs /dev/cdrom > cd.iso`**
> _Cria uma imagem .iso do CD-ROM no disco._

**`mkisofs /dev/cdrom | gzip > cd_iso.gz`**
> _Cria uma imagem iso compactada do CD-ROM no disco._

**`mkisofs -J -allow-leading-dots -R -V “Label CD” -iso-level 4 -o ./cd.iso data_cd`**
> _Cria uma imagem .iso de um diretório._

**`cdrecord -v dev=/dev/cdrom cd.iso`**
> _Grava uma imagem iso._

**`gzip -dc cd_iso.gz | cdrecord dev=/dev/cdrom –`**
> _Grava uma imagem iso comprimida._

**`mount -o loop cd.iso /mnt/iso`**
> _Monta uma imagem iso._

**`cd-paranoia -B`**
> _Tira músicas de um cd para arquivos wav._

**`cd-paranoia – ”-3”`**
> _Pegua as 3 primeiras músicas de um cd para arquivos wav._

**`cdrecord –scanbus`**
> _Faz a varredura de buffer para identificar o canal scsi._

**`dd if=/dev/hdc | md5sum`**
> _Executa um md5sum em um dispositivo, como um CD._

### 4.22. Redes (LAN e Wi-Fi)

**`ifconfig eth0`**
> _Exibe a configuração de uma placa de rede Ethernet._

**`ifup eth0`**
> _Ativa uma interface **‘eth0’**._

**`ifdown eth0`**
> _Desabilita uma interface **‘eth0’**._

**`ifconfig eth0 192.168.0.1 netmask 255.255.255.0`**
> _Configura um endereço IP._

**`ifconfig eth0 promisc`**
> _Configura **‘eth0’** modo comum para obter pacotes (sniffing)._

**`dhclient eth0`**
> _Ativa a interface **‘eth0’** em modo dhcp._

**`route -n`**
> _Exibe tabela de rota._

**`route add -net 0/0 gw IP_Gateway`**
> _Configura a entrada padrão._

**`route add -net 192.168.0.0 netmask 255.255.0.0 gw 192.168.1.1`**
> _Configura uma rota estática para encontrar a rede, ‘192.168.0.0/16’._

**`route del 0/0 gw IP_gateway`**
> _Remove a rota estática._

**`echo “1” > /proc/sys/net/ipv4/ip_forward`**
> _Ativa o IP de rota._

**`hostname`**
> _Exibe o nome do host do sistema._

**`host www.example.com`**
> _Encontra o nome do host para resolver o nome de um IP (1)._

**`nslookup www.example.com`**
> _Encontra o nome do host para resolver o nome de um IP e vice-versa (2)._

**`ip link show`**
> _Exibe o status de todas as interfaces._

**`mii-tool eth0`**
> _Exibe o status de **‘eth0’** link._

**`ethtool eth0`**
> _Exibe estatísticas da placa de rede **‘eth0’**._

**`netstat -tup`**
> _Exibe todas as conexões de rede ativa e seu PID._

**`netstat -tupl`**
> _Exibe todos os ouvintes de rede de serviços sobre o sistema e seu PID._

**`tcpdump tcp port 80`**
> _Exibe todo o tráfego HTTP._

**`iwlist scan`**
> _Exibe as redes sem fio._

**`iwconfig eth1`**
> _Exibe a configuração de uma placa de rede sem fio._

**`whois www.example.com`**
> _Pesquisa Base de dados Whois._

### 4.23. Redes Microsoft Windows (SAMBA)

**`nbtscan ip_addr`**
> _Resolução de nome de rede da BIOS._

**`nmblookup -A ip_addr`**
> _Resolução de nome de rede da BIOS._

**`smbclient -L ip_addr/hostname`**
> _Visualiza compartilhamentos remotos de um host windows._

### 4.24. Firewall (iptables)

**`iptables -t filter -L`**
> _Exibe todas as correntes na tabela de filtro._

**`iptables -t nat -L`**
> _Exibe todas as correntes da tabela nat._

**`iptables -t filter -F`**
> _Limpa todas as regras da tabela de filtro._

**`iptables -t nat -F`**
> _Limpa todas as regras da tabela nat._

**`iptables -t filter -X`**
> _Exclui qualquer cadeia criados pelo usuário._

**`iptables -t filter -A INPUT -p tcp –dport telnet -j ACCEPT`**
> _Permite conexões telnet de entrar._

**`iptables -t filter -A OUTPUT -p tcp –dport http -j DROP`**
> _Bloqueia conexões HTTP de saída._

**`iptables -t filter -A FORWARD -p tcp –dport pop3 -j ACCEPT`**
> _Permite conexões POP para uma cadeia de frente._

**`iptables -t filter -A INPUT -j LOG –log-prefix “DROP INPUT”`**
> _Registra uma sequência de entrada._

**`iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE`**
> _Configura uma PAT (conversão de endereços de porta) na eth0, escondendo os pacotes de saída de coação._

### 4.25. Monitoramento e depuração

**`top`**
> _Exibe as tarefas Linux que mais utilizam a CPU._

**`ps -eafw`**
> _Exibe as tarefas do Linux._

**`ps -e -o pid,args –forest`**
> _Exibe as tarefas do Linux de forma hierárquica._

**`pstree`**
> _Exibe uma árvore de processos do sistema._

**`kill -9 ID_Processo`**
> _Força o encerramento de um processo._

**`kill -1 ID_Processo`**
> _Força um processo para recarregar a configuração._

**`lsof -p $$`**
> _Exibe uma lista de arquivos abertos por processos._

**`lsof /home/user1`**
> _Exibe uma lista de arquivos abertos em um determinado caminho do sistema._

**`strace -c ls >/dev/null`**
> _Exibe o sistema de chamadas feitas e recebidas por um processo._

**`strace -f -e open ls >/dev/null`**
> _Visualiza chamadas para a biblioteca._

**`watch -n1 ‘cat /proc/interrupts’`**
> _Exibe interrupções em tempo real._

**`last reboot`**
> Última reinicialização do sistema._

**`lsmod`**
> _Exibe o kernel carregado._

**`free -m`**
> _Exibe o status da RAM em megabytes._

**`smartctl -A /dev/hda`**
> _Monitora a confiabilidade de um disco rígido através do SMART._

**`smartctl -i /dev/hda`**
> _Verifica se o SMART está habilitado em um disco rígido._

**`tail /var/log/dmesg`**
> _Exibe os eventos inerentes no processo de carregamento do kernel._

**`tail /var/log/messages`**
> _Exibe eventos do sistema._

### 4.26. Dicas e comandos úteis

**`apropos …keyword`**
> _Exibe uma lista de comandos que pertencem às palavras-chave de um programa; são úteis quando você sabe o que faz o seu programa, mas não conhece o nome do comando._

**`man ping`**
> _Exibe as páginas de manual on-line; por exemplo, um comando ping, use a opção **‘-k’** para encontrar qualquer comando relacionado._

**`whatis …keyword`**
> _Exibe a descrição do que o programa faz._	

**`mkbootdisk –device /dev/fd0 'uname -r'`**
> _Cria um disquete bootável._

**`gpg -c file1`**
> _Codifica um arquivo com o guarda de segurança do GNU._

**`gpg file1.gpg`**
> _Decodifica um arquivo com o guarda de segurança do GNU, informações do sistema Linux U._

**`wget -r www.example.com`**
> _Baixa um site inteiro._

**`wget -c www.example.com/file.iso`**
> _Baixa um arquivo com a possibilidade de parar o download e retomar mais tarde._

**`echo ‘wget -c www.example.com/files.iso‘ | at 09`**
> _Baixa um arquivo às 09 a.m_

**`ldd /usr/bin/ssh`**
> _Exibe bibliotecas compartilhadas que são exigidas pelo programa ssh._

**`alias hh='history'`**
> _Coloque um alias para um comando **– hh** = história._

**`chsh`**
> _Muda o Shell de comando._

**`chsh –list-shells`**
> _É um comando adequado para descobrir se você tem controle remoto em outro terminal._

**`clear`**
> _Limpa a tela do terminal._

**`umcomando > archivodesaida.txt 2>&1`**
> _Executa um comando e redireciona a saída para um arquivo, combinando entre ambos STDOUT e STDERR._

**`umcomando | archivodesaida.txt 2> archivodeerros.txt`**
> _Executa um comando, você redireciona a saída (STDOUT) para um arquivo e os erros (STDERR) para outro._

**`umcomando | tee arquivodesaida.txt`**
> _Executa um comando, exibe a saída na tela e simultaneamente grava em um arquivo._

## 5. Bibliografia

* [1] [Canonical Ltda. Ubuntu, 2015](https://canonical.com/)
* [2] [Debian. Debian, 2015.](https://www.debian.org/index.pt.html)
* [3] [Fedora. Fedora, 2015.](https://www.debian.org/index.pt.html)
* [4] [OpenSuse. OpenSuse, 2015.](https://www.debian.org/index.pt.html)

## 6. Redes sociais

Participe de nossas páginas e grupos de debate:

* [Facebook](https://www.facebook.com/gnulinuxbr)
* [WhatsApp](https://chat.whatsapp.com/FqZLt9dSK685VaGfjoxwuw)
* [Telegram](https://t.me/gnulinux_brasil)
