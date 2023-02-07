# HebrewDatasets  

Every comment in this dataset tagged by two independent taggers.
Comments without agreement - tagged by additional 3 independent taggers(total of 5)
Comments with agreement - we took ~10% of the sentences and tagged them again with another tagger

## Dataset fields  
* id
* text - the comment text
* tag - final tag for the sentence. ש,ח,נ for negative, positive and neutral.
* category - the category of the sentence. economy, news or sport.
* class - class code for the tagged sentence: 
  * A: consensus of 3 of 3 or 5 of 5  
  * B1: consensus of 2 of 2
  * B2: consensus of 2 of 3
  * C1: consensus of 4 of 5
  * C2: consensus of 3 of 5 
* total_tags - how many taggers tagged this sentence
* selected_tag - how many taggers choose the selected tag
* polarity - number between 0-1, indicate how many taggers choose positive or negative. polarity = (num_of_positives + num_of_negatives) / total_tags  

## Statistics  

The dataset contains 75,152 tagged sentences from 3 categories: economy, news(mostly politics) and sport.

tags count by category:  

| category | count |  
| :--- | :--- |  
| economy  |  40923 |  
| news     | 24905 |  
| sport    | 9323 |  

tags count by class:  

| class | count |  
| :--- | :--- |  
| a  |  2545 |  
| b1     | 60692 |  
| b2    | 5474 |  
| c1 | 1632 |
| c2 | 4808 |

tags count by sentiment and category:  
| category |  tag |  cnt |  
| :--- | :--- |  :--- |
|ECONOMY|   ח |       4164|  
|  |        נ|       5973 |  
|  |        ש|      30786 |  
|NEWS|      ח |       1147 |  
|   |       נ|        956 |  
|    |      ש|      22802 |  
|sport|     ח |       1671 |  
|     |     נ|        399 |  
|      |    ש|       7253 |  


## Sources  
The sentences in this dataset collected from comments posted on news websites. Crawler downloaded all the comments, and then crowd members rewrite the comments, and filter out invalid comments.  
All the  sentences were annotated by crowd members(2-5 annotators) to sentiment: positive, negative or neutral (they also marked invalid sentences, as second pass).  

