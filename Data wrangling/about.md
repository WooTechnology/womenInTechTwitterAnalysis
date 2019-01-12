## Step:2  Wrangling of datasets
<strong>Data wrangling, sometimes referred to as data munging, is the process of transforming and mapping data from one "raw" data form into another format with the intent of making it more appropriate and valuable for a variety of downstream purposes such as analytics. </strong>

# Steps to wrangle data

## Step 1
In your terminal/command line, install the PDFTables Python library with:
<br>
<strong> pip install git+https://github.com/pdftables/python-pdftables-api.git </strong> <br>
Or if you'd prefer to install it manually, you can download it from python-pdftables-api then install it with:
<br>
<strong>python setup.py install </strong>

## Step 2
Create a new Python script then add the following code:
<br>
### Code
import pdftables_api     // Importing the required library <br>
c = pdftables_api.Client('my-api-key') <br>
c.xlsx('input.pdf', 'output')  <br>
<strong>//replace c.xlsx with c.csv to convert to CSV</strong>

### Now, you'll need to make the following changes to the script:
- Replace my-api-key with your PDFTables API key from <strong> https://pdftables.com/ </strong> or <strong> https://github.com/pdftables </strong> .<br>
- Replace input.pdf with the PDF you would like to convert. <br>
- Replace output with the name you'd like to give the converted document. <br>
- Now, save your finished script as convert-pdf.py in the same directory as the PDF document you want to convert.

## Step 3
Open your command line/terminal and change your directory (e.g.<strong> cd C:/Users/pranjal</strong>) to the folder you saved your convert-pdf.py script and PDF in, then run the following command:
<br> 
<strong>python convert-pdf.py</strong>
<br>
To find your converted spreadsheet, navigate to the folder in your file explorer and hey presto, you've converted a PDF to Excel or CSV with Python!

