# java-information-retrieval-project
This project is a demonstration for a information retrieval tool. 

Textbank is the folder containing the medline query. </br>
These files are passed through the following steps: </br>
1. Stopwords remover based on a stoplist file. It generates a .stp file. </br>
2. Stemmer using the proter algorithym. It generates a .stem file </br>
3. A tfidf generation algorythim that stores the values in a inverted file. 
&nbsp&nbsp;;The inverted file has a custom JSON data structure. 
`{`</br>
 &nbsp;&nbsp;&nbsp;`"word":{`</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`"1(document frequency)":{`</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`"doc1.stp":0.01(tfidf values)`</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `}`</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `}`</br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `}`</br>
4.A cosine value generation and document retrieval tool.
&nbsp;&nbsp;These are the top three results for the following query: </br>  `the` `crystallin` `len` `vertebr` `includ` `human`</br></br></br>
&nbsp; `Document Name : doc72.stp and cosine value : 0.357`</br>
&nbsp; `Document Name : doc500.stp and cosine value : 0.284`</br>
&nbsp; `Document Name : doc965.stp and cosine value : 0.265`</br>

5. A precision and recall calculation tool. 
    These are the graphs showing the values of the precision and recall for the first query results of the medline collection. 
    
    ![alt text](http://samerdiab.net/fileshare/download.php?id=21&token=EX6vinkYQR2ALS35vrteXRRpq5A7kN0O"Logo Title Text 1")