# MillRightMegaVDocs
For Documentation developed as Open Source for the MillRight Mega V CNC machine

If you want to make a pdf make sure to install https://www.tug.org/mactex/

To install REstructuredText(assumes python3 and Pip3 are present)
```
goto https://www.latex-project.org/get/ and install the apprpriate version

brew cask install mactex
brew install sphinx-doc

fix path
echo 'export PATH="/usr/local/opt/sphinx-doc/bin:$PATH"' >> ~/.zshrc

then:
pip3 install docutil rst2pdf pdfTex 

To build html:
```
source ./venv/bin/activate
make html
open build/html/index.html
```

To build pdf:
```
source ./venv/bin/activate
make latexpdf
open 
```
