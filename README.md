Requisitos do Bom Programador
=============================

Neste curso você vai aprender o que é requisito, ou melhor, pré-requisito
para qualquer pessoa que pretende ser um **Bom Programador**.
Então se você pretende aprender a programar e embarcar nessa maravilhosa
profissão, sugiro que você entenda muito bem cada tópico aqui apresentado.

# Sumário
* Introdução
* O código é um "arquivo de texto"
* O sistema de arquivos
* Os editores
  - Do presente ao passado
  - Categorizando os editores
  - Algumas observações pessoais
    - Seja mais amigo do teclado
    - O código é mais importante que o editor
* Sua rotina no shell
  - Rotinas:
  - Comandos mais usados
  - Redirecionamento de saídas padrões
  - Mais rotina
  - Mais rotinas bônus
* Seu Kit Nativo de Desenvolvimento
  - Tenha sempre seu Kit de Programação Nativa
  - Conheça o mínimo da programação nativa
  - Gerenciadores de pacotes
  - Algumas outras ferramentas muito importantes
* Shell Script
* Conclusão

# Introdução

# O código é um "arquivo de texto"

Notas:
* Eu já compilei mais de 2 milhões de programas
  - Cerca de 1 compilação/interpretação por minuto em 20 anos
*  Sua rotina precisa ser entendida e "pronto"!
   - Criar/alterar código, e chamar o compilador/interpretador
* No bloco de notas
  - Criar arquivos
  - Abrir arquivos para alterar
  - Salvar, ou descartar alterações em arquivos
  - "Salvar como..." é copiar
* O *encoding* ASCII, UTF-8 e outros

# O sistema de arquivos

Notas:
* O Explorer (Windows Explorer, Finder, Nautilus)
* Os pontos de montagem
  - No Windows, letras (C:\, D:\, etc)
  - No Unix, pontos de montagem
* Caminhos ou "paths"
  - O separador de caminhos "/" ou "\\"?
  - Hoje o Windows "meio que aceita" separadores "/"
    - Ex: cd C:\Users\erlimar\sources
    - Ex: cd C:/Users/erlimar/sources
  - Hierarquia é o segredo
* Sensível ou insensível a caso (case sensitive)?
  - Windows NÃO É case sensitive ("Arquivo.txt" é o mesmo que "arquivo.txt")
  - Unix É case sensitive ("Arquivo.txt" NÃO É o mesmo que "arquivo.txt")
* O antigo DOS e seus nomes ecurtados "MYLARG~2.TXT"
  - FreeDOS VM
  - A lógica:
    - "Meu arquivo longo 1.txt"     -> "MEUARQ~1.TXT"
    - "Meu arquivo muito longo.txt" -> "MEUARQ~2.TXT"
    - "Meu arquivo mais longao.txt" -> "MEUARQ~3.TXT"

# Os editores

## Do presente ao passado

Vamos começar mostrando uma IDE bem legal com um código completo em modo de depuração, onde exibimos
uma applicação web funcionando, e um clique no botão aciona o foco em uma linha no código que inspecionada
exibe um objeto complexo.

Ao repetir a mesma ação, porém "modificando aquente" no depurador os valores
em depuração, que ocasiona um resultado diferente na aplicação final.

Abrindo um assistente simples, podemos adiconar uma nova página que já cria uma listagem de registros,
permite a incluxão, exclusão e alteração de um dados "quase" que magicamente.

Com isso queremos mostrar que hoje utilizamos IDE's poderosas para o trabalho do dia a dia, mas
a excência de uma IDE é bem simples: Continuamos editando arquivos de código e chamando ferramentas como
compiladores e interpretadores, mas agora temos várias outras ferramentas como assistentes, analisadores
e etc. Mas são todos em torno de nosso código que ainda é a grande estrela no desenvolvimento de sofware.

Então devemos focar no básico para entendê-lo bem, e então após evoluir até o "hoje" aproveitar todo
esse potencial e facilidade para sermos mais produtivos.

Então vamos caminhar para trás na história:
```
IDE
-> Smart editor
-> GUI Editor (Native Windows Notepad, Native macOS ?, Native Linux GEdit)
-> Shell Editor (FreeDOS edit.com, Unix Nano, vi, emacs)
-> Editor de linha Ed
```

## Categorizando os editores

Notas:
* Editores não visuais (obsoletos)
* Editores visuais (oque?)
* Editores gráficos
 - Editor visual é diferente de editor gráfico
* Editores inteligentes
  - Sintaxe colorida
  - Ajuda
  - Acesso a shell
  - Atalhos de comandos
    - Build
  - Ajudantes
    - Apagar linha inteira (vim, emacs)
    - Substituir entre parênteses (vim, emacs)
    - Selecionar colunas (VSCode, Atom, Sublime)
  - Complemento de código
    - Vim, Emacs
    - VSCode, Atom, Sublime
  - Ajudantes avançados
    - Goto definition (VSCode, Atom, Sublime, Vim, Emacs)
    - Lint (VSCode, Atom, Sublime, Vim, Emacs)

Resumindo:
* IDE's
* Editores Inteligentes Gráficos
  - VSCode, Atom, Sublime
* Editores Inteligentes não gráficos
  - Emacs, Vim (Neovim)

## Algumas observações pessoais

Notas:
* Os editores de shell antigos estão obsoletos: Ed, edit.com
* Os editores de shell que sobreviveram: Nano, vi/vim, emacs
* Os editores de shell inteligentes: Vim e Emacs
* Porque não?
  - Notepad++, Notepad2: Porque não são multiplataforma
* Escolha um editor IDE multiplataforma
  - De preferência não dependa das IDE's
  
### Seja mais amigo do teclado

Prefira ser mais amigo do teclado ao invés do mouse.

Notas:
* Quem digita mais código? O teclado ou o mouse?
* E, o que um programador mais faz? R: Digita código
* Os problemas de pulso: Tendinite ou LER
  - O mouse força o posicionamento incorreto das mãos
  - O teclado foi feito para a posição das mãos
  - O curso de digitação e a diferença na digitação com Whatsapp
  - Eu tenho problemas no pulso com o passar dos anos
  - Isso também é saúde

Alguns links:
* https://www.techtudo.com.br/noticias/noticia/2016/12/historia-do-teclado-veja-como-este-periferico-tao-importante-foi-pensado.html
* https://www.tecmundo.com.br/produto/122002-historia-teclado-maquina-escrever-gamers-video.htm
* https://pt.wikipedia.org/wiki/Teclado_(inform%C3%A1tica)
* https://www.youtube.com/watch?v=zfMvxTmY2rQ
* https://viverdeblog.com/teclado-qwerty/
* https://www.youtube.com/watch?v=Zo4kR8Q1qWE
  
### O código é mais importante que o editor

Escolha o editor com base em seus requisitos mínimos para codificar:
- Multiplataforma (assim você pode mudar de sistema e aproveitar a experiência)
- Suporte mínimo a encoding (UTF-8)
- Sintaxe colorida

Ou seja, um editor inteligente já é o suficiente.

# Sua rotina no shell

Notas:
* Tipos de shell Windows: 
  - Prompt de Comandos, CMD (padrão)
  - Powershell
* Tipos de shell Unix:
  - Bourne shell: sh, ksh, bash (padrão)
  - C shell: csh, tcsh
* Shell script
  - Windows: .bat, .cmd, .ps1
  - Unix: .sh, "sem extensão"
  
## Rotinas:
* Executar programas e ver o resultado
  - Executar com "nome-programa" ou "./nome-programa"
  - Windows não usa "./"
* Parâmetros
  - única-palavra, "várias palavras", 'várias palavras'
* Help
  - Unix: --help, -h, man cmd
  - Windows Cmd: /?
* Múltiplos comandos:
  - cmd1 && cmd2 - cmd1; cmd2
* Continuar na próxima linha:
  - ^ (circunflexo) - \ (contra-barra) - \` (crase)

## Comandos mais usados

UNIX           | WINDOWS
---------------|---------
echo           | echo
cd             | cd
mkdir          | mkdir
ls             | dir
cat            | type
rm, rm -d      | del, rmdir
touch file.txt | type nul > file.txt
pwd            | cd
which          | where
grep           | findstr

## Redirecionamento de saídas padrões

* Redirecionamento para arquivos
  - cmd > arquivo.txt
* Echo para saídas padrões:
  - echo Mensagem para saida padrao >&1
  - echo Mensagem para saida de erro >&2
* Redirecionamento para arquivos especiais, 1, 2, NULL
  - cmd 1> output.txt
  - cmd 2> error.txt
  - cmd 1> output.txt 2> error.txt
  - Unix: cmd >/dev/null
  - Windows CMD: cmd >nul
* Redirecionamento de um arquivo padrão para outro
  - cmd > output.txt 2>&1

## Mais rotina

* Pipes
  - ls | grep
  - dir | findstr
* Código de retorno
  - Unix: echo $?
  - Windows: echo %ERRORLEVEL%
* Variáveis de ambiente:
  - $NOME x %NOME%
  - NOME=Valor x set NOME=Valor
  - A variável $PATH, %PATH%
* Somente Unix:
  - NOME=valor command param
  
## Mais rotinas bônus
* Concatenar redirecionamento ao invés de substituir
  - cmd >> file.txt
  - echo a >> file.txt
  - echo b >> file.txt
  - echo c >> file.txt
* Redirecionamento de entrada
  - cmd < file.txt
  - findstr off < mensagens.cmd
  - type mensagens.cmd | findstr off

# Seu Kit Nativo de Desenvolvimento

Mais relacionado a entender e usar o conhecimento nessas várias ferramentas
do que ser ferramentas de programação nativa.

## Tenha sempre seu Kit de Programação Nativa

No Windows, o Visual Studio Build Tools
No macOS, o XCode minimal
No Linux, o build-essentials

Notas:
* Mesmo que você não vá programar nativamente precisará disso em algum momento
  - Instalação de módulos nativos do Node
  - Compilação com Rust
  - Instalação de alguns módulos Perl, Python, Ruby?
  
## Conheça o mínimo da programação nativa

Notas:
* Compilação de peças separadas
* Linkedição em programas e bibliotecas
* Bibliotecas estáticas (.lib, .a)
* Bibliotecas dinâmicas (.dll, .so)
* Máquinas Virtuais e Bytecodes
  - Java VM
  - Python *.pyobj
  - JavaScript V8

## Gerenciadores de pacotes

Notas:
* De sistema:
  - Linux: apt, yum, dnf, pacman
  - FreeBSD: pkg
  - MacOS: port, brew
  - Windows: scoop, chocolatey
* De linguagens:
  - NodeJS: Npm, Yarn
  - Ruby: Gem
  - Rust: Cargo
  - Dart: Pub
  - Python: Pip
  - PHP: Compose
  - Elixir: Mix
  - Etc.

## Algumas outras ferramentas muito importantes

Notas:
* Curl, Wget, PowerShell Invoke-WebRequest
* Unzip, tar, PowerShell Expand-Archive
* ./configure && make
* Git

## Shell Script

Notas:
* Arquivo de execução de comandos em lote
  - Windows Batch Script (https://en.wikibooks.org/wiki/Windows_Batch_Scripting)
  - Unix batch com `. file`, `source file`
* Arquivos executáveis
  - Permissão de execução? (Windows não tem, Unix `chmod`)
  - Shabang `#!` (https://pt.wikipedia.org/wiki/Shebang)
* O básico de entrada e saída com arquivos
  - Arquivos de texto
  - STDIN, STDOUT, STDERR
* O básico de CGI
  - Com shell script é claro
  - Com um `.exe` em C (antigão?)
  - Com um `.exe` em Go (moderninho?)
  - CGI não é antigo, é uma **forma** de fazer algo
  - O novo Fast-CGI
  - O mederno Proxy Reverso
* As primeiras linguagens de script
  - Um Shell Script mais poderoso
  - Perl e Python

# Conclusão

Você precisa conhecer todos os itens e mencionados aqui porque esse vai ser seu dia-a-dia.
Você precisa entender muito bem muitos dos itens mencionados aqui porque sua vida como desenvolvedor dependerá desse entendimento.
Você precisa praticar muito para ser bom em em alguns dos itens mencionados aqui.

1) O código é um arquivo de texto sempre;
2) Você precisa conhecer e saber navegar em todo seu sistema de arquivos;
3) Escolha logo seu editor, ele será seu melhor amigo junto ao teclado;
4) Deixa de preguiça e aprenda logo a ser fluido no shell;
5) Entenda o mínimo das peças da programação nativa, isso é útil pra tudo;
6) Use gerenciadores de pacotes, eles são melhores;
7) Se acostume logo com as ferramentas comuns do nosso meio;

Não falamos de uma série de coisas aqui como:
- Virtualização e Containers
- Padrões de Projeto
- Implantação, GitHub, Nuvem
- Segurança, Criptografia, OAuth, Bitcoin
- Performance, Aplicativos, IoT
- BigData, Inteligência artificial, Automação

E mais um "monte" de coisas ainda.
Só que tudo isso são tecnologias que surgem o tempo todo, uma substitui a outra;
outras sobrevivem mais tempo, algumas estão na moda e são muito faladas, e existem até
aquelas que parecem mais ficcão, e algumas muito complexas de se entender só com um
tutorial no YouTube.

O importante é saber que todas essas tecnologias, passam por algum momento pela mão de um programador,
e esse programador é um trabalhador que tem uma rotina diária e um conhecimento básico bem sólido,
tanto que consegue criar todas essas coisas maravilhosas que você vai aprender daqui em diante.

Por isso, esses pré-requisitos mencionados aqui precisam ser dominados por você caso queira
sobreviver na selva do desenvolvimento de softwares, ou até, se quiser ser bem sucedido em
sua carreira.
