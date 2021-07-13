# News Crawler to the TradeMap app.

This is the final project of the topics discipline; initials MS902; offered by IMECC - UNICAMP at the first semester of 2021.

The code was implemented on Databricks, using the student version. Its documentation is in Portuguese, including the tables.

Credits to:

Matheus Souza

Vinicius Jameli

Bryan Prado

Raul Teixeira

Gabriel Borin

Pedro Pietrafeza

# TradeMap

Trademap is a mobile and desktop platform created to compile tools and contents that allow investors to monitor the market in real time, manage their investments and operate quickly, easily and safely.

One of these tools is its "News" interface, as showed in the image below.

<img src="https://trademap.com.br/wp-content/uploads/2020/07/Print-App-Trademap-3-500x1080-1.jpg" alt="java" width="400" height="700" /> 


In light of this, the project aims to create an alternative version of the web crawler that is already implemented in the app.

# General Functionality

More specifically, Trademap uses 24 different websites to get the news. Then, our goal is to acess thoses websites and extract just the relevant news and show them for the user.

To acomplish that, we used a table with all companys listed in B3, the Brazilian stock market, including some international and important ones.

That is, to each line on the table, the crawler will search if there's any new in all websites that corresponds to the name of the company, or its name in the stock-market.

It's important to say that the crawler just search the initial page of the website.

![alt text](https://uploaddeimagens.com.br/images/003/330/143/original/percorrer.png?1626050541)

Here's an example of how the news are disposed on the initial page, tooking the website https://www.infomoney.com.br/ as an example.

![alt text](https://uploaddeimagens.com.br/images/003/330/137/original/exemplo.png?1626050446)

Every correspondency is saved in the table below:

![alt text](https://uploaddeimagens.com.br/images/003/330/145/full/output.png?1626050666)

Finally, when the user searches for news regarding any company, the table above is accessed and the output is the news in the dataframe about the company in question.

# Some parameters

Number of companys: 517

Number of crypto coins: 10

Number of sites: 11 sites of 24 sites in the TradeMap

Average computational time of execution: 36 minutes
