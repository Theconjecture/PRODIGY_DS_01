<!-- Add a banner image at the top -->
<img src="https://github.com/user-attachments/assets/c6f3892e-0754-492c-ae57-e7e5b15c7bfa" alt="Description" style="width: 100%;" />



#### First task of InfoTech Data Science Internship : Create a bar chart or histogram to visualize the distribution of a categorical or continuous variable, such as the distribution of ages or genders in a population.

# PRODIGY_DS_01
<!-- Replace "Project Title" with your project's name -->

## Table of Contents
<!-- A Table of Contents helps readers navigate your README -->
- [About the Project](#about-the-project)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contact](#contact)

## About the Project
<!-- A brief description of your project -->
Using land cover images taken by Landsat 8 to classify terrains, the study area is Iskele, Northern Cyprus

## Getting Started
<!-- Instructions on how to get a copy of the project up and running -->
Originally downloaded the the first seven bands from the USGS Earth Explorer.
![Raster_band](https://github.com/user-attachments/assets/7e9481c7-317d-4560-9676-451c38921690)

Next, I clipped the raster bands to the area of interest

#### Original Area

![Original_area](https://github.com/user-attachments/assets/470942da-9fb7-46e1-b24b-98bb102a30af)

#### Clipped Area
![Clipped_area](https://github.com/user-attachments/assets/fc84cba8-b911-4209-9144-1b8fb56d37e8)

Next, I chose a set of pixels to represent the macro classes in the image, ID as follows:

| Macro Class ID   | Label   |
|------------|------------|
| 1  | Water  |
| 2  | Built-up  |
| 3  | Vegetation  |
| 4  | Soil  |

#### Training sample regions

![Training_Sample](https://github.com/user-attachments/assets/008ae8f0-87bc-48ee-8060-2e55b0d1783e)

Then I ran a maximum likelihood classification and got the resulting layer:

#### You can the see the legend on the far left side

![Screen Shot 2024-07-27 at 21 20 11](https://github.com/user-attachments/assets/e999994f-6e57-4377-b1a6-06669698afa3)

Finally, I converted the layer into a vector and exported it as classification.csv. Two attributes: Pixel Nuumber and Macro class ID 

