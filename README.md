# TribridNU

## How to Install Jupyter Notebook (https://jupyter.org/install)
- get pip (if needed) by entering these two lines on the command prompt:
```
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
```
```
python get-pip.py
```
- Install Jupyter Notebook with pip on the command prompt:
```
pip install notebook
```
To access Jupyter Notebook, type the following on the command prompt:
```
jupyter notebook
```

## How to Install and use Tribrid_pos (https://github.com/karmaresearch/tribrid)
- Download tribrid_master from the link above
- Install python3 here: https://www.python.org/downloads/
- Make sure to have the following packages and their versions installed (or install the necessary ones by the errors Tribrid_pos gives):
<details><summary>Packages List (long)</summary>
<p>
argon2-cffi                       21.3.0
  
argon2-cffi-bindings              21.2.0
  
asttokens                         2.0.5
  
attrs                             21.4.0
  
backcall                          0.2.0
  
beautifulsoup4                    4.11.1
  
bleach                            5.0.0
  
blis                              0.7.7
  
boto3                             1.24.5
  
botocore                          1.27.5
  
catalogue                         2.0.7
  
certifi                           2022.5.18.1
  
cffi                              1.15.0
  
charset-normalizer                2.0.12
  
click                             8.1.3
  
colorama                          0.4.4
  
cuda-python                       11.7.0
  
cymem                             2.0.6
  
Cython                            0.29.30
  
debugpy                           1.6.0
  
decorator                         5.1.1
  
defusedxml                        0.7.1
  
en-core-web-sm                    3.3.0
  
entrypoints                       0.4
  
executing                         0.8.3
  
fastjsonschema                    2.15.3
  
filelock                          3.7.1
  
huggingface-hub                   0.7.0
  
idna                              3.3
  
ipykernel                         6.15.0
  
ipython                           8.4.0
  
ipython-genutils                  0.2.0
  
jedi                              0.18.1
  
Jinja2                            3.1.2
  
jmespath                          1.0.0
  
joblib                            1.1.0
  
jsonschema                        4.6.0
  
jupyter-client                    7.3.4
  
jupyter-contrib-core              0.3.3
  
jupyter-contrib-nbextensions      0.5.1
  
jupyter-core                      4.10.0
  
jupyter-highlight-selected-word   0.2.0
  
jupyter-latex-envs                1.4.6
  
jupyter-nbextensions-configurator 0.4.1
  
jupyterlab-pygments               0.2.2
  
langcodes                         3.3.0
  
lxml                              4.9.0
  
MarkupSafe                        2.1.1
  
matplotlib-inline                 0.1.3
  
mistune                           0.8.4
  
murmurhash                        1.0.7
  
nbclient                          0.6.4
  
nbconvert                         6.5.0
  
nbformat                          5.4.0
  
nest-asyncio                      1.5.5
  
notebook                          6.4.12
  
numpy                             1.22.4
  
packaging                         21.3
  
pandas                            1.4.2
  
pandocfilters                     1.5.0
  
parso                             0.8.3
  
pathy                             0.6.1
  
pickleshare                       0.7.5
  
Pillow                            9.1.1
  
preshed                           3.0.6
  
prometheus-client                 0.14.1
  
prompt-toolkit                    3.0.29
  
psutil                            5.9.1
  
pure-eval                         0.2.2
  
pycparser                         2.21
  
pydantic                          1.8.2
  
Pygments                          2.12.0
  
pyparsing                         3.0.9
  
pyrsistent                        0.18.1
  
python-dateutil                   2.8.2
  
pytorch-pretrained-bert           0.6.2
  
pytz                              2022.1
  
pywin32                           304
  
pywinpty                          2.0.5
  
PyYAML                            6.0
  
pyzmq                             23.1.0
  
regex                             2022.6.2
  
requests                          2.28.0
  
s3transfer                        0.6.0
  
scikit-learn                      1.1.1
  
scipy                             1.8.1
  
Send2Trash                        1.8.0
  
six                               1.16.0
  
sklearn                           0.0
  
smart-open                        5.2.1
  
soupsieve                         2.3.2.post1
  
spacy                             3.3.1
  
spacy-legacy                      3.0.9
  
spacy-loggers                     1.0.2
  
srsly                             2.4.3
  
stack-data                        0.3.0
  
terminado                         0.15.0
  
thinc                             8.0.17
  
threadpoolctl                     3.1.0
  
tinycss2                          1.1.1
  
tokenizers                        0.12.1
  
torch                             1.11.0+cu115
  
torchaudio                        0.11.0+cu113
  
torchvision                       0.12.0+cu113
  
tornado                           6.1
  
tqdm                              4.64.0
  
traitlets                         5.3.0
  
transformers                      4.19.3
  
typer                             0.4.1
  
typing_extensions                 4.2.0
  
urllib3                           1.26.9
  
wasabi                            0.9.1
  
wcwidth                           0.2.5
  
webencodings                      0.5.1
  
</p>
</details>

- Fill the model, dataset, and output path in Tribrid_pos.py
- Then, run it on the command prompt:
```
python3 -u Tribrid_pos.py
```
## Downloading the PHEME-dataset
Download the dataset from here: https://drive.google.com/drive/folders/15Fz7CcAsSNBBExsk4x86lYG3V4_Orifv?usp=sharing


## How to run the experiments
### Data Preperation
- Download all files from the repo
- Make sure all the prerequisites above have been met
- Run Jupyter Notebook by typing the following into the command prompt:
```
jupyter notebook
```
- Open the desired experiment from the TribridNU folder in Jupyter notebook.
- In the second cell, after all imports, there will be 4 or 5 empty variables with a lot of comments around them. Fill the variables with the guide of the comments.
- Run every cells up until the "Tribrid_pos for stance classification" header (some cells might take a while)
- The database will be created at the earlier filled "export_destination" folder.

### Stance Classifying
- Open command prompt
- Navigate to tribrid_pos
- Make sure that tribrid_pos uses the newly created database
- Run the following command:
```
python3 -u tribrid_pos.py
```
- Wait for Tribrid_pos to finish
- Return to the same notebook

**NOTE**: Sometimes, pandas creates a .tsv file, which causes errors with Tribrid_pos. To circumvent this problem, take the following steps:
1. Open Google Sheets (https://docs.google.com/spreadsheets/u/0/?usp=direct_url)
2. Create a Blank sheet (or open any sheet)
3. Click on File -> Import
4. Upload the faulty .tsv file
5. Click on "Import Data"
6. On the .tsv sheet, click on File -> Download -> Tab-seperated values (.tsv)
7. Replace the old .tsv file with the new one to use for Tribrid_pos.

### Weighing (only on Pheme-rumor dataset)
- Run everything up until the header "Choosing the weighing system"
- In the cell below, choose the weighing system by inputting the corresponding dataframe name into the "finaldf" variable.

### Analysing
- The rest of the notebook can be run until the end and analysed.
