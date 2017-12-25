# CRUD com PHP e MySQL

Curso: http://www.alura.com.br/cursos-online-introducao/php-mysql-e-fundamentos-da-web

Repository: https://github.com/alura-cursos/php-mysql-e-fundamentos-da-web

## Tutorial

Install wampp and acess localhost/phpmyAdmin & localhost/loja

## SCRIPT SQL
````SQL
create database loja;
create table produtos (id integer auto_increment primary key, nome varchar(255), preco decimal(10,2));
insert into produtos values (1, 'Carro', 20000);
insert into produtos values (2, 'Motocicleta', 10000);
alter table produtos add column descricao text;
update produtos set descricao = "Descrição deste produto";

create table categorias (id integer auto_increment primary key, nome varchar(255));
insert into categorias (nome) values ("esporte"), ("escola"), ("mobilidade"), ("guloseimas");
alter table produtos add column categoria_id integer;
update produtos set categoria_id=3;
update produtos set categoria_id=4 where id=17;

alter table produtos add column usado boolean default false;
````