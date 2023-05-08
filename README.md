**Jonathan Ng 113460607**

**Vinty Dong 113819690**

1. The original source for our code base came from the jupyter notebook for homework assignment 3. It is labelled in this repo as original_source.ipynb
2. original_source.ipynb was the only file we modified in order to create Notebook_1.ipynb and Notebook_2.ipynb. The functions we modified were tokenize_data() in the class DatasetLoader and the train() and eval() functions in the Trainer class.
3.
    i. Notebook_1.ipynb and Notebook_2.ipynb are responsible for finetuning DistilBert-base-uncased and training the classification layer respectively. Run the cells    from top to bottom and you should be able to train similar models. 
 
    ii. For Notebook_1.ipynb, change the variable c in tokenize_data() to choose how many training instances to train the model on
  
    iii. For Notebook_2.ipynb, options['model_name'] must be the path to the model you want to train the classification layer or evaluate on the tests.

    iv. Notebook_3.ipynb is responsible for automatically evaluating Flan-T5 on the same dataset we finetuned our models on and is code written by us. 

    v. In order to evaluate different Flan-T5 sizes, change the variable ```name```  to the model name with appropriate size. 

    vi. In order to evaluate few-shot or zero-shot, set the variable ```FEW_SHOT``` to ```True``` or ```False```. 

    vii. In order to change the prompt to include (or not include) the phrase "Choose the best option", set the variable ```CHOOSE_BEST_OPTION``` to ```True``` or ```False```.  

4. All of our models can be found in ```models.zip```. The dataset we used is https://huggingface.co/datasets/math_qa The models named MC have an additional classification layer trained used for the final multiple choice task.

5. Since we used automatic evaluation, all of our prompts were created by the script in Notebook_3.ipynb

6. We trained our models using Pytorch and CUDA and loaded our datasets. The software requirements were the same as the ones required for the homework assignments.
