# 📚The Briefing Room

## Real example: Find, Clean and Merge Data.
As a Data Analyst, “find, clean and merge” Data is the essential step for your daily role. 
On one occasion, When I was working as Data Analyst and Project Consultant for a state deputy cabinet, the parliament was in a heated moment because of a crisis between several Brazilian states, concerning about the tax rates on jet fuel. 
In one hand was one parliamentary group trying to collect more taxes, and in the other side was a party that advocated the opposite: they were trying to lower the rate, in the attempt to promote more international passengers flights to our state (specially from Europe, because the flights from the US were already consolidated).
As part of my job as a consultant, I needed to provide insights that could help the debate and, at the end, support my team.  
My goal was to find Data and show the situation of the Brazilian international aviation. For that, my idea was to create a dynamic dashboard in Tableau, showing with some lines, the density of flights from Europe to the Northeast region of Brazil. With this data precious asset, I could compare the flights to our state with the others from the same region of Brazil.

## 🔎 Where to find trustful Data and what to do with it?
Whenever possible, try to find Data directly from a government source or from a reference company, only after that try on open private repositories. This is the key part of the job: find good and trustful Data.
After some research, I found a public repository from the National Civil Aviation Agency of Brazil, containing a 220MB .csv file, with all the database of registered flights in Brazil since 2000.
The updated Data (until march 2021) can be found [here]( https://www.anac.gov.br/acesso-a-informacao/dados-abertos/areas-de-atuacao/voos-e-operacoes-aereas/dados-estatisticos-do-transporte-aereo/48-dados-estatisticos-do-transporte-aereo-formato-csv).
The only problem with this dataset is that is missing the coordinates from each airport, what is a trouble for geographic localization in Tableau.
I could not find an official repository with geographic location of the aforementioned airports, so I used this one [here](https://datahub.io/core/airport-codes).
With these two datasets I could merge then, allowing me to have all the flights information added to the coordinates of each airport, from departure to arrival.

## 🧹 🛠 Get your hands dirty
Once you have your Data, it’s time to get your hands dirty. 
The csv file has more than 900K rows and 35 columns, what makes impossible to work with Excel. 
So, to handle this Dataset I used Python, with the two libraries listed below. 
In the next lines the work can be seen, generating, at the end, a clean and smaller csv file, with just the necessary data to be used in Tableau.

-	[X] Pandas
-	[X] Chardet

## ✒️ Developer

Marcelo Pasquini

 [LinkedIn Profile](https://www.linkedin.com/in/mpbrazil/)
