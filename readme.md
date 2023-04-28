### Method Name ###
fine tuning BERT-base-uncased model

### Sentence pair encoder ###
It’s a bidirectional transformer pretrained using a combination of masked language modeling objective and next sentence prediction on a large corpus comprising the Toronto Book Corpus and Wikipedia.
Bi-encoder BERT base model
Used BERT-base tokenizer from Hugging face

- What type of encoder (LSTM, Transformer, etc.)
Transformer

- Is it based on a pre-trained model (BERT-large? RoBERTa-large-SNLI? BART-large-MNLI?) or completely trained from scratch by yourself (then how do you chracterize the words and aggregate them into sentence representations)?
A Pre-trained model using Hugging Face Auto Text classification library.

### Training & Development ###
Optimizer - Adam
Learning Rate - 0.00025
Batch Size - 8 (Since Colab crashes with higher batch sizes and also Accuracy drops significantly at higher batch sizes)
Termination - Early Stopping (tracking accuracies epoch by epoch)


### Other methods ###
Did you try other methods than the submitted one?
Yes, Roberta Base, Pure LSTM

### Packages ###
List the key python packages you have used in this assignment.
TensorFlow
PyTorch
Pandas
