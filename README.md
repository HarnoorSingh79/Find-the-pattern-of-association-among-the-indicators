# Find-the-pattern-of-association-among-the-indicators
Using NARM along with genetic algorithm to find the pattern of association among the indicators of dataset. 

For proper report, please go to  https://harnoorsingh2.blogspot.com/2023/01/using-narm-along-with-genetic-algorithm.html

### Objective

Finding a pattern of association among the indicators of the given dataset using numerical association rules which are generated via genetic algorithm

### Outcome -   

[![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgC1Sv7z-dzR0me6CJR6AhPOpk1TIwNxOprM55YHnngQAFVlZoTXTU2KtY6qW2cCHH1uKEnw8JHt-qE1sylcdOhZj52YYKBQe7v_vOgYaGfj3O-fdOlBuH99NAVCgTTCaVuIDbvoDKqsQsOvXY-YycHVqdbE-UjCypxUM9E54IN9JfaMmLlbpsEs8i80w/s320/viz(3).png)](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgC1Sv7z-dzR0me6CJR6AhPOpk1TIwNxOprM55YHnngQAFVlZoTXTU2KtY6qW2cCHH1uKEnw8JHt-qE1sylcdOhZj52YYKBQe7v_vOgYaGfj3O-fdOlBuH99NAVCgTTCaVuIDbvoDKqsQsOvXY-YycHVqdbE-UjCypxUM9E54IN9JfaMmLlbpsEs8i80w/s1000/viz(3).png)  

The round circle in the center represents all the rules with 100% confidence and 100% support.  
The circles coming out of the main circle is representing the antecedent in the rules.  
The size of each circle is representing its degree i.e. how many rules it is part of.  
Lastly, the circle originated from antecedent are consequent. Their sizes are also representing their degree  

[![](https://blogger.googleusercontent.com/img/a/AVvXsEgHb6pxs_q5CRy7bFCdP741vY-ck9aTB6aJgs0TRyOilwR25yEuKSc8JAbxtrKq_t9paAbH8hFek6K4VrhJRr7sgoqK_0K751wg6yXnPBA3Wg2j7tglO8ieaaweegASm1E4Pzk0EDYLB1fG4tEpfil8aaqHNBGFz9HCR4y_ulEi2XsfrL01vGleHDxcYA=w400-h240)](https://blogger.googleusercontent.com/img/a/AVvXsEgHb6pxs_q5CRy7bFCdP741vY-ck9aTB6aJgs0TRyOilwR25yEuKSc8JAbxtrKq_t9paAbH8hFek6K4VrhJRr7sgoqK_0K751wg6yXnPBA3Wg2j7tglO8ieaaweegASm1E4Pzk0EDYLB1fG4tEpfil8aaqHNBGFz9HCR4y_ulEi2XsfrL01vGleHDxcYA)

This visualization represents all the top rules (Rules with the highest support and confidence).  
Each arc is representing a rule. they are sorted high to low starting from right to left.  
As clear from the diagram, Most rule has I1, I3, I5, I7, AND I8 asantecedent  
  
### Note

This project is similar to the Research paper that I have co-authored. You can check out the paper [here](https://link.springer.com/article/10.1007/s10639-022-11265-4)

You can check out the GitHub repo. [here](https://github.com/HarnoorSingh79/Find-the-pattern-of-association-among-the-indicators)
