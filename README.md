# Enhanced Translation of Biomedical Texts via Named Entity Embeddings

## Models
Transfer learning was performed using MarianMT "Helsinki-NLP/opus-mt-en-zh" on biomedical data. An embedding layer was added on top 

Pretrained transformer model from:
https://huggingface.co/docs/transformers/en/model_doc/marian
https://arxiv.org/abs/1804.00344

~~Only the 3 model weights described in the `Data_266_Paper.pdf` are included in the `final-3-models-weights.zip` file. All intermediate files are not in this repo. If you are interested, please reach out to aaronlin@ischool.berkeley.edu~~
Model weights were too big to push, please reach out to aaronlin@ischool.berkeley.edu if you would like to have them.

## Notebooks
Final models are the current project, intial models are primary based around the old objective which was to incorporate dynamic knowledge selection via knowledge graphs.

Note that the BERT Scores in the final models notebooks are calculated incorrectly, so all values were recomputed in `en_to_zh_true.ipynb`. The most updated metrics for **Model I** as described in the paper can be found in `en_to_zh_true_final.ipynb`.

## Dataset
The training data is from:
https://github.com/boxiangliu/ParaMed

Embedding is from:
https://github.com/ncbi-nlp/BioSentVec

Biomedical NER in English from:
https://huggingface.co/venkatd/BioMed_NER