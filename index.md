# [1] Instalação MSQL com WAMP
**framework 4 Client Profile (PT-BR)
Visual C++ Redistributable packages for Visual Studios 2013
(Ingles)(Vx30)**


*MSQL WorkBench*
(Windows)

`Lembrando que se você não baixou a framework e as packages,
a WorkBench não vai funcionar.`

# Instalação do Pacote WAMP
(v2013)

```
Agora temos WorkBench, 3 bibliotecas instaladas e WAMP(server)
```

## Sempre que você tiver o W verde, quer dizer que esta funcional.
Para verificar, clique no W, vá em MySQL e clique em MYSQL CONSOLE
para ver se o MYSQL esta realmente funcionando.

***Irá pedir um login use " root " e a senha basta dar enter.***
”No caso do WAMP SERVER é uma senha vazia”

*Se você seguiu tudo direito até aqui, para testar o status do sistema
digite status na console*
Caso mostrar informação é sinal que esta funcionando sem problema nenhum.


Para programar a Database de forma agradevel e util, iremos usar a Workabench
já ira ter reconhecido uma instancia local (localhost) basta clicar sobre o servidor
o painel vai abrir.



* Qualquer duvida meu email: gdgamerbrbet@gmail.com
* Meu discord: Cayo#0002






-
# Criando Banco de dados
Nome
Nacionalidade
Peso
Idade

- Instancias 
Utilizando esse padrão você basicamente pode registrar
qualquer tipo de pessoa, porque elas todas vão ter as mesmas
carecteriscas **(Não os valores)**

Agora vamos pegar uma caixa e colocar essas todas pessoas nele, nessa caixa vamos escrever no lado de fora " PESSOAS ".

Como se fosse um arquivo, e nesse arquivo todos ficheiros nele vão ter varias instacias com as mesmas casteriscas demostrado acima.

Você pode criar caixas diferentes para coisas diferentes
por exemplo:

Eu posso ter uma caixa chamada " JOGOS " aonde eu vou colocar
todas casteriscas de jogos. Pessoas e jogos são coisas diferentes esta entendendo? Por isso posso impor casteriscas diferentes, por conta disso têem que estar em caixas diferentes.

Nessa caixa jogos, vou colocar varios jogos que cada um tem suas propias casteriscas como:
Titulo
Fabricante
Genero
Plataforma

e tudo mais..

`Basicamente nós vamos agrupar coisas com casteriscas semelhantes, e separar coisas com casteriscas diferentes e essas coisas que tem casteriscas diferentes eu viu agrupar entre elas.`

*Agora vamos pegar essas duas caixas e colocae dentro de uma
carrinha.*

Isso tudo tem nome:
 - a carrinha é o meu banco de dados
 _O banco de dados são coleções de dados que são de casteriscas separadas, mas que estão organizadas em locais
 especificos esses locais especificos chamam-se tabelas._
 
 - a caixa é uma tabela
 _Tabelas guardam dados de coisas que tem casteriscas semelhantes, e se eu quiser posso ter varias tabelas dentro do mesmo banco de dados_
 
 -- Os dados que estão dentro da tabela tambem tem um nome especifico, chamam-se registros
 
 Resumindo, banco de dados são um conjunto de tabelas e tabelas são um conjunto de registros.
 
 
 # Criação do banco de dados
 Para criar o seu banco de dados no MSQL, basta dar o comado
 
 - CREATE DATABASE **NOME-DO-BANCO**;
 *no meu caso eu vou chamad de cadastro*
 
 Agora vamos para o MSQL WebBench que instalamos na #1
 lembrando que inicie o WAMP(SERVER) primeiro, espere que o W fique verde. 


**Agora, irei desmotrar screenshots**
<img src= "https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F53030673-4E7F-43B8-A444-F179C720268F.jpeg?v=1600002751052">
Feito isso, para executar o comando
<img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F6207AF32-209C-4DEE-99F0-3BB6545AAD84.jpeg?v=1600002784870">

Depois de executar o comando, para verificar se foi mesmo concluido
 <img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F653BAA68-1ECB-4778-B2A8-7A7CEAA97EAC.jpeg?v=1600002820656">
 Agora é so atualizar os esquemas
 <img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2FD1241F38-CD8E-4E39-ACBE-538143F921E9.jpeg?v=1600002843011">
 Agora vamos verificar o banco que criamos
 <img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F89EF190A-A351-4C52-8F69-C1238D0F9004.jpeg?v=1600002873124">
 Viu que tem lá as tabelas como dito anteriormente no exemplo.
 
 **Para criar a tabela**
 <img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F4322DB7D-070D-445B-B526-ECBB6EE0D9FD.jpeg?v=1600002925637">
 Dentro do comando **CREATE TABLE**
 nós vamos colocar:
 Nome 
 Idade 
 Sexo
 Peso
 Altura
 Nacionalidade
 
 - Deste jeito
 <img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F22B8182B-FF05-437C-935B-71FBAF2BFAF6.jpeg?v=1600002964616">
 
 
 ***Tipos primitivos***
 <img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F33B2A754-9771-4315-A28A-F812B881D496.jpeg?v=1600003007051">
 *Iremos falar mais sobre na proxima aula*
 
 Meu exemplo:
 coloque o comando **use cadastro;**
 em cadastro meta o nome do seu banco de dados
 e execute o comando, depois

 
 Agora atualize os esquemas
 
 - Como pode ver agora temos a tabela " pessoas "
 e tem as seguintes colunas
 <img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F8645C0A8-5FE3-4906-995E-6435AE0EAFA7.jpeg?v=1600003083421">
  
  Você quer ver como funciona a estrutura interna da tabela?
  -
  basta ir em baixo e colocar **describe pessoas;**
  <img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F83CAA6D8-C49A-488F-AF07-7C9403A1D6F2.jpeg?v=1600003246526>
 
 e executar o comando, depois disso ele vai abrir a estrutura da tabela pessoas
 
<img src="https://cdn.glitch.com/4bb6fe78-0917-4ca3-9dd3-aa140f52ff8a%2F512AF604-D594-4B1C-9DE0-ACC8FB133E9C.jpeg?v=1600003276574">

```
E assim terminamos a nossa segunda aula,
Mais para afrente iremos melhorar o nosso banco de dados
```
 
  
 
 
 
 
 
 
 
 
 
 





