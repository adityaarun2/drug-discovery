# Generative Tensorial Reinforcement Learning (GENTRL) 

This repository contains an implementation of the GENTRL model, with a training example on the MOSES dataset. I extended the reinforcement learning pipeline by introducing two additional reward functions—one that promotes molecular diversity and another that enforces the presence of a specified substructure. Additionally, the repository includes 3 pre-trained reinforcement learning models, each corresponding to one of the reward functions.

To run the training procedure,
1. [Install RDKit](https://www.rdkit.org/docs/Install.html) to process molecules
2. Install GENTRL model: `python setup.py install`
3. Install MOSES from the [repository](https://github.com/molecularsets/moses)
4. Run the [pretrain.ipynb](./examples/pretrain.ipynb) to train an autoencoder
5. Run the [train_rl.ipynb](./examples/train_rl.ipynb) to optimize a reward function
