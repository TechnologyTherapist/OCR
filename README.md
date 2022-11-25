# OCR
Internship project
When collecting data for the text mining process or looking for other references, we often find sources in the form of images. For example, if we are going to analyze a word in pdf format, the file instead contains an image of text. This certainly makes it difficult for data processing. One solution to this problem is that we can use Optical Character Recognition (OCR).

OCR is a technology for recognizing text in images, such as scanned documents and photos. One of the OCR tools that are often used is Tesseract. Tesseract is an optical character recognition engine for various operating systems. It was originally developed by Hewlett-Packard as proprietary software. Later Google took over development.

Currently Tesseract is running well on the Windows, macOS, and Linux platforms. Tesseract supports Unicode (UTF-8) and supports more than 100 languages. In this article we will start with the Tesseract OCR installation process, and test the extraction of text in images.

The first step is to install the Tesseract. In order to use the Tesseract library, we first need to install it on our system. If you’re using Ubuntu, you can simply use apt-get to install Tesseract OCR:

sudo apt-get install tesseract-ocr
For macOS users, we’ll be using Homebrew to install Tesseract.

brew install tesseract
For Windows, please see Tesseract documentation. Let’s begin by getting pytesseract installed.

$ pip install pytesseract

Lets Start
We’ll start by developing the Flask back-end layer to serve the results of the OCR engine. From there you can just hit the endpoint and serve the results to the end user in the manner that suits you. All of this is covered in detail by the tutorial. We’ll also add a bit of back-end code to generate an HTML form as well as the front-end code to consume the API. This will not be covered by the tutorial, but you will have access to the code.

we need to make a class using pytesseract to intake and read images in ocr.py
Building a CLI Tool for Your New OCR Engine in cli.py
Back to the Server in app.py

Run your app:
$ python app.py
