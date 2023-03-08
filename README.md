# ImgComposer
the official repo for ImgComposer


# Overview

Here we provide the implementation of ImgComposer, *ImgComposer: Disentangling and Composing Images \\in Text-Guided Image Generation Using Latent Diffusion Models*, along with a minimal execution example (on the animal dataset and face expression datasets). 

The repository is organized  as follows:
- under each dataset folder, for example `animal/`
	- `data/`: contains all training data for each experiment setting; 
	- there are three scripts for different purposes, for example
		- `wildcard_SD_V1_5_fine_tune_unet_animal.ipynb`: the fine-tune script for UNet;
		- `wildcard_SD_V1_5_freezed_lookup_emb_animal_ipynb.ipynb`: the looking embedding optimization script for our specifically designed templates and wildcards;
		- `inference_SD_V1_5_wildcard_animal.ipynb`: the inference script that can be directly run to generate images as needed using pre-trained models, which have been saved in a dedicated Dropbox link mentioned below due to its large size. 

*Note: since the two pre-trained models are independently trained, to generate face expression related disentanglement images on animal-based pre-trained models will not return the images of a special form of face expression.*

The notebooks contains the implementation and experiment code of `ImgComposer` on all six datasets mentioned previously, and all notebooks can be directly ran on Google colab after putting the needed datasets and models under the corresponding Google drive directories. For example, saving the animal datasets under `/content/drive/MyDrive/SDV1_5_wildcard_animal/data_fine_tune_v5/` and `/content/drive/MyDrive/SDV1_5_wildcard_facial_expression/data_token_embedding/`.  

The colab code will auto-complete other folder creation process, if you want to train your own models. Otherwise, you can save the pre-tained models for direct inference. The models should be saved directly under the parent directories. For example, saving the pre-trained model trained on the animal dataset under `/content/drive/MyDrive/SDV1_5_wildcard_animal/` and the model trained on the face expression dataset under `/content/drive/MyDrive/SDV1_5_wildcard_facial_expression/`. 

![Experimental results](https://github.com/theseainc/ImgComposer/figs/ICCVResults.png?raw=true)


# Additional Notes 

Due to the large size of the preprocessed datasets and pre-trained models, we save them in a dropbox, which can be accessed via the following link: https://www.dropbox.com/scl/fo/hdjef3n5gjqwpd6w8sbh6/h?dl=0&rlkey=so3as3dajmbijkj5xzbm97nzx

The Dropbox is organized as follows: 
- under each dataset folder, for example `animal/`
	- 

