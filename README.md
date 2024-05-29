
# TEXT ANALYSIS

The main aim of this project is extract textual data from article's URL and perform text analysis to compute variables




## Libraries:

Load the necessary libraries

- Beautifulsoup4 - For web scraping to extract data from HTML content.
- Requests - For making HTTP requests to fetch web page content.
- Nltk - For natural language processing tasks such as tokenization.
- Openpyxl - For reading and writing Excel files.
- Re - For regular expression operations.
- String - string operations

## Data Extraction

Libraries like BeautifulSoup, Selenium or Scrapy are used to extract text from web pages. 

**Fetching the Web Page:**
- Using the requests library one can fetch the content of the URL.
- You need to specify a User-Agent header to mimic a browser request.

**Parsing the HTML:**

- Here I have used BeautifulSoup to parse the HTML content.
- Now, Identify and extract the relevant sections of the webpage. 
- After inspecting the webpage, I have found that the paragraphs of interest are within the class td-post-content. This class name is used to locate and extract the text content.

**Saving Extracted Text:**

- Finally save the extracted text into a text file named after the URL_ID. 

## Data Cleaning

- Data cleaning and tokenization is performed using the clean_and_tokenize function to tokenize text into words, remove punctuation, convert words to lowercase, and filter out custom stop words. 
- Stop words, which are common and less informative words, are loaded from various predefined files to ensure that only meaningful words remain in the processed text.

## Data Analysis 

The compute_variables function performs text analysis to derive various metrics. 
```
1) Positive and negative scores are calculated by matching words in the text against predefined dictionaries. 

2) The polarity score assesses the overall sentiment, while the subjectivity score indicates the extent of personal opinion in the text. 

3) Readability is evaluated using the Gunning Fog Index, which considers the average sentence length and the percentage of complex words. 

4) Additional metrics include the average number of words per sentence, complex word count, overall word count, syllable count per word, personal pronouns count, and average word length.

```
These calculations provide a comprehensive analysis of the text's sentiment, readability, and linguistic characteristics.



## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)


## To Run the script

```
1) Go to Google Colab/Jupyter Notebook.
2) Click on New Notebook/New ipykernel.
3) Copy and paste the Python script into a cell in the notebook.
4) Run the cell by pressing Shift + Enter.

```





## Dependencies:

You can install these dependencies using pip command in Jupyter notebook/google Colab or terminal.

```
pip install beautifulsoup4
pip install requests
pip install nltk
pip install openpyxl
```

## Run Locally

Clone the project

```bash
  git clone https://link-to-project
```

Go to the project directory

```bash
  cd my-project
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```


## License

[MIT](https://choosealicense.com/licenses/mit/)


## Contact

For any queries, contact - pranaswic2022@gmail.com

