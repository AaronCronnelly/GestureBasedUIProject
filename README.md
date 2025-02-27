# GestureBasedUIProject
# Aaron Cronnelly (G00403528)

---

## Loading & Exploring the Dataset

After downloading the fashion dataset from the module page, I set up the project structure and placed the dataset inside the data/ folder. The dataset consists of 10 different categories, each stored in a separate folder. The categories include ankleboot, bag, coat, dress, pullover, sandal, shirt, sneaker, trouser, and t-shirt/top.

To get an understanding of the dataset, I counted the number of images in each folder. Each category contains exactly 7,000 images, adding up to a total of 70,000 images. This confirms that the dataset is balanced, which is important for model training, as it prevents bias towards any specific category.

I then sampled some images from different categories and displayed them to get a better visual idea of what the dataset contains. All the images are grayscale and 28x28 pixels in size, meaning no resizing will be needed, which keeps things simple. Looking at the images also helped in confirming that the dataset contains clear and well-defined clothing items.

---

## Cleaning & Preprocessing the Data

With the dataset explored, the next step was data cleaning to make sure it was ready for training. The first thing to check was if all images were the same size (28x28 pixels). Running a check across all files confirmed that they were already uniform, meaning no extra resizing was needed.

Next, the images were normalized by scaling their pixel values from 0 to 1. Since image pixels originally range from 0 to 255, this step ensures that all values fall within a standard range. This is important for training, as it helps models learn better and prevents large pixel values from dominating the training process.

Since the dataset used folder names as categories, I also needed to prepare the labels. Instead of using text labels like "ankleboot" or "shirt", each category was assigned a numeric label from 0-9. This makes it easier for machine learning models to process and classify the images efficiently.

Now that the dataset has been cleaned, normalized, and labeled, it's ready for the next phase: analyzing patterns, checking feature distributions, and preparing for model training.

---