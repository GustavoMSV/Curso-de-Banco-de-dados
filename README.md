# Exercicio Livaria 
> Este projeto é um exercicio do curso de SQL e Banco de dados que estou realizando pela plataforma Udemy com o Professor Felipe Mafra.

#### SoftWares Utilizados: 
- MySQL
- NotePad
- VirtualBOX
---
_**Criação da DataBase:**_

![img](print.png)

---

## Exercicio:

O nosso cliente solicitou uma tabela para armazenar os livros que são comercializados pela empresa. A solicitação é somente para livros e não há a necessidade de realizar busca em outras tabelas. Hoje há um funcionário de vendas que tem uma tabela do Excel para guardar esses registros, mas as buscas estão ficando complexas. Decidiu-se então criar um banco de dados separado para esse funcionário.
Após a criação da tabela, deveremos entregar algumas queries prontas para que sejam enviadas para o programador. As queries são as seguintes:

1 – Trazer todos os dados.
2 – Trazer o nome do livro e o nome da editora
3 – Trazer o nome do livro e a UF dos livros publicados por autores do sexo masculino.
4 - Trazer o nome do livro e o número de páginas dos livros publicados por autores do sexo feminino.
5 – Trazer os valores dos livros das editoras de São Paulo.
6 – Trazer os dados dos autores do sexo masculino que tiveram livros publicados por São Paulo ou Rio de Janeiro (Questão Desafio).

### SQL (Resolução)
```SQL
/*1 - TRAZER TODOS OS DADOS*/
SELECT * FROM LIVROS; 

/*2 - Trazer o nome do livro e o nome da editora*/
SELECT LIVRO, EDITORA FROM LIVROS;

/*3 - Trazer o nome do livro e a UF dos livros publicados por autores do 
sexo masculino*/
SELECT LIVRO, UF FROM LIVROS 
WHERE SEXO = 'M';

/*4 - Trazer o nome do livro e o número de páginas dos livros publicados 
por autores do sexo feminino.*/
SELECT LIVRO, PAGINAS FROM LIVROS
WHERE SEXO = 'F';

/*5 - Trazer os valores dos livros das editoras de São Paulo.*/
SELECT VALOR FROM LIVROS
WHERE UF = 'SP';

/*6 - Trazer os dados dos autores do sexo masculino que tiveram livros 
publicados por São Paulo ou Rio de Janeiro (Questão Desafio).*/
SELECT AUTOR, SEXO FROM LIVROS 
WHERE SEXO = 'M' 
AND UF = 'SP';
```
---

## Referências
[O curso completo de Banco de Dados e SQL, sem mistérios!][curso]

[curso]:https://www.udemy.com/course/bancos-de-dados-relacionais-basico-avancado/

---

## Contato 

Gustavo Moreno - [Linkedin](https://www.linkedin.com/in/gustavo-moreno-5803a0229)

Meu e-mail: gustavomorenosiqueira86@gmail.com

Celular: (11) 99786-8798