## Introdução

C# e Linux, um casamento complicado? A um bom tempo atrás, era apenas possível desenvolver, sem dor de cabeça, para o ambiente .NET somente no Windows, com algumas ressalvas com a “falecida” IDE [MonoDevelop](https://www.monodevelop.com/) para ajudar o pinguim.

Bom, um pouco de história: em 2016, a Microsoft anunciava o .NET Core, uma reimplementação do famoso e amado, por uns odiados, Framework de sua autoria, dessa vez disponível para, além do Windows, o macOS e Linux. Claro, nem tudo são flores e é impossível fazer uma reimplementação de um gigantesco Framework igualmente completo como o seu “pai” do dia para a noite e distribuir por ai aos SO’s de maior relevância do mercado, mesmo que de forma gratuita e open source.

No ano de 2020, a versão 5 do .NET foi disponibilizada como estável, tanto SDK como para run time, o que marcou a unificação de uma baita confusão de versões do .NET, deixando para trás o .NET Framework (aquele exclusivo para Windows), .NET Core (versões iniciais do .NET open source) e a criação do padrão “.NET Standard.” Mas, agora retomando o rumo da venta. É viável programar em C# no Linux em 2024? Bom, a resposta é dupla: sim e não.

## Explicando

**Por que sim?**

Com o amadurecimento da ferramenta ao passar dos anos e, um gigante apoio, da JetBrains com a IDE Rider, desenvolver com C#, especialmente para a Web, Console applications, Worker Services e Unit Tests, hoje possuímos uma baita ferramenta completa, apesar de salgada, para desenvolver com comodidade no Linux (além de suporte para macOS e Windows, caso não queira o Visual Studio). Para os que ainda duvidam, deem uma olhada no meu mais recente e maduro projeto de ASP .NETC Core feito 100% no Linux: [CarteiraClientes](https://github.com/JGMelon22/CarteiraClientes)

![ImagemRider](https://user-images.githubusercontent.com/73988556/151468561-fbaa27be-625f-47c2-ac71-80a7a7f826d2.png)

**Por que não?**

Alguns podem estranhar que eu não comentei sobre o editor de textos, muito confundido com IDE, Visual Studio Code. O Visual Studio Code, apesar de ficar bem redondinho para codificar em C# com algumas extensões, especialmente as da imagem a baixo, acaba pecando por ser limitado em alguns aspectos, sendo os mais chatinho a falta de facilidade para auxiliar a geração de itens do Scaffolding ASP .NET Core - Usando os recursos do Scaffolding e a falta de suporte first party para desenvolvimento [MAUI](https://techcommunity.microsoft.com/t5/educator-developer-blog/net-maui-on-linux-with-visual-studio-code/ba-p/3982195).

![Extensions](https://github.com/JGMelon22/blog/assets/73988556/379f8a26-0586-4d19-a586-2513d63f81ed)

## Fazendo uma breve tangência: 

Existem alternativas ao .NET MAUI com first class suport para talvez Linux? Sim, jovem Padawan,  e essas duas alternativas já são consolidas são o [AvaloniaUI](https://avaloniaui.net/) e o [UNO Plataform](https://platform.uno/), ambos visando o desenvolvimento multiplataforma, Linux, macOS, Windows, Web, Android e IOS.
 
 ## Conclusão

Bom, caso você opte pelo desenvolvimento web, ASP. NET, desenvolver em C# no Linux, até o presente o momento, será uma experiência bastante agradável. Mas, caso você precise desenvolver aplicações locais usando WinForms, eu sinto em informar que somente pelo Windows mesmo, visto que o WinForms, assim como o Visual Basic For Application, depende de componentes do Windows para funcionar [Design Windows Forms | JetBrains Rider](https://www.jetbrains.com/help/rider/Working_with_Windows_Forms.html), você precisará usar o SO da Microsoft (ou via máquina virtual ou dual boot). 

## Continue lendo:

[Visual Studio Code - Instalação e costumização](https://balta.io/blog/visual-studio-code-instalacao-customizacao)

[WSL - Windows Subsystem for Linux](https://balta.io/blog/wsl)

[Plataform Specific no .NET](https://balta.io/blog/dotnet-platform-specific)
