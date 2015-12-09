---
title: Mono Basics
redirect_from:
  - /Mono_Basics/
---

Depois que seu Mono tiver sido instalado, provavelmente  é uma boa ideia executar um rápido programa "Hello World" para certificar-se de que tudo está configurado corretamente. Essa é a forma para você saber se seu Mono está funcionando antes de você escrever ou rodar aplicativos mais complexos.

Hello World no Console 
-------------------

Para testar as funcionalidades básicas disponíveis, copie o seguinte código dentro de um arquivo chamado hello.cs.

``` csharp
using System;
 
public class HelloWorld
{
    static public void Main ()
    {
        Console.WriteLine ("Hello Mono World");
    }
}
```

Para compilar, use o mcs:

    mcs hello.cs

O compilador irá criar "hello.exe", no qual você pode rodar usando:

    mono hello.exe

O programa irá rodar e exibir como saída:

``` bash
Hello Mono World
```

Conexões HTTPS
-----------------

Para ter certeza de que as conexões HTTPS funcionam, baixe  e rode a ferramenta  [tlstest](https://raw.github.com/mono/mono/master/mcs/class/Mono.Security/Test/tools/tlstest/tlstest.cs) (a versão do Mono precisa ser maior ou igual à 3.4.0).

``` bash
mcs tlstest.cs /r:System.dll /r:Mono.Security.dll
mono tlstest.exe https://www.nuget.org
```

O programa exibirá um erro se houver alguma coisa errada.

Hello World em Winforms 
--------------------

Escrevendo uma aplicação de teste em Winforms.

``` csharp
using System;
using System.Windows.Forms;

public class HelloWorld : Form
{
    static public void Main ()
    {
        Application.Run (new HelloWorld ());
    }

    public HelloWorld ()
    {
        Text = "Hello Mono World";
    }
}
```

Para compilar, use o mcs com a opção -pkg para informar ao compilador para invocar as bibliotecas do Winforms.

    mcs hello.cs -pkg:dotnet

O compilador irá criar "hello.exe", no qual você pode rodar usando:

    mono hello.exe

NOTA: No MAC OS X você terá que esperar torno de um minuto na primeira vez em que você executar este comando.

Hello World em ASP.Net 
-------------------

Crie um arquivo de texto com o nome hello.aspx com esse conteúdo:

``` csharp
<%@ Page Language="C#" %>
<html>
<head>
   <title>Sample Calendar</title>
</head>
<asp:calendar showtitle="true" runat="server">
</asp:calendar>
```

Então rode o comando xsp4 a partir desse diretório:

``` bash
xsp4 --port 9000
```

Use o navegador para acessar [http://localhost:9000/hello.aspx](http://localhost:9000/hello.aspx)

Hello World em Gtk# 
-----------------

Escrevendo uma aplicação de teste em Gtk#.

``` csharp
using Gtk;
using System;

class Hello
{
    static void Main ()
    {
        Application.Init ();

        Window window = new Window ("Hello Mono World");
        window.Show ();

        Application.Run ();
    }
}
```

Para compilar, use o mcs com a opção -pkg para informar ao compilador para invocar as bibliotecas do Gtk# (O Gtk# precisa ser instalado no seu sistema para que isso funcione):

    mcs hello.cs -pkg:gtk-sharp-2.0

O compilador irá criar "hello.exe", no qual você pode rodar usando:

    mono hello.exe
