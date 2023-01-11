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

