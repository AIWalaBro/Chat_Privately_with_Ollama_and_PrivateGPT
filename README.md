# Chat_Privately_with_Ollama_and_PrivateGPT


#### Step 1: Step a Virtual Environment
```bash
conda create -p venv_privategpt python=3.10 -y
conda activate venv_privategpt/
```

#### Step 2: Install the Requirements
```bash
pip install -r requirements.txt
```

#### Step 3: Pull the models (if you already have models loaded in Ollama, then not required)
#### Make sure to have Ollama running on your system from https://ollama.ai
```bash
ollama pull mistral
```

#### Step 4: put your files in the source_documents folder after making a directory
```bash
mkdir source_documents
```

### Step5: run the ingest.py file; on window after running it will look like
Creating new vectorstore
Loading documents from source_documents
Loading new documents: 100%|██████████████████████| 1/1 [00:12<00:00, 12.35s/it]
Loaded 186 new documents from source_documents
Split into 676 chunks of text (max. 500 tokens each)
Creating embeddings. May take some minutes...
Ingestion complete! You can now run privateGPT.py to query your documents

#### Step 6: Run this command 
```bash
python privateGPT.py
```

### Play with your docs
Enter a query: How many locations does WeWork have?


### Try with a different model:
```bash
ollama pull llama2:13b
MODEL=llama2:13b python privateGPT.py
```

## Add more files

Put any and all your files into the `source_documents` directory

The supported extensions are:

- `.csv`: CSV,
- `.docx`: Word Document,
- `.doc`: Word Document,
- `.enex`: EverNote,
- `.eml`: Email,
- `.epub`: EPub,
- `.html`: HTML File,
- `.md`: Markdown,
- `.msg`: Outlook Message,
- `.odt`: Open Document Text,
- `.pdf`: Portable Document Format (PDF),
- `.pptx` : PowerPoint Document,
- `.ppt` : PowerPoint Document,
- `.txt`: Text file (UTF-8),

### Ollama
This repo brings numerous use cases from the Open Source Ollama

### Step 1
Go Ahead to https://ollama.ai/ and download the set up file

### Step 2
Install and Start the Software

### Step 3
Clone my Entire Repo on your local device using the command
```bash
git clone https://github.com/AIWalaBro/Chat_Privately_with_Ollama_and_PrivateGPT.git
```
### Step 4
The Repo has numerous working case as separate Folders. You can work on any folder for testing various use cases


