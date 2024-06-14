# Computer_Vision
# Automatic Fracture Detection in X-ray Images Using Image Processing Techniques

## Introduction

Detecting fractures in bones is crucial in cases of injury or accidents. Fast and accurate identification of fractures is essential, yet small fractures are often not easily visible in X-ray images. This project aims to develop an efficient image processing-based system for the rapid and accurate classification of bone fractures using X-ray and CT images. Fractured bone images were obtained from hospitals, and processing techniques such as segmentation, edge detection, and feature extraction methods were applied. These images were processed in a developed tool to detect small fractures and broken bones.

Traumatic injuries can be fatal to patients, and the likelihood of death significantly increases when associated with bone fractures. Combined with other bodily injuries, such as abdominal trauma, the risk of death can approach 100%. Severe injuries can result in significant bleeding, multiple organ dysfunction, nerve damage, and internal injuries, raising the mortality rate from 8.6% to 50%. Even without such severe injuries, fractures often cause intense pain and reduced mobility. Automated and accurate fracture detection from traumatic injuries can help doctors assess the severity of patients' conditions. Extracting fracture features and measuring displacement are crucial for aiding doctors in making quicker and more accurate decisions.

## Challenges in Fracture Detection

Automatic bone fracture detection using X-ray images is challenging due to low-resolution images, variations in bone structures, and different visual features of fractures in various regions. Medical imaging devices like X-rays, CT scans, MRI, and ultrasound are used to detect various abnormalities. X-rays and CT scans are commonly used in fracture diagnosis due to their speed and simplicity for examining bone and joint injuries. Hospitals store medical images in the DICOM format, which includes embedded text and is accessible via PACS. Digital image processing is rapidly growing and becoming a crucial part of the medical field due to its lower development and operational costs. Innovations in image processing are increasingly popular, playing a significant role in image manipulation and information extraction using various algorithms, providing quick and accurate diagnostic results.

## Methodology

1. **Image Collection**
   - Images from imaging methods include normal and fractured bone images.
   
2. **Image Preprocessing**
   - **Grayscale Conversion:** The first step involves converting images from RGB to grayscale using preprocessing techniques.
   
   - **Noise Removal:** The next step enhances image quality by using various filtering techniques to remove noise. Noise is defined as random variations in brightness and intensity, which can appear as grainy, textured, or snowy patterns in medical images. Noise reduces the visibility of certain features, especially low-contrast objects. The general noise equation is:
     \[
     f(x,y) = g(x,y) + \eta(x,y)
     \]
     where \( f(x,y) \) is the noisy image, \( g(x,y) \) is the original image, and \( \eta(x,y) \) is the noise. Common types of noise include salt and pepper, Gaussian, and Poisson noise. Median filtering can reduce salt and pepper noise with minimal edge blurring.
   

3. **Edge Detection**
   - Edge detection identifies points in an image where brightness changes abruptly. These points are segmented into linear curve pieces called edges.
   

4. **Hough Transform**
   - The Hough Transform is a popular method for detecting lines in 2D images, with advanced versions capable of detecting shapes like circles and ellipses. It uses a 2D array defined by the relation:
     \[
     r = x \cos \theta + y \sin \theta
     \]
     By finding peaks in the parameter space, probable lines are detected. In this system, the generalized Hough Transform is used for edge analysis and fracture detection.
     

## Results

A computer-based system for detecting broken bones from X-ray images was developed. Focusing on X-ray images, the process begins with preprocessing to reduce noise, followed by edge detection and Hough Transform implementation. The developed tool was tested on a set of images and showed promising results, accurately identifying both major and minor fractures with 75% accuracy. However, the tool has limitations in detecting skull, pelvis, and spine fractures.

## Conclusion

This project demonstrates the development of an automated system for bone fracture detection using image processing techniques. While the tool shows significant promise, further enhancements are necessary to improve accuracy and extend its capabilities to detect fractures in other complex bone structures. 



