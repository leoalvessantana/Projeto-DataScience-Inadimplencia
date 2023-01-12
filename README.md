# Challenge de Data Science

Esse é meu projeto do Challenge de Data Science promovido pela Alura, uma plataforma online de cursos de tecnologia.
A ideia do Challenge é simular uma experiência de trabalho em uma empresa ficticia. 

<div align="center">
<img src="https://i.imgur.com/oxab3uu.png" width="800px" />
</div>

A <b>Alura Cash</b> é um banco digital internacional. A diretoria do banco convocou a gente, a equipe de dados, para uma reunião para informar que, recorrentemente, estão surgindo pessoas inadimplentes após a liberação de créditos.

Por conta disso, foi solicitada uma solução para diminuir as perdas financeiras geradas por pessoas mutuárias que não quitam suas dívidas. Nos foi informado também que teríamos o prazo de **um mês** para encontrar essa solução e apresentá-la à diretoria financeira. Sendo assim, solicitamos um conjunto de dados contendo as informações de clientes, da solicitação de empréstimo, do histórico de crédito, bem como se a pessoa mutuária é inadimplente ou não. Decidimos dividir as tarefas em semanas, na semana 1 faremos um tratamento inicial nos dados usando SQL, na semana 2 utilizando o Python criaremos um modelo para prever a inadiplência e na semana 3 e 4 
criaremos visualizações dos resultados no Power BI.

## Semana 1 - Limpeza dos dados

O banco Alura Cash nos forneceu os dados em **dumps**. Utilizando o MySQL Workbench buscamos entender os dados e notamos que os dados de cada cliente estavam divididos em tabelas, especificados pelo ID. Também notamos a existencia de uma tabela que continha a relação de todos os IDs de uma mesma pessoa.

Unimos as tabelas pelos valores de IDs que eram correspondentes entre si, deixando todos os dados em uma única tabela. 

Decidimos não eliminar os valores nulos, pois podem ser importantes para o banco. E os valores em inglês vamos traduzir utilizando o python mesmo.

Exportamos a tabela com os dados únidos para o formato **csv** e vamos utiliza-lo nas próximas semanas.