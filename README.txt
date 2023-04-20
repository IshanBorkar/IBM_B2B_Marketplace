This code used PyPDF2 which is a free and open-source pure-python PDF library capable of splitting, merging , cropping, and transforming the pages of PDF files.
Packages used:
nltk
PyPDF2

Pseudocode:
1. In this step we capture the URLs that are present in the GFK dataset.
2. Store the URLs from the excel in a separate excel file.
3. Use the above excel sheet and download the PDFs using urllib and urlretrieve.
4. Use PyPDF2 package to read a pdf file and extract the text from it.
5. We use certain functions like decontract and removing the repeated words to clean the text.
6. Save the cleaned text into a text file.
7. Iterate the steps 3,4,5,6 across all the PDFs present in a directory.
8. If the URL is empty, return the empty string.