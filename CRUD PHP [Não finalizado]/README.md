## Create, Read, Update, Delete (CRUD PHP)

> Crud desenvolvido para facilitar as consultas e inser��es no banco de dados e reduzir linhas de c�digos.

![](image.png)

* Inserts, Updates, Select's, Delete's no banco de dados sem se preocupar com par�metros de vari�veis e todas suas estruturas. Esse CRUD far� todo o servi�o pesado e facilitar� sua vida no dia-a-dia, al�m de diminuir algumas linhas de c�digo...

# Atualiza��es:

- [ ] Varia��es entre inserts, updates, selects.
- [ ] M�todo DELETE,
- [x] M�todo **insert**,
- [x] M�todo **update**.
- [x] Met�do **selectOneOrMore**,
- [x] M�todo **selectAll**,
- [x] M�todo para verificar a exist�ncia de tabelas
- [x] Atributo global para comunicar com o banco de dados
- [x] Conex�o com o banco de dados (PHP-POO PDO)

## Exemplo de uso

#### - Iniciando

```php
$crud = new CRUD('host', 'user', 'pass', 'dbname', 'charset');
```
> **charset** n�o obrigat�rio. Como padr�o: **utf8**
------------
#### - Selecionar todos os registros de uma tabela
```php
$crud->selectAllQuery('tabela', 'where', 'order', 'limit');
```
> **order** e **limit** n�o obrigat�rio. Como padr�o: **nulo**
------------
#### - Selecionar uma ou mais coluna de uma tabela
```php
$crud->selectOneOrMore('tabela', String 'colunas', 'where', 'order', 'limit');
```
> **order** e **limit** n�o obrigat�rio. Como padr�o: **nulo**
------------
#### - Selecionar uma ou mais coluna de uma tabela
```php
$crud->update('tabela', String 'coluna(s)', Array 'valores', 'where');
```
> **order** e **limit** n�o obrigat�rio. Como padr�o: **nulo**
------------