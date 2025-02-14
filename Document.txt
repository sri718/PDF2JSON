PDF to JSON Converter Documentation  

Overview:

- This project extracts text and images from a PDF file and converts the extracted content into JSON format.  
- The process includes text extraction, metadata retrieval, and image extraction from the PDF.  

Workflow:
 
1. Mount Google Drive to access PDF files. 
 
2. Install required dependencies like marker-pdf, torch, sympy, and PyMuPDF. 
 
3. Import necessary libraries for processing PDF files.  

4. Convert PDF to Markdown:  
   - Use PdfConverter from marker.converters.pdf to extract text from the PDF.  
   - Save the extracted text as a Markdown file. 
 
5. Extract images:  
   - Use PyMuPDF (fitz) to extract images from the PDF.  
   - Save extracted images in an output directory.  

6. Extract metadata:  
   - Retrieve metadata such as number of pages, creation date, and last modification date.  

7. Convert Markdown to JSON:  
   - Parse the Markdown text and organize it into a structured JSON format.  
   - Capture section headings, descriptions, and image references.  

8. Save output files:  
   - Save extracted text as output(md).md.  
   - Save structured JSON as output(json).json.  
   - Compress extracted images into a ZIP file.  

9. Download processed files:  
   - Download Markdown, JSON, and ZIP files for local storage.  

Output Files:
 
- output(md).md - Extracted text from the PDF in Markdown format.  
- output(json).json - Structured JSON representation of the document.  
- images.zip - Compressed folder containing extracted images.  

Conclusion:
  
- This script provides a streamlined process for converting PDFs into structured JSON format.  
- The output includes text, metadata, and images, enabling easy data extraction for further processing or analysis.  
