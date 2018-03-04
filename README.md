## SpringBoard-PUBMED Capstone 1
# Overview
This project is designed to search for trends within the Pubmed Publication database.

To start I am undergong a fishing expodition to identify if the rate of publications change throughout the year, if the rate per month- changes by year, or if within publications frequency of publication types changes by year. I am also considering if trends within publications are present (identified by word assocition within title or abstract) either by year, time of year, or within given topics. 

# Dataset
My dataset consists of freely available Pubmed publications from the years of 2012-2017. Using the Entrez biopython module to fetch nested datasets on publications by keyword and date sorting I was able to scrape the abstract, title, first author information, journal title and publication date (month/year) for papers. A complete scrapping by year (even within the narrowed group) was ~200,000 papers. Therefore dataframe was initially limited to ~5,000 per year. 

# Motivation
Pubmed is a database of peer-reviewed research papers in a variety of academic and medical topics. The distribution of information through Pubmed and accessibility of research is a cornerstone of the scientific community. 
However, not all information or publications are created equal. 

Within pubmed there are journals with a high impact factor score - and publication in such a journal increases the visibility of an institution or researcher's paper- therefore increasing the potential ability to influence the scientific community. Therefore, reserach institutions wish to employ people who publish in high impact factor journals (IFJ), and individual researchers work hard to get their research published in those journals. 

For the good of the overall research community it is ideal if the research with the greatest scientific value is published in high IFJs. However, from an institution and research individuals perspective their paper has the greatest chance of causing a steer and aiding their funding and careers if it is published in IFJs- and can increase the percieved scientific value. 

Therefore, it is an important question:

- Are there points of human bias if what papers are published in high IFJ? Can we identify social trends in those papers over time? 

# Data

1) Build a custom scraper to isolate data from Pubmed
-  The rate of total publications on Pubmed per year is > 700,000 papers. Therefore to narrow results category we are looking at papers with the keyword "Cancer" identified by Pubmed. To consider trends over time started with publications from 2012-2017 to represent a range of time. 
- Used Biopython module tools to extract and initial organization of data 

2) Clean data
- Pandas DataFrame for data wrangling and cleaning into 5 dataframes from the original csv files.

3) Initial Data Analysis:
- Normal distribution of publications. The data we have is a random sampling of all the Pubmed papers containing the keyword "Cancer" in order to have a realistic sized sample of one field, for 5 years (2012-2017). That said for each year we are still only sampling ~ 2.5% of all potential data samples. Therefore I wanted to confirm that overall publication rate fit a normal distribution- and was indeed most likely a random sampling within the potential sample size. 

#Topic Modeling

4) TFDIF 
Looking at key vocabulary words in the titles and abstract using TFDIF
#Final Goal (in progress)

- identify interesting trends:
    - Publication normalized trend by month
    - different rates of key word use in topic/ abstract by journal? (specifically the top 10 high impact journals on the list vs low impact journals)
    - changing word-association with research findings? common odd pairings? etc. 
    - What Articles tend to have high impact? Or what articles tend to be published in high-impact journals?
        - by keyword association
        - by topic
        - by title


- Produce predictive model identify trends for example:
        - how does the publication date and keyword effect impact score
        - How does the publication date and keyword effect paper published in- journal impact score
        - are there any natural variations throughout the year or trends in papers published in large high impact journals through time. 
        - keywords + key phrases in abstract have effect on publication date?
        - publication date have effect on impact score? overall or within specfic sub groups
        - use regression model (R score, 0.05 varience) 

## Final data and analysis also available on my blog at https://theenthusiasticscientist.wordpress.com/

# Use Cases:

People who publish want to optimize their impact in relationton to:
1) timing, seasonality, keyword optimization, and/or funding
pharmaceutical companies track trends of publications and want to identify easy markers of:
1) impactful reserach and 
2) medically relivant research

  
          A list of UIDs (i.e. PMIDs).Abstract view, formatted in plain text.MEDLINE view, including the field indicators.The full XML of the record.

