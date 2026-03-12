# LSTM_Code_Summary
# Virtual environment setup
It is recommended to run this project through a Python virtual environment.

```bash
python3.12 -m venv .venv
source .venv/bin/activate
```
# Dependency installation
Next, install the required dependencies within your virtural environment.

Dependencies for training:
```bash
pip install numpy==1.26.4 torch==2.2.0 transformers==4.46.0 sentencepieve=0.1.99 tqdm==4.65
```
NOTE: The dependencies for training were installed directly into the venv via the terminal.


Dependencies for evaluation:
```bash
pip install nltk, pandas, bert-score, sentence-transformers
```

# Running data extraction
To execute data extraction and splitting, open GenAI_A2_Data_Extraction.ipynb with your preffered IDE and run all cells. All generated files will be output to the working directory.

# Running train/validation/test

To train, validate, and evaluaet test data, open assignment_2_LSTM.ipynb your preffered IDE and run all cells. All generated files will be output to the working directory.
# Ouput locations
Results from the created test set were pushed to the repository. The lstm_small_codet5.pt file can be created by running the block for training the model, but the file was too big to commit to GitHub.
# Hyper-parameters tuned
batch_size = 20

max_len = 120 (max generated summary length)

hidden_layer = 512

eval_steps = 200

num_epochs = 100

patience = 10
