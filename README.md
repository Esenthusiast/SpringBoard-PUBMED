## SpringBoard-PUBMED Capstone 1
#Overview
This project is designed to search for trends within the Pubmed Publication database.
To start I am undergong a fishing expodition to identify if the rate of publications change throughout the year, if the rate per month- changes by year, or if within publications frequency of publication types changes by year. I am also considering if trends within publications are present (identified by word assocition within title or abstract) either by year, time of year, or within given topics.

The rate of total publications on Pubmed per year is > 700,000 papers. Therefore to narrow results category we are looking at papers with the keyword "Cancer" identified by Pubmed. 

#Dataset
My dataset consists of freely available Pubmed publications from the years of 2012-2017. Using the Entrez biopython module to fetch nested datasets on publications by keyword and date sorting I was able to scrape the abstract, title, first author information, journal title and publication date (month/year) for papers. A complete scrapping by year (even within the narrowed group) was ~200,000 papers. Therefore dataframe was initially limited to ~5,000 per year. 

#Initial Data Analysis:
Normal distribution of publications? 

#Topic Modeling


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
        
Use Cases:




People who publish want to optimize their impact 
    - timing, seasonality and/or funding
pharmaceutical companies track trends of 

  
          A list of UIDs (i.e. PMIDs).Abstract view, formatted in plain text.MEDLINE view, including the field indicators.The full XML of the record.

