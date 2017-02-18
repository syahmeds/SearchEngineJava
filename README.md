# SearchEngineJava
Information Retrieval project - TF-IDF Search Engine: 
Moonshot - A moonshot, in a technology context, is an ambitious, exploratory and ground-breaking project undertaken without any expectation of near-term profitability or benefit and also, perhaps, without a full investigation of potential risks and benefits. 
Google has adopted the term moonshot for its most innovative projects, many of which come out of the Google X, the company's semi-secret lab. Our version of a moonshot is to try and emulate Google's most used product, Google Search!

So here, we have customized the search screen to include an optional field called 'domain name', where the homepage of any website can be entered, for example, www.ku.edu or www.espn.com. The user needs to enter a search query and a homepage and click 'Search', then the homepage will be crawled and the TF-IDF index will be built based on it. The list of domains entered will be stored in a separate file to prevent rework in generation of index. 

After parsing, the HTML documents from the webpages will be parsed in a local directory and tokenized, passing them through a stop-word filter and stemming the words; hereafter referred to as ‘terms’. Next, we plan to index the parsed terms and build an inverted index mapping the terms to documents along with the ‘term frequency’ and ‘document frequency’ of the words.

Finally, the search engine uses the ‘Vector-space model’ where the term-weights are assigned and document vectors are calculated. The incoming query from the user is also parsed through the tokenizer to remove stop words and stem the words. The query vector is to be calculated and using the dot product formula, the similarity between the query vector and candidate document vectors (with query frequency >= 1) is calculated and the documents are ranked in order of similarity. There's a 'user-feedback' component added in the output screen to re-rank the documents based on user input.
