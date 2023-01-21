# Find-the-pattern-of-association-among-the-indicators
Using NARM along with genetic algorithm to find the pattern of association among the indicators of dataset

### Objective

Finding a pattern of association among the indicators of the given dataset using numerical association rules which are generated via genetic algorithm

### Data collection and preparation

For this project, we will use the SDG 5 dataset of the United Nations. This Dataset is cleaned and pre-processed. All the parameters of this dataset are renamed to I1, I2, I3, and so on. for ease of doing data analysis.  
[![](https://blogger.googleusercontent.com/img/a/AVvXsEg75PMRn1gURi9qLITiuBRFYlcy0JWwqxO_US9mgACVK6RHTu1vkRLw8OY4YbyJ9IFDV_26euBvIW7PXjp9kahv8J_qxBEx6e-QU5H2pdt8O9_R-PTVBEUIyN3rRlx2xPaW4uImdYaa1Y3clZcNDRHu2BX-an76sWE8Qbj_cqPhVv8FmwuA86-7Lxd3ew=w640-h86)](https://blogger.googleusercontent.com/img/a/AVvXsEg75PMRn1gURi9qLITiuBRFYlcy0JWwqxO_US9mgACVK6RHTu1vkRLw8OY4YbyJ9IFDV_26euBvIW7PXjp9kahv8J_qxBEx6e-QU5H2pdt8O9_R-PTVBEUIyN3rRlx2xPaW4uImdYaa1Y3clZcNDRHu2BX-an76sWE8Qbj_cqPhVv8FmwuA86-7Lxd3ew)  
### EDA

1. Understanding the makeup of the data  
[![](https://blogger.googleusercontent.com/img/a/AVvXsEia8NSw4WMpeZQVQOHQQZWSf9GlSx0lbyokQcMKMihqxuizB1GAaZE-tBIOi8BrOWuYlRNuLB0rgV-UV7v2RqFaVCSvxsTDrVFneO2IrvpVUU8tqqg6FRWaJBREw9lurGh4tD6-Jm3xm7kz8PIhIlihWuhvaLlex_-Ut3jiCzUv1URfxQ_Aj0brI4gCVA=w640-h168)](https://blogger.googleusercontent.com/img/a/AVvXsEia8NSw4WMpeZQVQOHQQZWSf9GlSx0lbyokQcMKMihqxuizB1GAaZE-tBIOi8BrOWuYlRNuLB0rgV-UV7v2RqFaVCSvxsTDrVFneO2IrvpVUU8tqqg6FRWaJBREw9lurGh4tD6-Jm3xm7kz8PIhIlihWuhvaLlex_-Ut3jiCzUv1URfxQ_Aj0brI4gCVA)  
  
2. Understanding the Correlation between different parameters  
[![](https://blogger.googleusercontent.com/img/a/AVvXsEgwO2lxlp4nfiLzLTq8BfBIjTsYFeWHiFuwJ-WuGaSfOz4DRH4HcWKnHMsoU_HQxsg_DSKUt3CWlHXew3i8YYqAzrGC-PwM6_1niRYe7EsRV-moKvBKLI9uqIs_Ya80BP45Fu3GCib7N2O-PDpFbBX2dW8oRyIXoeaRGpCXGgJoDDVrIpK4Ir8OcanbrA=w623-h179)](https://blogger.googleusercontent.com/img/a/AVvXsEgwO2lxlp4nfiLzLTq8BfBIjTsYFeWHiFuwJ-WuGaSfOz4DRH4HcWKnHMsoU_HQxsg_DSKUt3CWlHXew3i8YYqAzrGC-PwM6_1niRYe7EsRV-moKvBKLI9uqIs_Ya80BP45Fu3GCib7N2O-PDpFbBX2dW8oRyIXoeaRGpCXGgJoDDVrIpK4Ir8OcanbrA)  
  
  
3. Box Plots

[![](https://blogger.googleusercontent.com/img/a/AVvXsEjWAN1hzWQf7gO-U8hwgQQDKGfzcQjA1Zh-VwdQ-Pl0ISJ1b_m2NAn4UBV8zBt9v8t9f-MoMRPezLEIb8cAK4uMbpccczRhSOo7CzldIVe7v-vD4TJOfW9BOqyfcsXaNpZQbQdnQCcy_fPs4utoWocv84_p__PI7mhJuh7EdGFRbE79ijnEPwZYlDQY9w)](https://blogger.googleusercontent.com/img/a/AVvXsEjWAN1hzWQf7gO-U8hwgQQDKGfzcQjA1Zh-VwdQ-Pl0ISJ1b_m2NAn4UBV8zBt9v8t9f-MoMRPezLEIb8cAK4uMbpccczRhSOo7CzldIVe7v-vD4TJOfW9BOqyfcsXaNpZQbQdnQCcy_fPs4utoWocv84_p__PI7mhJuh7EdGFRbE79ijnEPwZYlDQY9w)  
  
  
[![](https://blogger.googleusercontent.com/img/a/AVvXsEgazwMni4SqORAwnUQ8T1WRSKTI_VM9EICghCCFRs-82nC-CWaxowiSZm3A1gEmUBUa7gVxdeLYMhE_i8Z5E5HNxSOgnMOgCrh9RJv2U8aOh5LHPJQSh3vgflWcaim1pdYbPQDowwZj_ScUC9s8u_L17GuQsm3pVxQ31bG7o5ehcM9OjK8MR906tZ_Vfw)](https://blogger.googleusercontent.com/img/a/AVvXsEgazwMni4SqORAwnUQ8T1WRSKTI_VM9EICghCCFRs-82nC-CWaxowiSZm3A1gEmUBUa7gVxdeLYMhE_i8Z5E5HNxSOgnMOgCrh9RJv2U8aOh5LHPJQSh3vgflWcaim1pdYbPQDowwZj_ScUC9s8u_L17GuQsm3pVxQ31bG7o5ehcM9OjK8MR906tZ_Vfw)  
[![](https://blogger.googleusercontent.com/img/a/AVvXsEiIkCALNFbi7jxHceoLn2cZEy_YH1sLG-si66h4_7xHKu2ZxdWJnjU__kStvc-BQbSz934DZhUHiwfsIN0dnIscOli6kor1s-86CUBZ0fGy8SFUjLz4XTkHE0FgcTv1QtXsDlIW0XnzXzhkjniCWVVBGFgdjXxTqF7zfvBG6Ins1Flyvd6eI65kMVbzCQ)](https://blogger.googleusercontent.com/img/a/AVvXsEiIkCALNFbi7jxHceoLn2cZEy_YH1sLG-si66h4_7xHKu2ZxdWJnjU__kStvc-BQbSz934DZhUHiwfsIN0dnIscOli6kor1s-86CUBZ0fGy8SFUjLz4XTkHE0FgcTv1QtXsDlIW0XnzXzhkjniCWVVBGFgdjXxTqF7zfvBG6Ins1Flyvd6eI65kMVbzCQ)  
[![](https://blogger.googleusercontent.com/img/a/AVvXsEibcjFGiVaUCpa1r-JPTOD4HnZFBBQGUd80JXaYl8UXfSwzq2PaWzGgwxvl-IWtgSrJtXqfnA8-Aohbsje5gthj-Dd6oHbQSKDybmgbzyWL4bua2UrkHdHRVH9ozAxTZ2T7rO0HEITj_aslblK6bbS3FQMQ4HYEJoy9BWTXhW0V9ksP4hjmO1r8YetFVQ)](https://blogger.googleusercontent.com/img/a/AVvXsEibcjFGiVaUCpa1r-JPTOD4HnZFBBQGUd80JXaYl8UXfSwzq2PaWzGgwxvl-IWtgSrJtXqfnA8-Aohbsje5gthj-Dd6oHbQSKDybmgbzyWL4bua2UrkHdHRVH9ozAxTZ2T7rO0HEITj_aslblK6bbS3FQMQ4HYEJoy9BWTXhW0V9ksP4hjmO1r8YetFVQ)  
  


### Numerical rules generation using genetic algorithm

  
For this purpose, we will use [quantminer](https://github.com/QuantMiner/QuantMiner)  
After the rules are generated, I copy them to a Text file. This is what the text file looks like -   
1. support = 34 (91%) , confidence = 100 % : I1 in [12.1; 115.2] --&gt; I2 in [0.0; 958.0]2. support = 35 (94%) , confidence = 100 % : I2 in [0.0; 941.0] --&gt; I1 in [4.1; 177.8]3. support = 31 (83%) , confidence = 100 % : I1 in [17.2; 110.4] --&gt; I3 in [0.53; 0.96]4. support = 35 (94%) , confidence = 100 % : I3 in [0.53; 0.95] --&gt; I1 in [4.1; 177.8]  
  
After that, I use python code to transfer that data from a text file to a CSV file, and here is what it looks like.  
[](https://blogger.googleusercontent.com/img/a/AVvXsEiLZ8NsBFq1Lj4vTjHdPXS0XzSy3aYOMQvDt-4lJ3gDuEQb1d8QKj4W9dERnuvZJpAOgQAkbaHQ6ekK7j7cjWExsu_cLtPRFl3jArm5dfitto-_nSigWreZ-uE2N2QAxTF_85LeZwLZ0GKBVZKZfDDtPlnOc4O___OFJRh2jtdkfl_ytXt2RMIh7ydkyw)[](https://blogger.googleusercontent.com/img/a/AVvXsEiLZ8NsBFq1Lj4vTjHdPXS0XzSy3aYOMQvDt-4lJ3gDuEQb1d8QKj4W9dERnuvZJpAOgQAkbaHQ6ekK7j7cjWExsu_cLtPRFl3jArm5dfitto-_nSigWreZ-uE2N2QAxTF_85LeZwLZ0GKBVZKZfDDtPlnOc4O___OFJRh2jtdkfl_ytXt2RMIh7ydkyw)[![](https://blogger.googleusercontent.com/img/a/AVvXsEhcfCenpWizjyfyTE4_vrK8BNGH04uB18pY373-uacFv6HNuXW1X--bq_shmw0lOMQ_ikE9BxBBxY9MLA6pPOLNa-Ir-IQmxM1SBz3v6WLolto5BOruUDR-GaYXgCoKbIzhDW_osLo9ucn1Ep9p-CoI03JgXF5VAdN6PxDqI0DQrGRvDrmh2PddXx6FlA=w640-h172)](https://blogger.googleusercontent.com/img/a/AVvXsEhcfCenpWizjyfyTE4_vrK8BNGH04uB18pY373-uacFv6HNuXW1X--bq_shmw0lOMQ_ikE9BxBBxY9MLA6pPOLNa-Ir-IQmxM1SBz3v6WLolto5BOruUDR-GaYXgCoKbIzhDW_osLo9ucn1Ep9p-CoI03JgXF5VAdN6PxDqI0DQrGRvDrmh2PddXx6FlA)  
### Result / Outcome

#### Number of Rules  
[![](https://blogger.googleusercontent.com/img/a/AVvXsEjjPYoIXvALiRjEzT1KCQ-ALBSa8psXRKFNRAAJOZdYq-Fx67nbEZGhhSr7gjgFtcdjkfXXZZAb0gDl4onbfRpj-MTbmffVxQMOqDRjrxDHeUYgz064uWt9n05tTOAIWvQ-iZsl2w_agutIfCe6ikn85RWShcDCug6h51_iNW_c0FaMuFmkK-EYY4V2cA=w400-h124)](https://blogger.googleusercontent.com/img/a/AVvXsEjjPYoIXvALiRjEzT1KCQ-ALBSa8psXRKFNRAAJOZdYq-Fx67nbEZGhhSr7gjgFtcdjkfXXZZAb0gDl4onbfRpj-MTbmffVxQMOqDRjrxDHeUYgz064uWt9n05tTOAIWvQ-iZsl2w_agutIfCe6ikn85RWShcDCug6h51_iNW_c0FaMuFmkK-EYY4V2cA)  
  
  

#### Vizulations -   

[![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgC1Sv7z-dzR0me6CJR6AhPOpk1TIwNxOprM55YHnngQAFVlZoTXTU2KtY6qW2cCHH1uKEnw8JHt-qE1sylcdOhZj52YYKBQe7v_vOgYaGfj3O-fdOlBuH99NAVCgTTCaVuIDbvoDKqsQsOvXY-YycHVqdbE-UjCypxUM9E54IN9JfaMmLlbpsEs8i80w/s320/viz(3).png)](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgC1Sv7z-dzR0me6CJR6AhPOpk1TIwNxOprM55YHnngQAFVlZoTXTU2KtY6qW2cCHH1uKEnw8JHt-qE1sylcdOhZj52YYKBQe7v_vOgYaGfj3O-fdOlBuH99NAVCgTTCaVuIDbvoDKqsQsOvXY-YycHVqdbE-UjCypxUM9E54IN9JfaMmLlbpsEs8i80w/s1000/viz(3).png)  

<br />
The round circle in the center represents all the rules with 100% confidence and 100% support.  
The circles coming out of the main circle is representing the antecedent in the rules.  
The size of each circle is representing its degree i.e. how many rules it is part of.  
Lastly, the circle originated from antecedent are consequent. Their sizes are also representing their degree  
<br />

[![](https://blogger.googleusercontent.com/img/a/AVvXsEgHb6pxs_q5CRy7bFCdP741vY-ck9aTB6aJgs0TRyOilwR25yEuKSc8JAbxtrKq_t9paAbH8hFek6K4VrhJRr7sgoqK_0K751wg6yXnPBA3Wg2j7tglO8ieaaweegASm1E4Pzk0EDYLB1fG4tEpfil8aaqHNBGFz9HCR4y_ulEi2XsfrL01vGleHDxcYA=w400-h240)](https://blogger.googleusercontent.com/img/a/AVvXsEgHb6pxs_q5CRy7bFCdP741vY-ck9aTB6aJgs0TRyOilwR25yEuKSc8JAbxtrKq_t9paAbH8hFek6K4VrhJRr7sgoqK_0K751wg6yXnPBA3Wg2j7tglO8ieaaweegASm1E4Pzk0EDYLB1fG4tEpfil8aaqHNBGFz9HCR4y_ulEi2XsfrL01vGleHDxcYA)

<br />
This visualization represents all the top rules (Rules with the highest support and confidence).  
Each arc is representing a rule. they are sorted (high to low) from left to right.  
As clear from the diagram, Most rule has I1, I3, I5, I7, AND I8 asantecedent  
  
### Note

This project is similar to the Research paper that I have co-authored. You can check out the paper [here](https://link.springer.com/article/10.1007/s10639-022-11265-4)
