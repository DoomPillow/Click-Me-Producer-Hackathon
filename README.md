# URL Grabber
<p align="center">
  <img src="https://user-images.githubusercontent.com/90370987/227833445-3f30c4b8-1c90-4ac7-a1ae-113352d2156d.png" width=560.7 height=151.9>
</p>

# Overview

Welcome to Click Me! This is a project that utilizes a fine-tuned Mobilenet Model and Pytesseract to recognize URL overlays in LinkedIn Courses and extract relevant metadata such as timestamp, the overlay itself, and the bounding box of the overlay (the coordinates on the screen where the overlay appears). The primary objective of this project is to automate the process of gathering essential metadata to create clickable UI elements in courses. In addition, the extracted data can be used to check the status of URLs provided in LinkedIn courses and generate PDFs containing the URLs from a given course.

# Dependencies

Here are the necessary packages to run the provided notebook:
- OpenCV - `pip install opencv-python`
- NumPy - `pip install numpy`
- Pillow - `pip install pillow`
- TensorFlow - `pip install tensorflow`
- PyTesseract - `pip install pytesseract`
- Requests - `pip install requests`
- ReportLab - `pip install reportlab`
- Beautiful Soup - `pip install beautifulsoup4`


# Examples

Below is a visual representation of the URL recognition, generated using data from the json file:<br/><br/>
<p align="center">
  
  <img src="https://user-images.githubusercontent.com/90370987/227855933-194c98ba-ec43-4362-9054-5ae4d1bb4c9e.jpg" width=700 height=400>
</p>


<br/><br/>  
Below is an example pdf generated using data from the json file. The title and header are both customizable parameters.
It's worth noting that as of this current version, generating pdfs course-by-course instead putting all urls onto one pdf
is not yet supported.
<br/><br/>
<p align="center">


  <img src="https://user-images.githubusercontent.com/90370987/227841527-66129135-acb4-46e3-b73a-f9dcfb8672ba.png">
</p>
