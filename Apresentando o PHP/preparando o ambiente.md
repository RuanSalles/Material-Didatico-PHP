# Preparando o ambiente

### Instalando o PHP no Linux

<p align="justify">Este tutorial poderá ser reaproveitado para qualquer distribuição baseada no Debian, podendo ser PopOS, Lubuntu, Mint, Debian, Ubuntu e afins.
Configurar um ambiente linux para desenvolver com PHP, não é nada complexo, porém necessita de alguns passos para se obter uma instalação estável e que se comporte de maneira produtiva. A seguir iremos abordar os pontos aos quais eu creio serem importantes para a instalação de um ambiente para os iniciantes ou até mesmo para os um pouco mais experientes. </p>

**Instalando e configurando o PHP**

De início ao se utilizar um ambiente linux, é necessário verificar se existe alguma dependência desatualizada, para isso execute o seguinte comando, para realizar a verificação e atualização ao mesmo tempo:
```bash
sudo apt update && sudo apt upgrade -y
```

Após a devida atualização do seu sistema, iremos partir para as partes específicas do PHP.

```bash
sudo apt install software-properties-common -y
```
Adicione o repositório do PHP.

```bash
sudo add-apt-repository ppa:ondrej/php -y
```
Execute novamente o comando de atualização dos repositórios e instalação dos mesmos:
```bash
sudo apt update && sudo apt upgrade -y
```
Instale agora o PHP com inclusão do Apache:
```bash
sudo apt install php8.1 libapache2-mod-php8.1
```
Agora você poderá verificar a versão do seu PHP com o comando:
```bash
php -v
```
Obs: No caso de querer utilizar alguma versão específica do PHP ao invés da versão 8.1 que é apresentada neste artigo, você poderá no comando acima, bem como nos comandos abaixo alterar a versão trocando-a diretamente nos comandos respectivos, como o exemplo abaixo:


- PHP 7.3
```bash
sudo apt install php7.3 libapache2-mod-php7.3
```
- PHP 7.4

```bash
sudo apt install php7.4 libapache2-mod-php7.4
```

- PHP 8.0
```bash
sudo apt install php8.0 libapache2-mod-php8.0
```
E assim respectivamente, o mesmo serve para os comandos que serão citados a seguir.

Agora iremos instalar algumas bibliotecas e extensões úteis para o PHP com o seguinte comando:

```bash
sudo apt install php8.1-intl php8.1-mysql php8.1-sqlite3 php8.1-gd -y
```

Caso vá fazer uso de testes ou utilizar algum framework que dependa ou implemente testes, é aconselhável você instalar o phpunit com o seguinte comando:

```bash 
sudo apt install phpunit 
```
### Ambiente Windows

Para realizar a configuração do PHP no ambiente Windows, indicamos o acesso do artigo: [Como instalar o PHP no Windows do jeito certo](https://blog.schoolofnet.com/como-instalar-o-php-no-windows-do-jeito-certo-e-usar-o-servidor-embutido/) ou [Como Instalar o PHP e XDebug no Windows](https://www.treinaweb.com.br/blog/como-instalar-o-php-e-xdebug-no-windows)


### Escolhendo o Editor de Código

Neste ponto é a hora que você começa a ter contato com editores de código, IDE's e a partir daí a sopa de letrinhas não para mais. Porém o que é importante levar em consideração é que um bom editor de código pode lhe trazer benefícios e até mesmo alavancar seus estudos, em virtude de recursos como auto-completar, dicas de códigos e afins. 

A seguir irei comentar dois dos mais conhecidos e utilizados editores de código, ambos podendo ser utilizados para criação de qualquer aplicação, obviamente seus usos dependem muito mais do gosto do Desenvolvedor.

### Sublime Text
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/odpv0v6d2qu8bdm17g0h.png)

O sublime-text é um editor de códigos simples e leve, que trás suporte a maioria das linguagens de programação, conta com diversos recursos visuais de syntaxe highlight (letras coloridas), para diferenciar o que são variáveis, funções, etc... 

O mesmo é leve, como um simples editor de códigos, ele não possuí muitas personalizações finas, exceto mudança de tema, escolha de linguagem que será usada, modificação de fontes, tamanho de fonte e afins.

### Visual Studio Code - VSCODE
![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4ca06cbikyk4ca6eleff.png)

O Visual Studio Code ou VsCode como é mais conhecido, é uma solução da Microsoft que serve também como editor de códigos, a ferramenta é poderosa, a nível de tecnologias suportadas, personalizações de temas, fontes, espaçamentos, ícones, além de ter um grande suporte a extensões, que facilitam a vida de todo e qualquer desenvolvedor, seja em que Stack (linguagem) ele esteja utilizando. 

> Finalizada a configuração do seu ambiente PHP seja no Windows ou no Linux, escolhido seu editor de códigos, iremos a partir do próximo material iniciarmos de fato a manipulação e aprendizado da sintaxe do PHP e suas funcionalidades.