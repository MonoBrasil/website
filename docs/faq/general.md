---
title: "FAQ: Geral"
redirect_from:
  - /FAQ%3A_General/
---

Perguntas Básicas
------

### O Mono pode executar binários gerados pelo Visual Studio?

Sim, o Mono pode executar os binários gerados pelo Visual Studio, sem necessidade de compilar os fontes originais.

Utilize nossa ferramenta [Mono Migration Analysis](/docs/tools+libraries/tools/moma/) para verificar se os recursos que sua aplicação utiliza foram implementados e/ou são compatíveis com o Mono, ou se existem quaisquer particularidades que necessitam de atenção.

A API atual do Mono está entre a versão .NET 4.0 e .NET 4.5; veja nosso [Roadmap](/docs/about-mono/roadmap/) para detalhes sobre o que está efetivamente implementado.

### O que o Mono™ é exatamente?

O Projeto Mono é uma iniciativa de desenvolvimento de um framework de desenvolvimento comunitário, patrocinado pela .NET Foundation e Microsoft, de uma versão livre (open source), da plataforma .NET da Microsoft. Ele tem por objetivo permitir que desenvolvedores Linux/Android/Mac OS X/iOS... possam criar e distribuir aplicações .NET cross-platform. O projeto implementa várias tecnologias desenvolvidas pela Microsoft que foram então submetidas à ECMA para padronização.

O Projeto Mono também tem despertado grande interesse no desenvolvimento de componentes derivados do C#, bibliotecas e frameworks. Dentre os mais importantes, alguns deles inclusive foram desenvolvidos pelo time do Mono, podemos citar:

-   [Gtk#](http://gtk-sharp.sf.net): uma variante do popular conjunto de ferramentas gráficas Gtk+ dos sistemas UNIX e Windows. Outras vertentes disponíveis são: Diacanvas-Sharp e MrProject.

-   [Mono.Cecil](/docs/tools+libraries/libraries/Mono.Cecil/): biblioteca para gerar e analisar assemblies CIL.

-   [#ZipLib](http://www.icsharpcode.net/OpenSource/SharpZipLib/Default.aspx): biblioteca para manipular diferentes tipo de arquivos compactados (Zip e tar).

-   [Tao Framework](/archived/tao): conector ao OpenGL.

-   Mono.Directory.LDAP / Novell.Directory.LDAP: acesso LDAP para aplicações .NET.

-   Mono.Data: suporte para banco de dados PostgreSQL, MySQL, Firebird, Sybase ASE, IBM DB2, SQLite, Microsoft SQL Server, Oracle e ODBC.

-   Mono.Cairo: variante da engine de renderização [Cairo](http://www.cairographics.org) (nosso System.Drawing utiliza esse pacote).

-   Mono.Posix / Mono.UNIX: variante para criar aplicações POSIX utilizando C#.

-   Mono.Remoting.Channels.Unix: socket UNIX para comunicação remota.

-   Mono.Security: framework com recursos avançados de segurança e criptografia.

-   Mono.Math: geração de números BigInteger e Prime.

-   Mono.Http: suporte à criação de servidores HTTP customizados e manipuladores HTTP bastante úteis para suas aplicações.

-   Mono.XML: provê suporte adicional à XML.

-   Managed.Windows.Forms (também conhecido como System.Windows.Forms): implementação de pacote (System.Drawing) completo e cross-platform, baseado na implementação Winforms.

-   [Remoting.CORBA](http://remoting-corba.sourceforge.net/): implementação CORBA para Mono.

-   Ginzu: implementação sobre o pacote Remoting da pilha [ICE](http://www.zeroc.com).

Para a lista completa, veja as páginas [Libraries](/docs/tools+libraries/libraries/) e [Software](/docs/about-mono/showcase/software/).

### Qual a diferença entre o Mono e a .NET Initiative?

A ".NET Initiative" é uma espécie de esforço corporativo da Microsoft, e parte desse projeto prevê o desenvolvimento de um framework cross-platform. O Mono é uma implementação de um framework de desenvolvimento, mas não é uma implementação de nada relativo à .NET Initiative, como por exemplo o Passport ou o Software-as-a-Service (SaaS).

### Quais tecnologias estão incluídas no Mono?

O Mono contém um conjunto de componente útil para desenvolver novas softwares:

-   Common Language Infrastructure (CLI - Infraestrutura Comum as Linguagens): Máquina virtual que contém um carregador de classes (class loader), um compilador Just-in-time, e um mecanismo de coleta de lixo (gerenciamento automátivo de memória).

-   Uma biblioteca de classes que funciona com qualquer linguagem que adota o CLR (Common Language Runtime - Executor Comun as Linguagens) como alvo. Tanto bibliotecas compatíveis com as do .NET (não todas) como bibliotecas próprias do Mono estão incluídas.

-   Um compilador da linguagem C#. Existe também um compilador de VB.NET (desatualizado) e compiladores de código aberto para outras linguagens, particularmente ativos os das linguagens F# e Boo, que são mantidos por seus respectivos projetos.

Existem diversos outros compiladores disponíveis em Windows que miram a VM padronizada do Mono/.NET para [um conjunto de linguagens:](http://msdn.microsoft.com/net/thirdparty/default.asp#lang) C++ Gerenciado, Javascript, Eiffel, APL, Cobol, Perl, Python, Scheme, Smalltalk, Standard ML, Haskell, Mercury and Oberon.

O CLR e o Common Type System (CTS - Sistema Comum de Tipos) permitem que aplicações e bibliotecas escritas em variadas linguagens interajam porque são compiladas para um mesmo byte code (código intermediário). Isto significa, por exemplo, que se você define uma classe para manipulação algébrica em C#, essa classe pode ser reutilizada em qualquer outra linguagem que suporta a CLI. Você pode criar uma classe em C#, subclassea-la em C++ gerenciado e instanciar a classe derivada em um programa em Boo. Um sistema de objetos, um sistema de linhas de execução (threading), um conjunto de bibliotecas de classes fundamentais, e um sistema de coleta de lixo são compartilhados por todas essas linguagens.

### Onde eu posso encontrar as especificações para todas essas tecnologias?

Você pode encontrar essa informação aqui:

C# [http://www.ecma-international.org/publications/standards/Ecma-334.htm](http://www.ecma-international.org/publications/standards/Ecma-334.htm)

CLI [http://www.ecma-international.org/publications/standards/Ecma-335.htm](http://www.ecma-international.org/publications/standards/Ecma-335.htm)

### Vocês irão implementar as bibliotecas das classes do SDK do .NET Framework?

Sim, nós iremos implementar as APIs das bibliotecas das classes do SDK do .NET Framework.

### Vocês irão disponibilizar um conjunto de bibliotecas de classes que sigam todas as definições do ECMA?

Eventualmente nós iremos disponibilizar. Nosso foco atual tem sido na interoperabilidade com o SDK da Microsoft, mas nós também iremos disponibilizar um conjunto de bibliotecas que sigam todas as definições do ECMA.

### Qual o significado da palavra "Mono"?

Mono significa 'macaco' em espanhol. Nós gostamos de macacos.

### O Mono está sendo utilizado atualmente?

Sem dúvida! O Mono é utilizado em muitas [aplicações comerciais e open source](/docs/about-mono/showcase/software/) e é utilizado por muitas [empresas](/docs/about-mono/showcase/companies-using-mono/) ao redor do mundo.

O ambiente de execução do Mono roda em muitas plataformas (veja a [lista detalhada](/docs/about-mono/supported-platforms/)) e o escopo do Mono é bastante compreensivo. Planos detalhados estão disponíveis abertamente na nossa página de [planos](/docs/about-mono/plans/).

Alguns softwares comerciais produzidos com o Mono estão listados [aqui](/docs/about-mono/showcase/software/).

### Quando o Mono é liberado?

Verifique o [Roadmap do Mono](/docs/about-mono/roadmap/) para maiores detalhes bem como planos de liberação das versões.

### Como eu posso contribuir com o Projeto

Verifique o [guia de como contribuir](/community/contributing/).

### Existe algum guia online sobre o Mono?

Visite a página [Monkeyguide](/archived/monkeyguide "Monkeyguide").

### Vocês não estão simplesmente copiando o projeto de alguém?

Nós buscamos oferecer as melhores ferramentas para programadores desenvolverem aplicações em Sistemas Operacionais Livres (Open Source). Nós também almejamos oferecer a interoperabilidade necessária para que esses sistemas possam interagir com outros padrões.

### O Miguel disse uma vez que o Mono foi implementado em COBOL. Isso é verdade?

Não. Isso é apenas uma piada.

### Existe alguma lista de vulnerabilidades conhecidas que afetam certas versões do Mono?

Sim. Nós compilamos uma lista de [vulnerabilidades](/docs/about-mono/vulnerabilities/) para o Mono e as ferramentas associadas à ele.

Disponibilidade
---------------

### Quais arquiteturas e sistemas operacionais o Mono suporta?

Veja nossa página de [Plataformas Suportadas](/docs/about-mono/supported-platforms/) para uma lista completa.

Embora nós suportamos uma variedade muito grande de plataformas, nós não empacotamos o Mono em sua forma binária/executável para cada uma das plataformas suportadas.

### Minha plataforma não está na lista, o Mono pode suportá-la?

Portar o Mono para uma nova plataforma envolve dois aspectos:

-   Executar o porte da arquitetura: isso significa portar o gerador de código utilizado pelo JIT para produzir código nativo para o novo processador (CPU).
-   Executar o porte do sistema operacional: isso inclui o porte da camada de I/O do Mono, que é o componente do sistema responsável por lidar com threading, I/O de arquivos e rede, assim como fazer o porte do coletor de lixo e do código que faz o tratamento das exceções, que frequentemente tende a ser específico à cada sistema operacional.

A maioria dos sistemas UNIX e seus variantes se comportam de maneira bastante similar, sendo assim, portar o Mono para um sistema UNIX diferente é relativamente simples. Portar para sistemas operacionais embarcados ou novos sistemas operacionais em desenvolvimento são provavelmente as únicas situações que requerem realmente um porte completo do Mono para um novo sistema operacional.

Portar o Mono para uma nova arquitetura exige aproximadamente três meses de trabalho.

### A Xamarin irá portar o Mono para a minha arquitetura/meu sistema operacional?

No passado, a Novell portava o Mono para novas arquiteturas e sistemas operacionais. Nós fazíamos isso devido à necessidades internas da própria Novell (x86-64, Itanium e s390, s390x com a ajuda do Neale Ferguson) ou devido à necessidades específicas de clientes (PowerPC).

A Xamarin certamente está aberta à adicionar suporte à novos arquiteturas, entretanto existem algumas variáveis envolvidas: quantidade de usuários ou nicho de mercado a ser beneficiado com esse possível porte, requisitos de hardware e subsídio adequado.

Se você deseja discutir o porte do Mono para alguma nova arquitetura, por favor, [entre em contato com a equipe de desenvolvimento do Mono na Xamarin](http://www.go-mono.com/contact/).

Problemas na Instalação
-----------------------

### Eu instalei o Mono através do instalador, mas agora alguns programas pararam de funcionar...

Quando você instala o Mono via instalador, o novo Mono irá ter prioridade em relação a qualquer outra versão mais antiga do Mono que tenha sido anteriormente instalada em seu sistema. Para exemplificar, vamos nos referir à essas duas instâncias como MonoNew e MonoSystem.

Tipicamente esse problema acontece pois os programas dependem dos assemblies instalados na memória Cache de Assembly Global (GAC - Global Assembly Cache). Isso geralmente fica localizado no diretório /usr/lib/mono/gac. O MonoNew normalmente é instalado em um diretório comum de usuário, por exemplo: /home/bob/mono-1.2.6.

Você pode solicitar que o MonoNew para alternativamente carregar assemblies do diretório do sistema, definindo a seguinte variável de ambiente:

``` bash
export MONO_GAC_PREFIX=/home/bob/mono-1.2.6:/usr
```

Observe que o primeiro diretório aponta para o GAC do MonoNew. Isso é necessário para que os novos assemblies sempre sejam carregados antes que os assemblies do MonoSystem. Se o carregador de assembly do Mono não encontrar um assembly específico no diretório do MonoNew, ele irá então carregar os assemblies contidos no diretório /usr.

O Mono e o GNOME
----------------

### Como o Mono está relacionado ao GNOME?

De várias formas. Este projeto nasceu da necessidade de oferecer ferramentas mais adequadas à comunidade GNOME, utiliza e continuará a utilizar componentes que foram e serão desenvolvidos para o projeto GNOME. A equipe do Mono trabalha ativamente no projeto [Gtk#](/GtkSharp): uma variante das bibliotecas do GNOME para .NET e Mono.

### O GNOME Foundation ou a equipe do GNOME adotaram o Mono?

O Mono é relativamente novo para ser adotado por esses grupos. Nós esperamos que as ferramentas que nós iremos oferecer sejam adotadas por desenvolvedores de software livre incluindo a equipe do GNOME Foundation e do projeto GNOME.

### Os programadores do GNOME devem adotar o Mono?

Sim, nós acreditamos que o Mono é uma grande plataforma de desenvolvimento na criação de aplicações para o GNOME desktop. O Mono inclui o [Gtk#](/docs/gui/gtksharp/), que é uma variante .NET do GTK+ e várias outras bibliotecas GNOME que, juntamente com o C# e as Bibliotecas de Sistema, oferecem aos desenvolvedores grandes vantagens em termos de produtividade na criação de aplicações gráficas, especialmente se comparadas com o GTK+ ou o Java Swing.

### O Mono será compatível com componentes Bonobo? Como é o relacionamento entre o Mono e o Bonobo?

Embora nós tivéssemos planos de suportar o Bonobo, nós ainda não havíamos iniciado nenhum trabalho nesse sentido e isso não é mais uma prioridade para nós.

### O Mono depende do GNOME?

Não, o Mono não depende do GNOME. Nós utilizamos alguns pacotes gerados pela equipe do GNOME, como a biblioteca 'glib', assim como também utilizamos bibliotecas open source de outras entidades, como o Cairo e o ICU (International Components for Unicode).

### Mas eu ainda poderei criar aplicações para GNOME?

Sim, nós possibilitamos que pessoas possam desenvolver aplicação GNOME utilizando Mono.

### Vocês têm variantes C# para GNOME?

Sim, o [projeto Gtk#](/docs/gui/gtksharp/) é uma variante para Gtk+, Gdk, Atk, libgnome, libgnomecanvas e libgnomeui. Outras bibliotecas que rodam sob o framework GNOME serão adicionadas baseadas na necessidade (e demanda).

Linguagens e Conectores
-----------------------

### Que linguagens de programação são suportadas no Mono?

Veja nossa página de [Linguagens de Programação](/docs/about-mono/languages/) para acesso à uma lista de compiladores - tanto comerciais quanto open source - que estão disponíveis para Mono.

### Por que as setas direcionais e a tecla tab não funciona com o IronPython?

O IronPython por padrão restringe a emulação do python via linha de comando (console). Para fazer com que as setas direcionais, a tecla tab (para auto completar os comandos) e a tecla backspace, execute o interpretador do IronPython com a seguinte sintaxe:

mono ipy.exe -X:TabCompletion

### O Mono suporta COM (Component Object Model)?

Veja [Interoperabilidade via COM](/docs/advanced/com-interop/).

### Existem conectores para o Open Office?

Existem conectores .NET para desenvolvimento de aplicações OpenOffice. Para mais detalhes, veja o Wiki do OpenOffice, [Integrando o Open Office com o Mono](http://go-ooo.org/wiki/index.php/Mono_Integration).

O openSUSE já disponibiliza uma versão do Open Office "Mono-enabled", sobre a qual desenvolvedores podem adaptar às suas necessidades.

Créditos
--------

Esse FAQ contém material que recebeu contribuição de Miguel de Icaza, Jaime Anguiano e Lluis Sánchez.

