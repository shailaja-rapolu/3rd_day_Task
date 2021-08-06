# 3rd_day_Task
1)Read a pdf in jupyter notebook
2)Do OCR
3)create a file

 

Read pdf in jupyter notebook
# importing required modules
import PyPDF2
 
# creating a pdf file object      =>we should give pdf name as File and have to upload that pdf in jupyter notebook
pdfFileObj = open('File.pdf', 'rb')
 
# creating a pdf reader object
pdfReader = PyPDF2.PdfFileReader(pdfFileObj)
 
# printing number of pages in pdf file
print(pdfReader.numPages)
 
# creating a page object
pageObj = pdfReader.getPage(0)
 
# extracting text from page
print(pageObj.extractText())
 
# closing the pdf file object
pdfFileObj.close()
refernce link:-https://www.geeksforgeeks.org/working-with-pdf-files-in-python/#:~:text=1%20Extracting%20text%20from%20PDF%20file%20Python%20Python,in%20...%205%20Adding%20watermark%20to%20PDF%20pages

 

# closing the pdf file object
pdfFileObj.close()
refernce link:-https://www.geeksforgeeks.org/working-with-pdf-files-in-python/#:~:text=1%20Extracting%20text%20from%20PDF%20file%20Python%20Python,in%20...%205%20Adding%20watermark%20to%20PDF%20pages

