# Symba-GSOC-Task

## Common task 1:-
#### Cleaned the dataframe for getting appropriate values
#### Used separate tokenization for encoder and decoder 
#### In encoder we encode float sequences using 3 bits , sign , mantissa and exponent ,(see the notebook Data_with_tokenization/Encoder_tokenizer(Symbolic).ipynb)


#### In decoder we use Direct polish notation to encode the sequences , first we convert the given expression into sympy expression and replace the present variables into variables like v1, v2 ... because we don't need to learn the name of the variable and it would be easier for the model to learn that way 

## Common task 2:- 
#### I trained a common seq2seq with 2 encoder layers and 4 decoder layers (Training/seq2seq_transformer.ipynb)
#### The tokenized input into the encoder is passed through an embedder and no positional embedding is used in encoder as mentioned in ""End-to-end symbolic regression with transformers ("https://arxiv.org/abs/2204.10532")
#### The encoder-decoder is trained using cross entropy loss 

## Specific Task 1:- 
#### ("Training/Evolved_transformer.ipynb")
#### Evolutionary and Transformer Models for Symbolic Regression("https://ml4sci.org/gsoc/2024/proposal_SYMBA3.html")
#### The application of evolved transformer into the project using the implementation("https://github.com/moon23k/Transformer_Variants/blob/main/model/evolved.py")

## Specific Task 2:- 
#### ("Training/Longformer.ipynb")
#### Transformer Models for Symbolic Calculations of Squared Amplitudes in HEP("https://ml4sci.org/gsoc/2024/proposal_SYMBA1.html")
#### For the model specialized in long sequences i used LongFormer , a model that combines a local windowed attention with a task motivated global attention using Hugging Face()
