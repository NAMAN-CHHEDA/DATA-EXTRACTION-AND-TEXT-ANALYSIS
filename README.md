# DATA-EXTRACTION-AND-TEXT-ANALYSIS
The provided Python code performs web scraping and sentiment analysis on textual data extracted from a set of URLs. Here's a summary of the key functionalities:

1. **Web Scraping:**
   - Utilizes the `requests` library to fetch HTML content from a given URL.
   - Applies the `BeautifulSoup` library to parse and navigate the HTML structure.
   - Extracts the article title and main text content from the HTML.

2. **Text Analysis:**
   - Employs the `nltk` library for natural language processing and sentiment analysis.
   - Defines a function (`analyze_text`) to calculate various text metrics, such as sentiment scores, average sentence length, percentage of complex words, FOG index, and more.
   - Uses the Sentiment Intensity Analyzer from `nltk.sentiment` to obtain sentiment scores.

3. **Input Reading:**
   - Reads input data from an Excel file (`Input.xlsx`) using the `pandas` library.

4. **Iterative Processing:**
   - Iterates over each row in the input DataFrame, extracting and analyzing text data from the corresponding URLs.

5. **Output Creation:**
   - Stores the results, including URL_ID, title, article text, and various text metrics, into lists.

6. **Output DataFrame:**
   - Creates a new DataFrame (`df_output`) to organize the processed information.

7. **Output Saving:**
   - Writes the output DataFrame to an Excel file (`Output.xlsx`) using the `to_excel` function.

In summary, the code automates the extraction and analysis of textual content from URLs, providing sentiment analysis and various text-related metrics. The results are stored in a structured format for further analysis or reporting.
