# NPR Articles | Unsupervised Topic Modeling
## Clustering Topics with Latent Dirichlet Allocation and Non-Negative Matrix Factorization

* **Author**: Miguel Santana

Thank you for reviewing this repository. The author's contact info, sources and social media profiles are listed below under **further information.**

The contents of this repository detail a clustering analysis of National Public Radio (NPR) articles for topic discovery. The analysis will provide insight into clustering and dimensionality reduction within the context of natural language processing. 

#### Project Framework | OSEMN

**Data processing and analysis is completed using the OSEMN framework. The structure includes: Obtaining the data, Scrubbing (processing), Exploratory Data Analysis, Statistical Modeling and Interpretation of the Results.**

![](/images/OSEMN.png)

**Data processing and analysis is completed using the OSEMN framework. The structure includes: Obtaining the data, Scrubbing (processing), Exploratory Data Analysis, Statistical Modeling and Interpretation of the Results.**

### The Data

The dataset includes over 11,000 unlabeled NPR articles. The dataset was originally sourced from Udemy. The Udemy citation is available below under sources.

## Scrubbing/Data Cleaning 

The provided dataset was made available for illustrative purposes through Udemy. No data pre-processing was required in this analysis.

## Exploratory Data Analysis 

### Article Lengths

![jpg](/images/articlelength.jpg)

# Statistical Modeling 
## Latent Dirichlet Allocation

**Decisions:**
* 1) Ignoring terms with high document frequency.
* 2) Discarding words occurring in 90 percent (or more) of docs.
* 3) Removing stop words.

### Top Words
#### Top 15 Per Topic

    THE TOP 15 WORDS FOR TOPIC #0
    ['companies', 'money', 'year', 'federal', '000', 'new', 'percent', 'government', 'company', 'million', 'care', 'people', 'health', 'said', 'says']
    
    
    THE TOP 15 WORDS FOR TOPIC #1
    ['military', 'house', 'security', 'russia', 'government', 'npr', 'reports', 'says', 'news', 'people', 'told', 'police', 'president', 'trump', 'said']
    
    
    THE TOP 15 WORDS FOR TOPIC #2
    ['way', 'world', 'family', 'home', 'day', 'time', 'water', 'city', 'new', 'years', 'food', 'just', 'people', 'like', 'says']
    
    
    THE TOP 15 WORDS FOR TOPIC #3
    ['time', 'new', 'don', 'years', 'medical', 'disease', 'patients', 'just', 'children', 'study', 'like', 'women', 'health', 'people', 'says']
    
    
    THE TOP 15 WORDS FOR TOPIC #4
    ['voters', 'vote', 'election', 'party', 'new', 'obama', 'court', 'republican', 'campaign', 'people', 'state', 'president', 'clinton', 'said', 'trump']
    
    
    THE TOP 15 WORDS FOR TOPIC #5
    ['years', 'going', 've', 'life', 'don', 'new', 'way', 'music', 'really', 'time', 'know', 'think', 'people', 'just', 'like']
    
    
    THE TOP 15 WORDS FOR TOPIC #6
    ['student', 'years', 'data', 'science', 'university', 'people', 'time', 'schools', 'just', 'education', 'new', 'like', 'students', 'school', 'says']

#### Selecting Topic Labels & Mapping Features

* Cluster 0:'Money'
* Cluster 1:'Politics'
* Cluster 2:'People'
* Cluster 3:'Health'
* Cluster 4:'Lifestyle'
* Cluster 5:'Other'
* Cluster 6:'Education'

![jpg](/images/LDA.jpg)

## Non-Negative Matrix Factorization

**Decisions:**
* 1) Ignoring terms with high document frequency.
* 2) Discarding words occurring in 90 percent (or more) of docs.
* 3) Removing stop words.
* 4) TF-IDF Vectorizer

### Top Words NMF
#### Top 15 Words Per Topic

    THE TOP 15 WORDS FOR TOPIC #0
    ['new', 'research', 'like', 'patients', 'health', 'disease', 'percent', 'women', 'virus', 'study', 'water', 'food', 'people', 'zika', 'says']
    
    
    THE TOP 15 WORDS FOR TOPIC #1
    ['gop', 'pence', 'presidential', 'russia', 'administration', 'election', 'republican', 'obama', 'white', 'house', 'donald', 'campaign', 'said', 'president', 'trump']
    
    
    THE TOP 15 WORDS FOR TOPIC #2
    ['senate', 'house', 'people', 'act', 'law', 'tax', 'plan', 'republicans', 'affordable', 'obamacare', 'coverage', 'medicaid', 'insurance', 'care', 'health']
    
    
    THE TOP 15 WORDS FOR TOPIC #3
    ['officers', 'syria', 'security', 'department', 'law', 'isis', 'russia', 'government', 'state', 'attack', 'president', 'reports', 'court', 'said', 'police']
    
    
    THE TOP 15 WORDS FOR TOPIC #4
    ['primary', 'cruz', 'election', 'democrats', 'percent', 'party', 'delegates', 'vote', 'state', 'democratic', 'hillary', 'campaign', 'voters', 'sanders', 'clinton']
    
    
    THE TOP 15 WORDS FOR TOPIC #5
    ['love', 've', 'don', 'album', 'way', 'time', 'song', 'life', 'really', 'know', 'people', 'think', 'just', 'music', 'like']
    
    
    THE TOP 15 WORDS FOR TOPIC #6
    ['teacher', 'state', 'high', 'says', 'parents', 'devos', 'children', 'college', 'kids', 'teachers', 'student', 'education', 'schools', 'school', 'students']

#### Selecting Topic Labels & Mapping Features

* Cluster 0:'Health'
* Cluster 1:'Politics'
* Cluster 2:'Health Care'
* Cluster 3:'Military'
* Cluster 4:'Election'
* Cluster 5:'Lifestyle'
* Cluster 6:'Education'

![jpg](/images/NMF.jpg)

### Results, Limitations, Future Work

#### Results and Limitations
Topic modeling through LDA or MNF is an unsupervised learning process. As a result, we have no way of validating our model results. In this particular case, both algorithms clustered topics in a similar way but the non-negative matrix factorization algorithm separated the topics in a more distinguishable way. MNF simultaneously performs dimensionality reduction and clustering to achieve its results. 

#### Future Work

Future work should include the use of recurrent neural networks for text classification and sentiment analysis within the context of topic modeling for enhanced performance. 

#### Further Information

Please review the narrative of our analysis in [our jupyter notebook.](./jupyter_notebook.ipynb)

For any additional questions, please reach out via email at santana2.miguel@gmail.com, on [LinkedIn](https://www.linkedin.com/in/miguel-angel-santana-ii-mba-51467276/) or on [Twitter.](https://twitter.com/msantana_ds)

#### Sources

Additional analysis, notes and file sources can be found on Udemy's website. 

* Course Name: NLP - Natural Language Processing with Python by Jose Portilla

##### Repository Structure:

```

├── README.md               <- The top-level README for reviewers of this project.
├── jupyter_notebook.ipynb     <- narrative documentation of analysis in jupyter notebook

```

