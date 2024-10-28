# Guia com mais de 500 comandos do Linux (Explicados)

![Imagem1](https://github.com/user-attachments/assets/6f4de205-c54d-47df-a803-fcae7861d59b)

Por: [Bruno Andrade](https://www.linkedin.com/in/brunobredaandrade/) (GNU/Linux - Brasil)

## Introdução

Neste documento, irá encontrar mais de 500 comandos via terminal do Linux. Todos bem explicados da forma como funcionam e o que executam. Totalmente em português, com uma linguagem simples e objetiva que pode ser compreendida por todos os usuários (desde o nível mais simples ao avançado).

Esta é uma oportunidade de não usar somente a interface gráfica para executar os comandos, e sim ter o domínio do terminal. Aumentando ainda mais o seu conhecimento no universo Linux. Afinal, em certos momentos, precisamos de um conhecimento a mais para executarmos determinadas tarefas.

O Linux já está presente nas grandes empresas, e dominá-lo significa um diferencial a mais com relação a outros colaboradores da empresa. 

Mesmo com a prática diária, é improvável que guarde todos os comandos do terminal, porém a ideia desta lista é trazer os comandos primordiais para o terminal Linux, pois sua lista é vasta.

Esta apostila é de distribuição gratuita e pode ser compartilhada e baixada por qualquer pessoa, afinal o objetivo principal é sua divulgação e distribuição, sem qualquer fim lucrativo.

Útil para iniciantes; curiosos; de nível intermediário procurando se aprofundar e para quem já é avançado e deseja relembrar algum dos comandos.

Porém, antes de executarem os comandos no terminal, lembrem-se da famosa frase do modo root: _"Com grandes poderes, vem grandes responsabilidades"_ - Stan Lee

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

### 5. Bibliografia

### 6. Redes sociais

## 1.	Guia de referência – Lista de comandos para Linux

### 1.1 Conhecendo a hierarquia do sistema

![Imagem1](https://github.com/user-attachments/assets/825aae89-966e-4806-9b0a-15e2f737dc32)

## 1.2 Atalhos globais

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




