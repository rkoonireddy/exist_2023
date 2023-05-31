# exist_2023
sEXIST task for CLEF 2023

This repository contains code to use EXIST2023 task from CLEF. 

More information about the task can be found here:
http://nlp.uned.es/exist2023/

My code acquired the following (own best) poisitions in the task:
You can also find the details from the website above.
The data given is tweet data of English and Spanish languages.

- Task 1 is a binary classification task 
- Task 2 is a multi label classification task
- Task 3 is a multi class classification task

| Submission Name | Task Type				|Sub Task 				|Rank 						|
|-----------------|-----------------|-----------------|-----------------|
| roh-neil_2 			|Task 1						| Soft -Soft ALL  |49|
| roh-neil_1 			|Task 1						| Hard -Hard ALL	|**4**|
| roh-neil_1 			|Task 1						| Hard -Soft ALL	|13|
|-----------------|-----------------|-----------------|-----------------|
| roh-neil_1 			|Task 2						| Soft -Soft ALL  |23|
| roh-neil_1 			|Task 2						| Hard -Hard ALL	|**2**|
| roh-neil_1 			|Task 2						| Hard -Soft ALL	|12|
|-----------------|-----------------|-----------------|-----------------|
| roh-neil_1 			|Task 3						| Soft -Soft ALL  |7|
| roh-neil_1 			|Task 3						| Hard -Hard ALL	|**1**|
| roh-neil_1 			|Task 3						| Hard -Soft ALL	|13|

The given code achieves good results on hard labels consistently but fail to perform well on soft labels. One reason could be not using the right logistic loss for the direct probabilities.

Key Information is that I use a twitter trained XLM-Roberta_large model from Hugging Face library called sdadas/xlm-roberta-large-twitter (which can be found here: https://huggingface.co/sdadas/xlm-roberta-large-twitter)
