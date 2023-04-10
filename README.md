### Pytorch clean code 

An advice given to me by a PhD student studying at CMU with regards to being a good deep learning research is to first be able to learn how to write good code in deep learning

Important aspects for clean code
1. Reproducibility 

This is a repository documenting clean code guidelines for developing pytorch models

Links to repository with clean code:
- Pytorch documentation: https://pytorch.org/docs/stable/index.html
- Pytorch template: https://github.com/victoresque/pytorch-template  

#### Building datasets 
Dataset template card: https://github.com/huggingface/datasets/blob/main/templates/README_guide.md

#### creating new AI models for research
##### folders for a new project 
1. config folder: Contains a set of yaml files for your dataset configurations 
-   examples 
    - GLIP: https://github.com/microsoft/GLIP/tree/main 
2. 

##### tips
1. use distributed data parallelism: https://pytorch.org/tutorials/intermediate/ddp_tutorial.html#initialize-ddp-with-torch-distributed-run-torchrun 
- to date, command is torchrun --nnodes=2 --nproc_per_node=8
2. 