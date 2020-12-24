# ID-card-information-extraction-OCR

A model that extracts the information from an identity document using Pytessaract OCR and verifies it from the user-inputted data. It is most commonly used to verify the customer's identity in online banking and known as KYC Verification Process.

## Applications

It is most commonly used to verify the customer's identity in online banking and known as KYC Verification Process.


## Code Requirements 

The example code is in Python (version 3.6 or higher will work)

## Dependencies

1) import cv2
2) import imutils
3) import pytesseract
4) import numpy
5) import ftfy
6) import matplotlib.pyplot

## Install Tesseract

To install tesseract-OCR, follow this guide:
https://medium.com/@marioruizgonzalez.mx/how-install-tesseract-orc-and-pytesseract-on-windows-68f011ad8b9b

## Procedure

After installing all the dependencies and Tesseract on your system, clone the repo and run the 'Extraction and Verification.ipynb' notebok.

Our model will first ask the user his/her first name, last name, date of birth and Address then you'll need to input the image of ID card by changing the image path. After that, it will crop the image automatically and then it will apply some OpenCv tools on the image to make the image more clear and easy for text extraction. After that, model will apply Tesseract OCR to the ID card image and extract all the possible text from it. Then, it'll clean the text from junk/gibberish and compare the extraced information with the user inputted information, if matched it will save the verified information into a JSON file otherwise it will give message as not verified. 
