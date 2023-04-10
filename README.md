## Pytorch clean code 

An advice given to me by a PhD student studying at CMU with regards to being a good deep learning research is to first be able to learn how to write good code in deep learning

Important aspects for clean code
1. Reproducibility 

This is a repository documenting clean code guidelines for developing pytorch models

Links to repository with clean code:
- Pytorch documentation: https://pytorch.org/docs/stable/index.html
- Pytorch template: https://github.com/victoresque/pytorch-template  

### Building datasets 
Dataset template card: https://github.com/huggingface/datasets/blob/main/templates/README_guide.md

### creating new AI models for research
##### folders for a new project 
1. config folder: Contains a set of yaml files for your dataset configurations 
-   examples 
    - GLIP: https://github.com/microsoft/GLIP/tree/main 
2. 

##### tips
1. use distributed data parallelism: https://pytorch.org/tutorials/intermediate/ddp_tutorial.html#initialize-ddp-with-torch-distributed-run-torchrun 
- to date, command is torchrun --nnodes=2 --nproc_per_node=8
2. 

### Dealing with secrets: 
If you have secrets such as API keys to use in your repository, you can create a .env file and place it under your gitignore file, you should also provide an env.example file to provide a template for your original env file
https://dev.to/edgar_montano/how-to-setup-env-in-python-4a83#:~:text=How%20to%20setup%20a%20.env%20file%201%201.To,file%20using%20the%20following%20format%3A%20...%20More%20items

Steps: 
1. pip install python-dotenv file 
2. create a .env file and a .env.example file 
3. Add the .env to your gitignore 
4. 
```
from dotenv import load_dotenv, find_dotenv
load_dotenv(find_dotenv())
```

### Styling your outputs 
#### Coloring command line outputs 
1. Colorama 
    ```
    from colorama import Fore 
    print(Fore.RED) + "text message here in red"
    ```
    examples:
    - Auto-GPT: https://github.com/Torantulino/Auto-GPT/blob/master/scripts/main.py