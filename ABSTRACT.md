**EALPR: Vehicles** stands as a specialized dataset tailored for object detection purposes, specifically focusing on the identification and localization of license plates. With a compilation of 2084 images, the dataset encompasses a total of 2140 annotated objects, all falling under the singular class of *license_plate*. Notably, the dataset predominantly features Egyptian License Plates (LP) marked by Arabic digits and characters, showcasing the diversity of license plate styles found across different regions and countries utilizing various scripts, including Latin letters commonly used in Europe, Brazil, the US, and several other locales. This diversity provides an extensive array of examples for training models to recognize and extract license plate information from varying international contexts.

## EALPR Structure

- EALPR: Vehicles (current)
- EALPR: Plates [(available on DatasetNinja)](https://datasetninja.com/ealpr-plates)

<img src="https://i.ibb.co/BNjRwgR/Screenshot-2023-10-30-151153.png" alt="image" width="400">

<span style="font-size: smaller; font-style: italic;">EALPR: Vehicles demo.</span>

<img src="https://i.ibb.co/brTZ8NC/Screenshot-2023-10-30-151206.png" alt="image" width="400">

<span style="font-size: smaller; font-style: italic;">EALPR: Plates demo.</span>

## Proposed method

Authors use two object detection models for license plate detection and recognition. The input to authors' proposed system is the vehicle image, whereas the output is the recognized license plate characters and digits. Tiny-YOLOV3 is the backbone architecture for both stages LP detection and recognition.

<img src="https://i.ibb.co/D8B8sBh/Screenshot-2023-10-30-145453.png" alt="image" width="800">

<span style="font-size: smaller; font-style: italic;">Main Stages of the Proposed EALPR Approach.</span>

## About EALPR

Authors scrap the EALPR dataset images from websites such as Instagram pages and Facebook Marketplace using web scraping Tools. It has 2,450, and 12,160 characters images including many types of vehicles such as cars, buses, trucks, microbuses, and mini-busses. The vehicle images are captured using different cameras, at varying times, lighting, and background. 

<img src="https://i.ibb.co/tx3gwCz/Screenshot-2023-10-30-150107.png" alt="image" width="800">

<span style="font-size: smaller; font-style: italic;">Characters and Digits Statistics in the EALPR Dataset.</span>

The Egyptian License Plate (LP) uses the Arabic digits and characters which is varying in several countries that use Latin letters such as Europe, Brazil, US, ... etc. It has a dimension 16 (height) X 40 (width) with aspect ratio 1:2 approximately. its layout is divided into 3 regions: the country region contains the Egypt word in Arabic and English format, the character region includes plate characters, and the number region contains plate digits. Egyptian License Plate structure uses 10 Arabic digits and 17 Arabic characters.

<img src="https://i.ibb.co/0Jb9NqC/Screenshot-2023-10-30-150456.png" alt="image" width="400">

<span style="font-size: smaller; font-style: italic;">Egyptian License Plate Structure.</span>

<img src="https://i.ibb.co/x6Q65PD/Screenshot-2023-10-30-150910.png" alt="image" width="400">

<span style="font-size: smaller; font-style: italic;">Plate Arabic Digits and Latin Digits.</span>

<img src="https://i.ibb.co/Pc3Ljny/Screenshot-2023-10-30-150925.png" alt="image" width="800">

<span style="font-size: smaller; font-style: italic;">Plate Arabic Characters and Latin Characters.</span>

After collecting EALPR dataset authors manually annotate the vehicles, characters, and digits using [Ybat tool](https://github.com/drainingsun/ybat).
