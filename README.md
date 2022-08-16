# Investigate A Dataset
>This is an Exploratory Data Analysis project which investigates the Tmdb dataset to find useful insights
## Table of Contents
<ul>
<li><a href="#intro">General Information</a></li>
<li><a href="#questions">Questions for the Analysis</li>
<li><a href="#tech">Technologies And Libraries</a></li>
<li><a href="#about">About Dataset</a></li>
<li><a href="#setup">Setup</li>
<li><a href="#conclusion">Conclusions</li>
</ul>
<br>

<a id='intro'></a>
# General Information
> The dataset used for this project contains information about 10,000 movies collected from The Movie Database (TMDb), including user ratings and revenue
> Certain columns, like ‘cast’ and ‘genres’, contain multiple values separated by pipe (|) characters.
> There are some odd characters in the ‘cast’ column. Don’t worry about cleaning them. You can leave them as is.
>The final two columns ending with “_adj” show the budget and revenue of the associated movie in terms of 2010 dollars, accounting for inflation over time.

# QUESTIONS FOR THIS ANALYSIS
- 1.How is budget data distributed?
- 2.Do movies with high popularity have more revenues?
- 3.What are the top 20 most popular movies?
- 4.What are the top 20 movies with the highest revenue?
- 5.What are the top 20 most popular genres?
- 6.Which words occur the most in the title of movies?
- 7.Which words occur the most in movie overviews?

<a id='tech'></a>
# Technologies 
- 1.Python 3.7
- 2.Pip 20.3.4
- 3.Jupyterlab
- 4.Google Colab
### LIBRARIES
- 1.Pandas
- 2.Numpy
- 3.Seaborn
- 4.Matplotlib
- 5.Word Cloud
# About Dataset
> this dataset contains 21 columns and 10866 rows

> **Column name**:

>> id,imdb_id,popularity,budget,revenue,original_title,cast,homepage,director,tagline,keywords,overview,runtime,genres ,
>> production_companies,release_date,vote_count,vote_average,release_year,budget_adj and revenue_ad

<a id='setup'></a>
# Setup
- 1.Open google colab through this link <a>https://colab.research.google.com/</a>
![Sample cell in google collab](https://github.com/Akonobea/Investigate_A_Dataset/blob/main/sample_cell.png)
- 2.Click on upload and then proceed to upload the files in this repository
- 3.Alternatively, you can click on on github(after step 1),then enter the Url to this repository
- 4.Open the file with extension .ipynb
- **NB** : A notebook is made of a group of cells that may or may not run independtly.

- 4.To run a cell use shift+Enter. **NB** To run the ipynb file ,it is important to make sure the .csv file is in the same folder as the .ipynb file else there will be errors



<a id='conclusions'></a>
# CONCLUSION

- 1. Columns like homepage,tagline,keywords and production_companies had a lot of Nan values and had to be dropped even though they could yielded a lot of  useful insights

- 2. The budget_adj and revenue_adj columns seemed very interesting but I did not have the expertise to understand what they represented.
<br>


>Question 1: How is budget data distributed?

- Answer : The histogram shows that budget data is skewed to the left
![This is an image](https://github.com/Akonobea/Investigate_A_Dataset/blob/main/budget.png)

>Question 2: Do movies with high popularity have more revenues?

- Answer : Not necessarily.The analysis showed that movies with low popularity have less revenue but movies with high popularity can sometimes have high revenues or low revenues.
![This is an image](https://github.com/Akonobea/Investigate_A_Dataset/blob/main/scatter_plot.png)
>Question 3:What are the top 20 most popular movies?

- Answer : From the dataset ,we see that the top 20 most popular movies  > are Jurassic World ,Mad Max:Fury Road,Interstellar,Guardians of the Galaxy just to mention a few
![This is an image](https://github.com/Akonobea/Investigate_A_Dataset/blob/main/top_20.png)


>Question 4:What are the top 20 movies with the highest revenue?

- Answer :  The highest earning movies are Avatar ,Starwars:The force Awakens just to mention a few.

>Question 5 :What are the top 20 most popular genres?

- Answer : The most popular genres are Action/Adventure/Science Fiction/Thriller followed by Adventure/Drama/Science Fiction and Action/Science Fiction/Adventure just to mention a few

>Question 6: Which words occur the most in the title of movies?

- Answer: The most popular words in the title of movies are **Jurassic**,**World**, **Fury**, **Mad** occur frequently in the title of movies.
![This is an image](https://github.com/Akonobea/Investigate_A_Dataset/blob/main/word_cloud.png)

>Question 7: Which words occur the most in movie overviews?

- Answer: The most popular words in movie overviews are **years**,**Twenty**,**two**,**events**
