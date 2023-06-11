# Prediction of Lysine Succinylation Site using Protein Language Model
Our method uses a protein Language Model to extract features from protein sequences and CNN combined with ANN to predict succinylation. In this paper, we used two protein Language Models which are ProtBert and ProtT5. The protein sequences are fed to the model to develop a different set of protein embeddings. The embeddings from different pLMs were found to have negligible similarity. The embeddings are fed to 1D-CNN Neural networks and the outputs from the networks are stacked and ANN is trained on top of that. The stacking ensemble has improved the performance of our proposed architecture. On comparison using benchmarking dataset, our method was comparable with other state of the art models on nearly every metric.

## Train Pipeline

### Dataset
- The required dataset are in the csv_folder

### Generate Embeddings from Sequence
- To generate embeddings, you can run generate_embeddings_from_sequence.ipynb which will generate embeddings for you. You can choose ProtT5 or ProtBert embeddings or even use other protein language model

### Training
- We have three training models.
    - 1D-CNN ProtBert model
    - 1D-CNN ProtT5 model
    - Combined (ProtBert+ProtT5) model
- Run these model during training your datasets

### Visualization
- We have included additional file tsne plot to visualize the model. Run this code to better know how your model is performing.

### Testing
- Finally test the model for evaluation. 

## Authors
- [@SubinMaharjan](https://github.com/SubinMaharjan)


## Acknowledgements

We would like to express our sincere gratitude to Asst. Prof Lokhnath Regmi, our project supervisor, for his constant guidance and precious encouragement. We would like to earnestly acknowledge the support, guidance and valuable time given by Mr. Suresh Pokhrel and Asst. Prof Dr. Dukka KC. We are also very grateful to Department of Electronics and Computer Engineering, Pulchowk Campus for providing us with such a splendid opportunity to do the project.
