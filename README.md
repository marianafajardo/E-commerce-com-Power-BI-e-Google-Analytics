<h1 align="center">E-commerce com Power BI e Google Analytics</h1>
 
<p align="center">
  <img src="https://user-images.githubusercontent.com/102304054/175793172-455cc61c-8430-41f8-a65f-adec66196128.png">
</p>

## 1. Dashboard

Esse dashboard foi desenvolvido através do curso de **"Power BI Para Data Science, Versão 2.0"**, realizado pela [Data Science Academy](https://www.datascienceacademy.com.br/). Ele pode ser visualizado de forma online e interativa, clicando na imagem abaixo:

<p align="center">
<a href="https://app.powerbi.com/view?r=eyJrIjoiZTM2NDI0MGMtNjJiNC00NzllLWIxNjktMGQ1MmYwMGU1M2VlIiwidCI6IjhlNDJlNTBlLTNkMWEtNDAzYy04ZWZmLTU4OGJkOGQxMjk5ZiJ9"><img src="https://user-images.githubusercontent.com/102304054/175793174-e2ba04ee-831c-4b8c-84a2-40b5a095787c.png"></a>
</p>

## 2. Google Analytics

No Power BI é possível realizar uma conexão direta com o Google Analytics, porém, para que isso fosse possível, é necessário possuir uma conta no Google Analytics e o "meu acesso" no Google Analytics deveria estar configurado para captar as informações do meu Website, página e/ou Portal.

Como não tenho um website, não é possível realizar as configurações necessárias e a conexão direta ao Google Analytics, sendo assim, para o desenvolvimento desse dashboard, foram buscados dados reais do Google Analytics para análise de dados, criação de gráficos e construir um dashboard.

Os dados utilizados nesse dashboard são do Google Merchandise Store e foram extraídos do próprio site (https://shop.googlemerchandisestore.com/), ou seja, uma página da própria Google, que tem como objetivo extrair dados do próprio Google Analytics, mascarar esses dados e disponibilizar gratuitamente. 

## 3. Estudo de Caso

Uma empresa comercializa produtos online. A empresa configurou o **Google Analytics** para extrair dados sobre o perfil dos visitantes do portal de e-commerce e agora o Gestor da área de Marketing gostaria de ter as respostas às perguntas abaixo:

1. Como os clientes mais acessam nosso portal, por busca orgânica ou paga?
2. Quanto tempo em média um visitante permanece em nosso portal por dia do mês?
3. Qual é a principal fonte de acesso ao nosso portal?
4. Qual é o sistema operacional mais usado para acessar nosso portal?
5. Qual é o dispositivo mais usado para acesso ao nosso portal?
6. Qual é o total de faturamento por dia?

## 4. Indicadores

Com o carregamento dos dados e a compreensão dos dados, foi possível dar início no desenvolvimento das visualizações, conforme as informações solicitadas pela área de negócio.

**1. Como os clientes mais acessam nosso portal, por busca orgânica ou paga?**

Para responder a essa pergunta, foi utilizado um **gráfico de barras clusterizado na horizontal**, trazendo a coluna **"channelgrouping"**, tanto para o eixo X quanto para o eixo Y, concluindo que a maioria dos acessos ao Portal *"Google Merchandise Store"*, foi através de busca orgânica.

<img src="https://user-images.githubusercontent.com/102304054/175793176-94b13ef4-8160-4c6a-8412-9c2758d4f6df.png"/><a>
</p>

**Observação:** A *busca orgânica* é quando você abre o Google com o objetivo de realizar uma busca de um tema qualquer, e ao encontrá-lo, clica no link da página relacionada ao assunto. No momento em que você clica no link da página, o Google considera essa busca como orgânica, ou seja, ninguém pagou para você fazer aquilo. Por outro lado, uma empresa pode criar uma campanha, isto é, quando recebemos uma propaganda sobre um portal ou produto e clicamos no link para obter maiores informações, naquele momento, o Google considera essa busca como paga. E o objetivo aqui, é descobrir como os clientes mais acessam as páginas disponibilizadas no Google, através de busca orgânica ou paga.

**2. Quanto tempo em média um visitante permanece em nosso portal por dia do mês?**

Para responder a essa pergunta, foi utilizado um **gráfico de barras**, trazendo a coluna **"timeonsite_st"** para o eixo Y e alterando os valores dessa coluna, de *"Soma"* para *"Média"*. Em seguida, a coluna **"date"** foi selecionada e direcionada ao eixo X,  *"maximizando a hierarquia de data"*, apenas com a opção *"Dia"*.

<img src="https://user-images.githubusercontent.com/102304054/175793181-fdddde8e-b8af-4c6b-8ddd-1b59b6d26f56.png"/><a>
</p>

O gráfico a cima apresenta o tempo médio que um visitante permanece no portal *"Google Merchandise Store"* por dia no mês, podendo ser notado que por volta do dia 10, é onde os visitante permanecem mais tempo no Website.

**3. Qual é a principal fonte de acesso ao nosso portal?**

Para responder a essa pergunta, foi utilizado um **gráfico de cascata**, trazendo a coluna **"source_today"**, tanto para a opção Categoria quanto para o eixo Y, concluindo que a maior fonte para acesso ao portal *"Google Merchandise Store"*, foi o **Google**.

<img src="https://user-images.githubusercontent.com/102304054/175793186-54dbe2a3-7096-41f8-ba42-f722e9f492ca.png"/><a>
</p>

**4. Qual é o sistema operacional mais usado para acessar nosso portal?**

Para responder a essa pergunta, foi utilizado um **gráfico de área**, trazendo a coluna **"operatingsystem"**, tanto para o eixo X quanto para o eixo Y, concluindo que o sistema operacional mais usado para acessar o portal *"Google Merchandise Store"*, é o **Windows**.

<img src="https://user-images.githubusercontent.com/102304054/175793187-f36e4fd7-2161-4d1c-b90c-f8fb533a2173.png"/><a>
</p>

**5. Qual é o dispositivo mais usado para acesso ao nosso portal?**

Para responder a essa pergunta, foi utilizado um **gráfico de pizza**, trazendo a coluna **"devicecategory"**, tanto para a opção legenda quanto para a opção valores, concluindo que o dispositivo mais usado para acessar o portal *"Google Merchandise Store"*, é o **Desktop**, e talvez, não valha a pena investir tanto em aplicativos móveis para Smartphone, e principalmente para Tablet.

<img src="https://user-images.githubusercontent.com/102304054/175793188-afeb346e-1ef6-4f1c-a3fd-089c276d837a.png"/><a>
</p>

**6. Qual é o total de faturamento por dia?**

Para responder a essa pergunta, foi utilizado um **gráfico de linha**, trazendo a coluna **"transactionrevenue_st"** para o eixo Y e a coluna "date" para o eixo X, *"maximizando a hierarquia de data"*, apenas com a opção *"Dia"*, gerando uma espécie de serie temporal, ou seja, um evento que acontece ao longo do tempo.

<img src="https://user-images.githubusercontent.com/102304054/175793190-db13c13f-b0d8-4533-a998-a01f18bbc9eb.png"/><a>
</p>

Analisando o gráfico a cima, podemos notar que por volta do dia 10 do mês, há um pico em termos de faturamento, ou seja, nesse período houve um maior índice de compras registradas no website.

**7. Como está a evolução das PageViews (Páginas Visualizadas) no portal  "Google Merchandise Store"?**

Para responder a essa pergunta, foi utilizado um **gráfico de KPI**, trazendo a coluna **"PageViews_st"** para a opção Valores, alterando os valores dessa coluna, de *"Soma"* para *"Média"*. Em seguida, a coluna **"date"** foi selecionada e direcionada para a opção Eixo de tendência, *"maximizando a hierarquia de data"*, apenas com a opção *"Dia"*. Por último, a coluna **"PageViews_st"** foi adicionada também em Metas de destino, alterando os valores dessa coluna, de *"Soma"* para *"Máximo"*.

<img src="https://user-images.githubusercontent.com/102304054/175793191-3bcaac1d-1e37-4560-ad00-ccb630776d66.png"/><a>
</p>

No gráfico a cima, foi estipulado uma meta de 167 PageViews e o mesmo apresenta uma média de 1.26, bem abaixo da meta, isso provavelmente, indica que o usuário não está navegando pelas páginas, talvez porque ele não sabe como navegar, ou porque ele não sabe que tem outras páginas disponíveis, ou ainda, a navegação do portal não seja tão intuitiva, isto é, várias e várias questões podem estar relacionadas ao baixo KPI.

**Observação 1:** As PageViews são páginas visualizadas, isto é, quando um usuário chega a um determinado portal de E-commerce para fazer compras, é possível verificar a quantidade de páginas que ele acessa, até decidir, por fim, realizar a compra, sendo assim, através desse indicador, pode-se validar como está a interação do usuário com o portal de E-commerce.

**Observação 2:** O valor correspondente a meta de 167, está relacionado ao valor máximo de Pageviews  alcançado pelo  portal *"Google Merchandise Store"* em algum momento, porém a média como visto é de 1.26, sendo necessário, a realização de um trabalho, com o objetivo de tentar elevar a média atual, para o mais próximo possível do valor máximo alcançado em algum período. É provável que esse valor máximo, tenha sido alcançado devido alguma promoção, alguma campanha específica e/ou divulgação.
