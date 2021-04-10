# Earnings_Call_Analysis
Corporate earnings calls contain a wealth of information for a publicly traded company. They can unveil a company's strategic priorities, business objectives, economic head-and-tail-winds, and other information relevant to company operations. 

One drawback of the earnings call is that listening to one requires an investment of time (most are at least half an hour) and attention (listening carefully to mentally sift through the jargon and distill the often small amount of useful information). What if you could save time and brainpower by analyzing an earnings call's transcript rather than listening live? That's the idea behind this repository. 

The code here leverages Natural Language Tool Kit (NLTK), and a few other common Python Libraries, to identify the most frequent 1, 2, and 3-word phrases in a corporate earnings call. The idea is that the most commonly mentioned words and phrases in a company’s earnings call can give us some insight into what are the hot topics in the business.

The architecture is a simple Jupyter Notebook that reads in the earnings call transcript from a TXT file. For the sake of writing and testing the code, I used Nike’s March 2021 earnings call. 

One call-out worth mentioning is the treatment of STOPWORDS in this code. I built this code with two sets of STOPWORDS: the first is the original set of ~180 stopwords from NLTK.corpus, and the second is a specific list of words I removed after noticing that a few “immaterial” words were bubbling to the top. If you want to use this framework to analyze other earnings calls, I recommend modifying the second stopword list to fit your earning’s call. That list is called more_stop_words in this code. 

Happy coding! 
-Adam
