# XY_Recurrent_Glioma
## textract install(we recommend install it under python2 env)
  it should be install from source:
  ```
    git clone https://github.com/deanmalmgren/textract.git
    cd textract
    python setup.py install
  ```  
  if you pip install this error may occur:
  ```
    Failed building wheel for pocketsphinx
    Running setup.py clean for pocketsphinx
    Successfully built textract python-pptx docx2txt xlrd EbookLib
    Failed to build pocketsphinx
    requests 2.18.4 has requirement chardet<3.1.0,>=3.0.2, but you'll have chardet 2.3.0 which is incompatible.
  ```
some of the Word Document may can't be read by textract, then we can try to use other software trans doc to txt, then read it.
```
  libreoffice --headless --convert-to txt:text --outdir "/tmp/outdir" "/path/to/file.doc"
```
