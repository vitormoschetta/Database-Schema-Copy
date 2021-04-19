# Database-Schema-Copy

A ideia deste projeto é criar um console app em C# capaz de fazer uma cópia de um banco de dados informado em um destino informado.
Obs: de qualquer provedor de banco dedos,seja de origem ou destino.

Precisamos receber as seguintes informações (origem e destino):   

0. Provedor de banco de Dados
1. String de conexão;
2. Nome do Banco de Dados;
3. Nome do Schema;
4. Nome das tabelas (futuramente podemos automatizar a descoberta das tabelas)


O que mais precisamos:

1. Salvar as queries necessárias, separando e organizando por provedor de banco de dados. Preferencialmente chumbadas no próprio código fonte, ou arquivo de 
configuração, para não ser necessário utilizarmos base de dados própria. Deve funcionar apenas ao executar o app informando o que for necessário. 
