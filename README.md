# BERT-Finetuning-for-Medical-Dataset
In this project, we pre-trained and fine-tuned BERT, RoBERTa and GPT2 from the HuggingFace Library to classify medical dataset. The specifics are mentioned in the experiment section. The correspoding Jupyter Notebooks can be found in this repo.


## Dataset
The datasets used are allpatients, zreddit, smalldataset, Reddit All, Twitter. 

## Experiments

Out domain: 
|Experiments |Model |Continue pretraining |Finetune |Regression (severity) /Classification|
|-----------|------|------------------|----------|----------------------|
|Experiment 1 |Reddit dataset|----|-|dataset1/dataset2/Twitter|
|Experiment 2|Bert-RoBERTa-GPT|zReddit Patients only(without labels)|-|dataset1/dataset2/Twitter|
|Experiment 3|Bert-RoBERTa-GPT|Reddit All Patients (without labels)|-|dataset1/dataset2/Twitter|
|Experiment 4|Bert-RoBERTa-GPT|Twitter|-|dataset1/dataset2|
|Experiment 5|Bert-RoBERTa-GPT|-|zReddit  dataset (sent via email)|dataset1/dataset2/Twitter|
|Experiment 6|Bert-RoBERTa-GPT|-|AllReddit Patients and control only (i will include control text and labels)|dataset1/dataset2/Twitter|
|Experiment 7|Bert-RoBERTa-GPT|-|Twitter|dataset1/dataset2/|

In Domain: 
|Experiments |Model |Finetune |Classification|
|-----------|------|------------------|----------------------|
|Experiment 1|Bert|zReddit (patients and control)|zReddit|
|Experiment 2|RoBERTa|zReddit (patients and control)|zReddit|
|Experiment 3|GPT2|zReddit(patients and control)|zReddit |
|Experiment 4|Bert|Reddit All(patients and control)|Reddit All |
|Experiment 5|RoBERTa|Reddit All (patients and control)|Reddit All |
|Experiment 6|GPT2|Reddit All (patients and control)|Reddit All |

## Model Architectures:
 
![Screenshot from 2021-10-28 22-25-11](https://user-images.githubusercontent.com/69421538/139301223-f889fb38-0225-4491-99e1-bed2279850d6.png)
   BERT
   
   

![The-RoBERTa-model-architecture ppm](https://user-images.githubusercontent.com/69421538/139301483-fc102062-735a-41ab-be1b-da9407989aec.png)
    RoBERTa



![Decoder-Only-Architecture-used-by-GPT-2 ppm, width="400"](https://user-images.githubusercontent.com/69421538/139301262-53702de1-90aa-49f4-9fc6-bb9496fcce70.png)
    GPT2

## Results
![Screenshot from 2021-10-28 22-12-18](https://user-images.githubusercontent.com/69421538/139300799-4cf40b48-8ee5-482d-ae5f-73bc4a510804.png)

![Screenshot from 2021-10-28 22-12-45](https://user-images.githubusercontent.com/69421538/139300843-26c44670-cb70-4b65-831b-2bad0100d3d3.png)

*Due to computational constrains some models couldn't be trained by us using Google Colab. Hence, the results for these are left blank.*
