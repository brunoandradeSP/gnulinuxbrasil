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
>_Lista de diretórios._

**`ls -al`**
>_Lista de diretórios com exibição de arquivos ocultos._

**`cd dir`**
> _Muda do diretório atual para o especificado (substituir a variável_ **`dir`** _pelo nome da pasta)._


