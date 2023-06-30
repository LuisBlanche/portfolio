
## Public sector: scraping of thousands of public documents and training of a Named Entity Recognition Model


### Context 

Government-accorded loans issued to social housing projects by municipalities are subject to mandatory publication in reports made available on the respective local government websites. The purpose of this initiative was to compile data pertaining to housing loans across different regions by scraping relevant details from online resources to construct a comprehensive repository of lending statistics for analysis and future decision-making considerations regarding improvements in the loan market for housing.


### Methodology 

To gather information, we began by leveraging the Google Search API to uncover potentially relevant municipalities and the websites associated with them. Subsequently, we manually reviewed our compiled list before commencing extensive website crawling, combing them for any conceivably pertinent documentation. These retrieved files were subsequently parsed programmatically, culminating in a structured archive. Throughout this process, we employed cloud-based solutions to facilitate the annotation task on a distributed scale. Our efforts ultimately led us to train powerful machine learning models capable of automatically mining essential insights. Ultimately, these automated tools enabled us to rapidly collect vast amounts of data without sacrificing accuracy. In doing so, we have established a robust system ready for deployment at minimal cost while providing easy accessibility to users. 
![docanno annotation](../assets/img/Quantmetry/docanno.png)


### Tools
- Python : spacy, scrapy, gsearch
- Docanno 
- VSCode for development

### My involvment 
As a technical consultant overseeing this venture, I was teemed up with a strategist consultant but still handled most of the communication with the customer. I was responsible for the whole development from start to finish. Additionally, I assumed responsibility for guiding the annotation group, guaranteeing harmonious labeling throughout our joint enterprise

### Results and achievements

- Efficiently harvesting numerous digital records from targeted municipal sites through advanced programming techniques.
- Ensuring accurate markups through integration of remote crowd annotation software.
- Developing highly effective natural language processing systems to yield critical details required by your organization in monitoring industry trends and assessing competitive dynamics."


