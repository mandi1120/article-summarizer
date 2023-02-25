# Amanda Hanway - Web Mining & Applied Natural Language Processing, Module 7
- Final Project: Article Summarizer
- Date: 12/4/22

## Overview:  
This program was created as a final assignment for a master's course at NWMSU, Web Mining & Applied NLP.  

### Project Description   
- This program uses [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) to scrape text from a website, and performs sentiment analysis using [spaCy](https://spacy.io/).  

### Original Data Source  
- Bogost, Ian. "The Madness of Twitter: People just can’t stop tweeting about all the tweets they see." The Atlantic, 22 Nov. 2022, www.theatlantic.com/technology/archive/2022/11/elon-musk-twitter-bad-habit/672249/.

### Program Overview     
- Article-summarizer.ipynb
    - This program first scrapes the text of an article from a webpage, and writes the text to an html output file.
    - It then loads the text into a trained spaCy pipeline to generate a polarity score, and finds the most frequent words and lemmas.
    - Next, it generates a score for each sentence based on the count of important words and lemmas in the sentence, and plots the scores in a histogram.
    - Then, the program creates an article summary comprised of the highest-scored (most important) sentences.
    - Lastly, it finds the polarity score for the article summary.
    
### Completed Program    
- [View completed Jupyter notebook](https://github.com/mandi1120/article-summarizer/blob/master/article-summarizer.ipynb)

### Output Files    
- [View article output](https://raw.githubusercontent.com/mandi1120/article-summarizer/master/elon-musk-twitter-bad-habit.html)

## Prerequisites:
- Libraries:
    - Standard libraries required:  
        - collections 
        - pickle
    - Additional libraries required: 
        - beautifulsoup4 
        - requests 
        - spacy
        - spacytextblob
    - Installation instructions:  
        - beautifulsoup4: https://anaconda.org/anaconda/beautifulsoup4 
        - requests: https://requests.readthedocs.io/en/latest/user/install/ 
        - spacy: https://spacy.io/usage
        - spacytextblob: https://spacy.io/universe/project/spacy-textblob
```
conda install -c anaconda beautifulsoup4
conda install -c conda-forge requests
conda install -c conda-forge spacy
pip install spacytextblob
```
## Assignment
Complete the tasks in the Python Notebook in this repository.
Make sure to add and push the pkl or text file of your scraped html (this is specified in the notebook)
### Rubric
* (Question 1) Article html stored in separate file that is committed and pushed: 1 pt
* (Question 2) Polarity score printed with an appropriate label: 1 pt
* (Question 2) Number of sentences printed: 1 pt
* (Question 3) Correct (or equivalent in the case of multiple tokens with same frequency) tokens printed: 1 pt
* (Question 4) Correct (or equivalent in the case of multiple lemmas with same frequency) lemmas printed: 1 pt
* (Question 5) Histogram shown with appropriate labelling: 1 pt
* (Question 6) Histogram shown with appropriate labelling: 1 pt
* (Question 7) Cutoff score seems appropriate given histograms: 2 pts (1/score)
* (Question 8) Summary contains a shortened version of the article (less than half the number of sentences): 1 pt
* (Question 8) Summary sentences are in the same order as they appeared in the original article: 1 pt
* (Question 9) Polarity score printed with an appropriate label: 1 pt
* (Question 9) Number of sentences printed: 1 pt
* (Question 10) Summary contains a shortened version of the article (less than half the number of sentences): 1 pt
* (Question 10) Summary sentences are in the same order as they appeared in the original article: 1 pt
* (Question 11) Polarity score printed with an appropriate label: 1 pt
* (Question 11) Number of sentences printed: 1 pt
* (Question 12) Thoughtful answer based on reported polarity scores: 1 pt
* (Question 13) Thoughtful answer based on summaries: 1 pt

