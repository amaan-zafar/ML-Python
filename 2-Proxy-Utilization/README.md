 6-NLP
# NLP Pipeline

Attached are 10 JSON files (https://stackabuse.com/reading-and-writing-json-files-in-python-with-pandas) which contain entire web page data of 10 different web pages

You need to load these files data in Pandas and then perform the following tasks from NLP Pipeline :

1. Data Cleansing     - Remove any HTML data tags , strip spaces , punctuations and any other garbaage element present. Utilize Regular Expressions (Regex) for same
2. Stop Words removal - Remove any stop words present in this data and *extend* stopwords corpus incase you find some other junk words present as well due to web scraping
3. Tokenization - Split the remaining words into tokens , and tokenize all the text data
4. Stemming - Perform stemming on the tokenized text data
5. Lemmatization - Perform Lemmatization on stemmed data
6. Bigram formation - Pair most frequently occuring words together , via bigram formation

Your *output* should a Pandas dataframe with 2 columns - *Raw_Text , Processed_Text*

- **Raw Text** should contain each file text in raw form( i.e. as it is)  
- **Processed_Text** should contain the same text after going through the NLP Pipeline as mentioned above.

Since there are 10 files , so there would be 10 records in this dataframe

#### References

- NLTK Library - https://www.nltk.org/
- https://www.analyticsvidhya.com/blog/2020/11/text-cleaning-nltk-library/

