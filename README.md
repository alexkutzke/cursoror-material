[//]: # (Title:	Curso Ruby on Rails: do zero ao deploy)
[//]: # (Author:	Prof. Dr. Alexander Robert Kutzke)
[//]: # (Date:		06/02/2017)

![Logo do Curso](logo.png "Logo do Curso")

# Material das aulas

* [Aula 01 - Introdução](01.html)
* [Aula 02 - Aplicação "do zero"](02.html)
* [Aula 03 - Continuação "Aplicação 'do zero'", console e seed](03.html)
* [Aula 04 - Controllers e prática](04.html)
* [Aula 05 - Aplicação Movie Store](05.html)
* [Aula 06 - Autenticação e Autorização](06.html)
* [Aula 07 - Término da aplicação Movie Store](07.html)
* [Aula 08 - Deploy, internacionalização e testes](08.html)

# Sobre o Curso

*Ruby on Rails: do zero ao deploy* tem a intenção de ser um curso direto e flexível sobre os tópicos mais importantes no desenvolvimento de aplicação Web com o framework Ruby on Rails.

Para tanto, desde os princípios básicos de instalação do Ruby até os conceitos mais importantes de servidores de produção serão abordados.

# Ambiente de trabalho

Embora o Rails esteja apto a ser executado em qualquer plataforma (melhor em algumas do que outras), durante o curso será realizada a tentativa de uso de uma máquina virtual simples. Assim, todos os alunos terão condições de compreender e executar os principais passos na configuração de um ambiente de desenvolvimento (e produção) Ruby on Rails.

Nesse sentido, para que tudo corra como planejado, é importante que todos os participantes que utilizarão suas próprias máquinas no curso tenham instalados e configurados os seguintes softwares:

* [VirtualBox]
* [Git]
* [Vagrant]
* [Sublime Text]

## Instruções para instalação

Os softwares citados possuem guias de instalação para cada tipo de plataforma.

Para ambientes GNU-linux e macOS, a instalação é, em geral, bem documentada.
Por favor, para tais plataformas, consulte guias de instalação disponíveis na internet.

A seguir, são apresentados links para os arquivos de instalação para plataforma Windows. Em todos eles, basta seguir o processo normal de instalação.

### VirtualBox

http://download.virtualbox.org/virtualbox/5.1.12/VirtualBox-5.1.12-112440-Win.exe

### Git

32-bit:
https://github.com/git-for-windows/git/releases/download/v2.11.0.windows.1/Git-2.11.0-32-bit.exe

64-bit:
https://github.com/git-for-windows/git/releases/download/v2.11.0.windows.1/Git-2.11.0-64-bit.exe

### Vagrant

https://releases.hashicorp.com/vagrant/1.9.1/vagrant_1.9.1.msi

É provável que a instalação do Vagrant solicite que o computador seja reiniciado.

### Primeiro teste com Vagrant

Siga os passos a seguir para averiguar se a instalação dos componentes foi realizada com sucesso:

1) Caso esteja em ambiente Windows, execute a aplicação "git bash" (o qual foi instalado juntamente com o Git). Para outras plataformas, utilize a aplicação de terminal de comandos de sua preferência.

2) No terminal aberto, digite os seguintes comandos.

```bash
	$ mkdir vagrant
	$ cd vagrant
	$ mkdir precise32
	$ cd precise32
	$ vagrant init hashicorp/precise32
	$ vagrant up
	$ # Esse processo exige internet e pode levar alguns minutos
	$ vagrant ssh
```

Caso, após os comandos acima, um terminal de uma máquina virtual Ubuntu esteja disponível, como no exemplo a seguir, então sua instalação foi realizada com sucesso.

```bash
	$ vagrant ssh
	Welcome to Ubuntu 12.04 LTS (GNU/Linux 3.2.0-23-generic-pae i686)

	 * Documentation:  https://help.ubuntu.com/
	New release '14.04.5 LTS' available.
	Run 'do-release-upgrade' to upgrade to it.

	Welcome to your Vagrant-built virtual machine.
	Last login: Fri Sep 14 06:22:31 2012 from 10.0.2.2
	vagrant@precise32:~$
```

Os comandos executados criaram uma pequena máquina virtual utilizando o Vagrant. A imagem utilizada foi de um Ubuntu "limpo" de 32bit, nomeada "precise32" pela equipe do Vagrant. Essa será a máquina virtual utilizada durante o curso.

O mais interessante do uso do Vagrant é que, para desenvolver suas aplicações, você poderá utilizar seu próprio ambiente nativo. Apenas as aplicações Rails desenvolvidas irão rodar na máquina virtual.

Sugiro uma rápida leitura em materiais sobre Vagrant disponíveis na internet como, por exemplo, a página oficial do projeto: https://www.vagrantup.com/

## Outras informações

Estarei sempre disponível para contato através de email: alexkutzke@gmail.com

Sugiro a todos aqueles que ainda não possuem uma conta no serviço GitHub_, que criem a sua até início do curso.

[VirtualBox]: https://www.virtualbox.org/wiki/Downloads
[Git]: https://git-scm.com/downloads
[Vagrant]: https://www.vagrantup.com/
[Sublime Text]: https://www.sublimetext.com/
[GitHub]: http://www.github.com
