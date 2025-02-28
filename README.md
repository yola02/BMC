# BMC
Bacterial Morphology Classification - Yola Charara

Link to dataset: https://drive.google.com/drive/folders/1dN3EfDDlfjZP1Yw1RlsErZtNaKafpt-7?usp=sharing 

Dataset Format:

The dataset includes 600 images of bacteria seen under different types of microscope. 

The 600 images are divided into three classifications as follows:
200 images of cocci bacteria
200 images of bacilli bacteria
200 images of spirilla bacteria

The images will be labeled as either "cocci", "bacilli", or "spirilla".

Data Extraction:

Downloaded images of bacteria seen under the microscope using the python library "bing-image-downloader" which downloads a bulk of images from Bing. 

The code was written on Google Colab as follows:

#Install the bing-image-downloader library.

!pip install bing-image-downloader 

#Download the images in the folder named "images".

!mkdir images 

#Replace "cocci_under_microscope" with other bacteria names to download the desired images (e.g. "bacilli_under_microscope", "spirilla_under_microscope", "campylobacter_jejuni_under_microscope", "diplococcus_electron_micrograph", "staphylococcus_electron_micrograph"...).

#Set the limit for images download (e.g. limit=50 means that it will download a maximum of 50 images).

From bing_image_downloader import downloader
downloader.download("cocci_under_microscope", limit=50, output_dir='images', adult_filter_off=True, force_replace=False, timeout=60) 

Lastly, check the images under the "images" folder and download the best images on your desktop. Organize all the datapoints in a folder and upload it to Google Drive.

Expected timeframe for labeling the data:

It should take approximately 5 seconds to label each datapoint. 
The labeler will only need to distinguish between 3 shapes of bacteria.

Data Collection Date:

The data was collected from September 28, 2024 till October 1, 2024.
