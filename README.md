# Modelo de recomendação de produtos

Olá, seja muito bem vindo a este projeto da criação de um modelo de recomendação de produtos :happy:

Este projeto foi desenvolvido como uma dinâmica individual de treinamento do curso Data Expert, oferecido pela Dinâmica Group (DNC). Trata-se de dados de funcionamento de um e-commerce, que deseja realizar a construção de um modelo de recomendação dos seus produtos ofertados.



## Introdução

Foram disponibilizados quatro diferentes datasets: order_items, order_reviews, orders e products. 



- **Order_items:**

O dataset formado por order_items continha dados referentes a venda, tais como o valor da compra, o número de produtos comprados, o id do produto e o id da compra.



- **Order_reviews:**

Em relação ao order_reviews é composto por um identificador do review, o identificador da compra e a avaliação do produto.



- **Orders:**

Já para order, é composto pelo identificador da compra, o identificador do consumidor e o status da 		compra (se foi entregue, está a caminho, etc)



- **Products:**

Por fim, a tabela produtos é formada pela descrição do produto, como sua devida categoria e informações de sua dimensão, peso e características de nome e descrição.



## Escopo

Observando os dados referentes a estes produtos, foi determinado que seria viável realizar a construção de um modelo de recomendação com os mil produtos mais vendidos pelo e-commerce, ordenados pela avaliação dos usuários.



## EDA e tratamento dos dados

Foi realizada uma breve análise de cada um dos dados fornecidos, verificando os valores nulos, dados duplicados e alguns gráficos para entender melhor o funcionamento deste e-commerce.

Ao final, foi construído o dataset "ProdutosMaisVendidos.csv", que engloba os mil produtos mais vendidos, com a sua nota média, características físicas e suas devidas categorias dummificadas. 



## Modelo

Foi construído um modelo utilizando uma matriz de correlação entre os produtos, através da similaridade pelo cosseno. Desta forma, ao ser informado algum dos mil produtos mais bem avaliados, é informado os 10 produtos mais similares àquele escolhido, assim como o grau similaridade, entre 0 e 1.



## Aprendizagens

Neste projeto consegui entender um pouco melhor como realizar a construção de um modelo de recomendação, além de poder praticar vários conteúdos aprendidos durante o curso, como a junção de dataframes, pivot tables, ordenação e algumas funções de repetição. 

