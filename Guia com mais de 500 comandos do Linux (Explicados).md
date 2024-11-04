# Guia com mais de 500 comandos do Linux (Explicados)

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

## Sumário

### Introdução

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

## 5. Bibliografia

## 6. Redes sociais

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

**`cal 10 2016`*
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
> _Exibe o tipo MIME de **`file1`**, como **`text/plain`** ou **`image/jpeg`*._

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

* **pwck**
** Verifica a sintaxe correta ‘/ etc/passwd’ arquivo formato e a existência de usuários.

* **grpck**
**Verifica a sintaxe correta e formato do arquivo ‘/ etc/grupo’ e a existência de grupos.

* newgrp group_name:
** Registra um novo grupo para alterar o grupo padrão dos arquivos recém-criados.




































