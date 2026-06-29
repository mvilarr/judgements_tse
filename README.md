<h1>An analysis of how Brazil's Superior Electoral Court judges political parties' financial reports</h1>

<h2>What is this</h2>

<p>This project was the first assignment I completed during the Lede Program, Columbia University's summer course in data journalism.</p>

<p>The idea came after Brazil's Chamber of Deputies approved a bill in May 2025 proposing a mini electoral reform. Among other changes, the bill would reduce the fines imposed on political parties whose annual financial reports are rejected and establish a one-year statute of limitations if Brazil's Superior Electoral Court (TSE) fails to rule on those reports.</p>

<p>While researching the proposal, I discovered that the TSE provides a public database containing the outcomes of political parties' financial reports. I wanted to investigate which parties had accumulated the highest electoral fines and which had their reports rejected most often.</p>

<p><h2>What I found</h2></p>
<p>The first surprise was that most financial reports have still not been judged — more than 60% remain pending. I also found that five political parties failed to submit their annual financial reports, a total of ten times between 2010 and 2024. Finally, I discovered that two of the three political parties that sponsored the electoral reform bill are among those with the highest accumulated electoral fines, confirming one of my initial hypotheses.</p>

<p><h2>How the data was collected</h2></p>
<p>The data was collected from the TSE's public website: https://www.tse.jus.br/partidos/contas-partidarias/prestacao-de-contas.</p>
<p> I then went to its political party financial reporting system (SICO): https://sico-consulta-web.tse.jus.br/sico-consulta-web/home.jsf. 
<p>  I filtered the database by selecting "Annual Political Party Financial Reports"(prestação de contas partidárias anuais) under "Type" (Tipo) and "National Party Committee"[Diretório Nacional) under "Party Organization Level" (Tipo da Direção Partidária) since I wanted to analyze only the national leadership of each party rather than state or local branches. 
<p> The data was downloaded on June 21, 2026, and covers reports from 2010 through 2024. Financial reports for 2025 were not included because political parties had until the end of June 2026 to submit them.</p>

<p><h2>Overview of the data analysis process</h2></p>
<p>Looking back, I spent too much time exploring the dataset in Pandas without a clear analytical plan. I realized later that I could have structured the code more efficiently by grouping the data by political party from the beginning instead of repeating similar operations for each analysis.
<p>I also encountered some technical challenges when importing the CSV file, such as identifying the correct encoding and delimiter. </p>
<p>Functions like unique() helped me understand the categorical variables, while groupby() became the foundation of most of the analysis.</p>
<p>Another challenge emerged after I thought I had finished the analysis. Several political parties had merged, dissolved, or changed their names over time. To address this, I produced two versions of the analysis - oOne preserving the historical party names and another using the current party names.</p>
<p>Only later did I realize that it would also be interesting to analyze how long the court takes to rule on each financial report</p>

<p><h2>What I learned</p></h2>
<p>This was my first time using Datawrapper, and I initially struggled to choose the most effective visualizations. After reading Soma's tutorial, talking to TAs and asking classmates for feedback, I made some changes and I became much more comfortable with them.</p>
<p>It was also my first time using GitHub to publish a personal project. Once I learned the workflow, it turned out to be much easier than I expected.</p>
<p>Beyond that, I learned how to use Pandas for data analysis, how to adapt an HTML template into a project website, and how to build a complete data journalism project from data collection to publication, which felt like I had superpowers or something.</p>

<p><h2>What I could have done better</h2></p>
<p>Given more time, I would have improved the visual design of the charts by incorporating each political party's logo, colors, and typography, likely using Illustrator. I also would have liked to customize the website further, but I have limited front-end development experience, so I was not able to do within the available time. </p>
