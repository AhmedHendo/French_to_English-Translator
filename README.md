# French to English Translator

This project is a neural machine translation (NMT) system for translating French sentences into English. It explores two modern deep learning approaches for sequence-to-sequence translation:

- A Seq2Seq RNN model with a BiLSTM encoder, LSTM decoder, and additive attention
- A Transformer-based architecture implemented in PyTorch

The work is designed as an academic / learning project and includes notebook-based experiments, tokenizers, a prepared dataset, and a saved trained model checkpoint.

## Project overview

The goal of this project is to build a model that can take French text as input and generate English translations with reasonable quality using neural networks. The project uses a parallel French-English corpus and tokenization pipeline to train and evaluate translation models.

## Key features

- French-to-English translation
- Seq2Seq architecture with attention
- Transformer implementation from scratch
- Dataset loading and preprocessing
- Tokenizer-based encoding/decoding
- Model checkpoint saving for reuse
- Training and inference in Jupyter notebooks

## Repository structure

```text
French_to_English Translator/
├── README.md
├── seq2seq-rnn (3).ipynb
├── transformers.ipynb
├── transformer_en_fr.pth
└── resources-20251214T045019Z-3-001/
    └── resources/
        ├── parallel_en_fr_corpus/
        ├── tokenizer_fr/
        └── tokenizer_en/
```

## Technologies used

- Python
- PyTorch
- Hugging Face `datasets`
- Hugging Face `tokenizers`
- `transformers`
- NumPy
- Matplotlib / Seaborn
- NLTK
- Jupyter Notebook

## Dataset

The project uses a parallel French-English corpus stored under:

```text
resources-20251214T045019Z-3-001/resources/parallel_en_fr_corpus/
```

The tokenizers are also included and saved under:

```text
resources-20251214T045019Z-3-001/resources/tokenizer_fr/
resources-20251214T045019Z-3-001/resources/tokenizer_en/
```

## Model files

- `transformers.ipynb` contains the Transformer-based model training and translation workflow.
- `seq2seq-rnn (3).ipynb` contains the RNN-based sequence-to-sequence training pipeline.
- `transformer_en_fr.pth` is the saved trained Transformer model checkpoint.

## Setup

1. Clone the repository.
2. Open the project folder.
3. Install the required dependencies:

```bash
pip install torch torchvision torchaudio
pip install datasets tokenizers transformers tqdm matplotlib seaborn nltk
```

4. Open either notebook in Jupyter or VS Code Notebook mode.
5. Run the cells in order to:
   - load the dataset
   - load the tokenizers
   - train the model
   - translate sample French sentences

## Example workflow

A typical workflow is:

1. Load the French and English tokenizer files.
2. Load the parallel corpus.
3. Tokenize and pad the data.
4. Train the model on the French-English pairs.
5. Save the learned weights.
6. Use the translation function to convert a French sentence into English.

## Example usage

```python
sentence = "je suis fatigué aujourd'hui"
# Run the translation logic from the notebook
# Output should be an English sentence such as:
# "I am tired today"
```

## Notes

This repository is best suited for:

- educational machine translation experiments
- NLP coursework and projects
- learning about encoder-decoder architectures and Transformers
- testing and comparing sequence-to-sequence models

## License

This project does not appear to include a formal license file. If you plan to publish or share it publicly, you may want to add an appropriate open-source license such as MIT.

## Future improvements

- add a web interface for live translation
- compare model performance using BLEU score
- add command-line translation script
- clean up notebook code into reusable Python modules
- improve preprocessing and training pipeline quality

## Acknowledgements

This project was built as a practical deep learning and NLP experiment focused on machine translation between French and English.
