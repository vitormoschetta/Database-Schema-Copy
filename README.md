# Database-Schema-Copy

A ideia deste projeto é criar um console app em C# capaz de fazer uma cópia do `Schema` de um banco de dados de qualquer provedor. Exemplificando, imaginemos que eu tenha um banco de dados Oracle com um schema 'X', e desejo transformar ele em um banco de dados Sql Server, trazendo a mesma etrutura de tabelas e colunas existente no schema 'X' do meu DB Oracle.

##### Precisamos receber as seguintes informações (origem e destino):   

0. Provedor de banco de Dados
1. String de conexão;
2. Nome do Banco de Dados;
3. Nome do Schema;
4. Nome das tabelas (futuramente podemos automatizar a descoberta das tabelas)

<br>


##### O que mais precisamos:

1. Montagem das queries genericas que deverão ser utilizadas para a extração do schema. Precisamos montar e organizar essas queries por provedor.

<br>


##### O que basicamente o console app deve fazer?

O app é executado e recebe de alguma forma (pode ser nos argumentos de inicialização) as informações que precisamos, tanto de entrada de dados quanto de saída, conforme descrito anteriormente. 

Ele precisa montar e guardar em memória cada uma dessas informações. Deve guardar em memória também uma lista de tabelas (nome das tabelas), uma lista de colunas e tipos relacionadas à essas tabelas. Isso pode ser tudo guardado em memória para a execução da criação do novo schema. Podemos tanto extrair tudo primeiro para depois criar o novo schema, ou extrair e criar uma tabela por vez.




