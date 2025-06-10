# Synthetic-Tabular-Data
This repository contains the Machine Learning Models used and developed for my thesis on Synthetic Tabular Data Generation

There is a Jupiter Notebook for every model with easy to run code.

All eModels notebooks are ready to run independent Notebooks. TabDDPM, tVAE and ctGAN require extra some modules and setup apart from their corresponing Jupiter Notebooks. There are steps for uploading your desired csv dataset and some basic necessary preprocessing in every notebook.

# eGAN
GAN model used to generate data from embedded datasets. It contains the Embedding Model and a Wasserstein based GAN

# eVAE
The same Embedding Model as eGAN followed by a VAE based model to train on embedded datasets

# EDDPM
The same Embedded Model as eGAN and eVAe followed by a Denoising Diffusion Probabilistic Model. 

# ctGAN and tVae
These two models have their model setup in CTGAN_Synthesizer.ipynb and tVAE_Synthesizer.ipynb respectively. There is a code cell in each that specifies to upload the given transformer.py and data_sampler.py modules that are used by the models. Both implementations follow the algorithms of the 'Modeling Tabular data using Conditional GAN' (https://arxiv.org/abs/1907.00503) and their code form https://github.com/sdv-dev/CTGAN .

# TabDDPM
This is the original TabDDPM model found in here: https://github.com/rotot0/tab-ddpm . The TabDDPM.ipynb is an adaptation of the TabDDPM_Training_and_Extraction.ipynb notebook from the https://github.com/javiagu13/TabDDPM_easyRun/tree/main repo. It is an easy run notebook that requires the files of the folder to be uploaded in your Drive. It accesses the generated samples and automatically constructs and saves the generated dataset ready for use as 'final_df'.
