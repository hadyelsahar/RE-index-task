# RE-index-task
A repo for a small task to create an index of wikipedia pages. 


## Task Description

The task is to create a simple index for the provided document in `data` folder (~100 MB) . 

 - Clone the existing repository
 
 - create a python script that does: 
    - Parse the wikipedia xml sample document using a standard xml parser module in python or manually (if easier) 
    - Skip Wikipedia Categories i.e.: documents that are very short and start by `Category:`
    
    - create 3 output files in the `output` folder 
    - `doc.vocab` a CSV file contains unique words in the document and their counts it's columns formatted as below
        -  `wordid`  : generaetd id of the word
        -  `word`    : text of the word
        -  `word_count`: number of appearances of the word in all documents 
        -  `document_count` : number of documents that word appear in.
        
 - Tips and notes: 
  
    - Not to load the whole file in memory but rather read it line by line (or pick a xml parse that does that).  
    - The sample document is a bit noisy and many special characters are not skipped so it might be more convenient to use Regex to extract sentences 
    - Last thing you want is an unhandeled exception being thrown while your code is running.
    - To tokenize the document into a list of words you may want to use [NLTK word tokenizer](http://www.nltk.org/api/nltk.tokenize.html)
    - Use whatever will get you the task done.
    - Keep the code readable, commented and maintainable. 
     
     
 
     
 