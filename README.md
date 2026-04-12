[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/_SA52CFJ)
# AI-CA2-2026
Python notebook template for students to use for CA2
# Ideal pipeline
## Idea:
#### Create an OCR and NLP program to categorize and extract fields from inputs

1. Image preprocessing:
- greyscale
- resize
- denoise
- thresholding/binarization
- edge detection
- contour detection to find the edge of receipt border
- perspective transformation

2. OCR extraction
- Tesseract on the cleaned image
- compare OCR before and after preprocessing

3. NLP / text processing
- tokenization
- stopword removal
- lemmatization or stemming
- keyword extraction
- entity extraction 
- lowercase
- remove noise/ special characters 
- Possible patterns for rules could be Date patterns, total patterns, currency patterns, item-price line patterns, VAT/TAX keywords, Payment keywords eg VISA or CASH etc.

4. Visual feature detection
- header area
- merchant info
- item list/ table area
- totals area
- maybe logo if visible
- qr or barcode maybe

5. Final output
- original image
- processed image
- ocr text
- cleaned NLP output
- extracted fields in JSON
- maybe pandas table of line items