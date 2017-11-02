# HCDS512_A2
## HCSD 512 Homework A2
## Michael Grant

### License: MIT
The MIT license means that this work is open to use by anyone, just please credit me for the work. 

---

Data collection is arguable one of the most important aspects of being a data scientist. My background in the applied sciences was all about data collection in laboratory and field settings. Designing experiments and collecting results is where the bulk of my data originated. However, collecting data in this way is extremely time consuming, and there is a mountain of data for the taking on the web. Scraping data is a great way to collect data for analysis, model building and all the other fun little tasks we as data scientists partake in. 

In this project we downloaded two csv files, one of article ids and country of origins along with the population of those countries. Subsequently, we used the Object Revision Evaluation Service (ORES) which offers machine learning as a service for wiki-projects. In this project we leveraged the ability of ORES to return the quality of the article. We passed in the article ids discussed above and returned was one of six quality categories. A final merge of this dataset to the merged dataset from above was then used for analysis. 

The goal of this project was to identify bias as it pertains to articles written about politicians. What I found interesting was that countries that have the highest number of articles written per population were all small, obscure countries while countries that are the most powerful and influential have the least number of articles written per population. This could be due to the large populations in these countries, but there is also likely bias in this data showing that these countries actually write less about politicians even though they are the most influential countries on the planet. 

---

### Codebook

* country: The country that the article was written about.
* article_name: The name of the article.
* revision_id: A unique id used by Wikimedia that links to this article. This is used in the ORES system to perform machine learning on. 
* article_quality: The predicted quality of the article returned by the ORES system.
* population: The population of the country the article was written about. 

ORES quality codes:
* FA - Featured article
* GA - Good article
* B - B-class article
* C - C-class article
* Start - Start-class article
* Stub - Stub-class article

---

### Data Source

The article data was uploaded to [figshare](https://figshare.com/articles/Untitled_Item/5513449) by Oliver Keyes and is under the CC BY 4.0 license meaning it is available for use this data as I see fit: share, copy or redistribute.

The population data came from [population reference bureau](http://www.prb.org/DataFinder/Topic/Rankings.aspx?ind=14). I could not find a license for this data, but I used it anyway because I like to live dangerously.  

The [ORES](https://www.mediawiki.org/wiki/ORES ) service is provided by the Wikimedia foundation for open use. 

---

### Reproducibility

Please follow along with the provided jupyter notebook. Each step is annotated and the code provided to reproduce the work I have completed. The code used in this project was R. 
