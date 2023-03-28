
<p align="center">
  <img src="https://user-images.githubusercontent.com/90370987/227833445-3f30c4b8-1c90-4ac7-a1ae-113352d2156d.png" width=640.7 height=171.9>
</p>

# Overview

Welcome to Click Me! This is a project that utilizes a fine-tuned Mobilenet Model and Pytesseract to recognize URL overlays in LinkedIn Courses and extract relevant metadata such as timestamp, the overlay itself, and the bounding box of the overlay (the coordinates on the screen where the overlay appears). The primary objective of this project is to automate the process of gathering essential metadata to create clickable UI elements in courses. In addition, the extracted data can be used to check the status of URLs provided in LinkedIn courses and generate PDFs containing the URLs from a given course. Below is a demonstration of extracting data from an input video and outputting it to JSON:

<br/><br/>


<video src="https://user-images.githubusercontent.com/90370987/228164081-2591a1e6-b7c3-4d61-9aaf-c7897e6e228d.mp4">Demo Video 1: Checking link status</video>

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


# Potential Applications
## Clickable UI Elements
There are currently three potential applications of the extracted data. The primary one is to use it to create clickable user interface elements. This provides a convenient way for learners to access links, and also makes the content more accessible to visually impaired learners by providing them with URLs that may not be available in closed captioning. <br/><br/>
<p align="center">
  
  <img src="https://user-images.githubusercontent.com/90370987/227855933-194c98ba-ec43-4362-9054-5ae4d1bb4c9e.jpg" width=700 height=400>
</p>

<br/><br/>  
## Evergreen Content
Another application of the program is to maintain evergreen content. After publishing, the program can be executed to verify which links are currently functional and which ones return a 404 error, allowing for the timely maintenance of older courses with non-functional URLs. The following is a demonstration of how the program checks the links in the JSON file, including an example of how it responds when it detects a broken link.
<br/><br/>

<video src="https://user-images.githubusercontent.com/90370987/228154234-a2c54630-fa4a-4248-a99a-c70dab1adfe8.mp4">Demo Video 2: Checking link status</video>

<br/>

## Automatic PDF Generation
The third and final current use case is the automatic generation of PDFs containing links that can be distributed in exercise files. An example PDF, which utilizes data from the JSON file, is shown below. Both the title and header of the PDF are customizable parameters. However, it's important to note that generating PDFs course-by-course instead of putting all URLs onto one PDF is not yet supported in this current version.
<br/><br/>
<p align="center">


  <img src="https://user-images.githubusercontent.com/90370987/227841527-66129135-acb4-46e3-b73a-f9dcfb8672ba.png">
</p>


