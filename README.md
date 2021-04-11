# TCC_PUC_MINAS_ARQUITETURA
Diretorio designado para inclusão do código fonte do TCC de arquitetura de software.

-----------------------------
A senha do arquivo RAR encontra-se no apendice do TCC enviado pelo canvas. 

Passos para criação do ambiente:

Utilizando o MySQL command line, executar o script abaixo:

create database dbusuario;

use dbusuario;

CREATE TABLE `tbusuarios` (
  `nome` varchar(200) NOT NULL,
  `sobrenome` varchar(200) NOT NULL,
  `email` varchar(200) NOT NULL,
  `senha` char(64) DEFAULT NULL,
  `cpf` varchar(11) NOT NULL,
  PRIMARY KEY (`cpf`)
); 

-------------------- fim do script-----------------

Também é necessário possuir um broker kafka rodando no servidor localhost:9092 para enviar o email. 

Para envio do email, é necessário incluir um email válido com senha no arquivo Infraestrutura Modulo Cidadão\Microservico Email\Controller\email.js nos campos user e pass da linha 9 e 10 respectivamente.

Qualquer dúvida, sinta-se a vontade para entrar em contato pelo Canvas ou pelo email cadastrado. 

