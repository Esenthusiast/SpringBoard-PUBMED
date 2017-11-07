# SpringBoard-PUBMED
Springboard 
#Current goals
- Scrap data from pubmed
- initial data wrangling
    - organize into columns/table:
        - Title
        - Author(s)
        - keyword(s)
        - abstract words present or full abstract(?)
        - publication date
        - journal published

#Final Goal (in progress)

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
        
   Notes:
  impact score defined as number of links to paper within an amount of time
  
          A list of UIDs (i.e. PMIDs).Abstract view, formatted in plain text.MEDLINE view, including the field indicators.The full XML of the record.

