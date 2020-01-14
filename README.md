![alt text](https://i.imgur.com/lbMEqqs.png)

PROJETO DA DISCIPLINA:
PRÁTICAS ORIENTADA EM COMPUTAÇÃO I e II
INTEGRANTES: 
   - EIKE SOUSA
   - JOÃO MANOEL
   - JOSÉ ROBSON
   - LUCAS BRABEC
   - MATHEUS AQUINO
   - EDSON MARQUES

*OBS: Como o projeto foi realizado para o departamento o projeto é privado. Segue somente o readme publico.

## 0) Tecnologias Utilizadas

Laravel, HTML, CSS, Javascript, PHP, GitHub, MySQL, Apache.
 
## 1) Problema

O Bicho no Campus da Universidade Federal de Sergipe possuia uma dificuldade de gerenciar seus animais para adoção, pois todos os dados eram armazenados no papel.
Não possuia divulgação dos animais que podiam ser adotados nem informações de como adotar, as pessoas muitas vezes até pegavam o animal na UFS sem avisar.

## 2) Solução

Um programa capaz de gerenciar todos animais para adoção e todas as informações dos animais adotados.

## 3) Escopo do Projeto

No projeto foi utilizado o [Laragon](https://laragon.org/download/) (ambiente de desenvolvimento isolado), pois ele vinha com os softwares necessarios para o projeto (Laravel, Git, Banco de Dados, Servidor Web) sem conflitos.

![alt text](https://i.imgur.com/kOMoYBo.jpg)

## 4) Documentação

* [Diagrama de Classe](https://i.imgur.com/GUjSrvX.jpg)
* [Diagrama de Casos de Uso](https://i.imgur.com/ObRbLDY.jpg)
* [Diagrama de Estados](https://i.imgur.com/ZeqpIDG.jpg)
* [Modelagem do Banco](https://i.imgur.com/Yg2jiZy.jpg)

## 5) Telas

* [00 - Inicio - Publico](https://i.imgur.com/58lhGQz.jpg)
* [01 - Inicio - Restrito](https://i.imgur.com/2vfarx5.jpg)
* [02 - Animais para adoção - Publico](https://i.imgur.com/H2GUEON.png)
* [03 - Animais para adoção - Restrito](https://i.imgur.com/xxvmqKW.png)
* [04 - Busca por animais - Publico](https://i.imgur.com/hdaEk6I.png)
* [05 - Busca por animais - Restrito](https://i.imgur.com/WAf2M8V.png)
* [06 - Animais requisitados - Restrito](https://i.imgur.com/MFdtEXc.png)
* [07 - Requisições do animal - Restrito](https://i.imgur.com/hTMVm2R.png)
* [08 - Situação da requisição - Restrito](https://i.imgur.com/RkNL9Bi.png)
* [09 - Gerenciamento de usuario - Restrito](https://i.imgur.com/74P6l8S.png)
* [10 - Cadastro de usuario - Restrito](https://i.imgur.com/UdBVDSq.png)
* [11 - Adicionar usuario - Restrito](https://i.imgur.com/jBzSKH5.png)
* [12 - Convidar usuario - Restrito](https://i.imgur.com/GunvEBF.png)
* [13 - Configuracoes do sistema - Restrito](https://i.imgur.com/1TAuRFs.png)
* [14 - Criar, alterar e excluir especies - Restrito](https://i.imgur.com/lvO7lRl.png)
* [15 - Modificar imagem do inicio - Restrito](https://i.imgur.com/UBEVTwA.png)
* [16 - Modificar texto "quem somos" - Restrito](https://i.imgur.com/3rSZIoj.png)

## 6) Iniciar o Projeto

Para iniciar o projeto pela primeira vez, deve seguir esses passos para todos os arquivos e todas as configurações sejam atualizadas.

### a) Atualizar o composer

* 1 - Faça o git clone.
* 2 - Abra o terminal.
* 3 - Digite:
```sh
composer update
```

**OBS: Caso não dê o composer update alguns arquivos necessarios não serão instalados na maquina. Provavelmente ocorrerá esse erro.**

![alt text](https://i.imgur.com/rJ36tVE.png)

### b) Criar o arquivo .env

* 1 - Duplique o arquivo ".env.example".
* 2 - Renomei o arquivo para ".env".
* 3 - Abra o terminal.
* 4 - Digite o comando:
```sh
php artisan key:generate
```

**OBS: Caso não faça esses passos haverá um problema de configuração. Ocorrerá esse error.**

![alt text](https://i.imgur.com/F37iMGy.png)

### c) Criar e Povoar o Banco de Dados

* 1 - Crie o banco de dados.
* 2 - Modifique a configuração de banco de dados no arquivo ".env".
* 3 - Modifique a configuração de banco de dados no arquivo "config/database.php".
* 4 - Abra o terminal.
* 5 - Digite o comando:
```sh
php artisan migrate
```
* 6 - Digite o comando:
```sh
php artisan db:seed
```

### d) Atualizar alguns componentes

* 1 - Abra o terminal.
* 2 - Digite o comando:
```sh
composer require unisharp/laravel-ckeditor
```
* 3 - Digite o comando:
```sh
php artisan vendor:publish--tag=ckeditor
```
* 4 - Digite o comando:
```sh
npm install
```
