# Age Verification for Supermarket Customer with Computer Vision

## Project Description

Good Seed, a supermarket franchise, is exploring the potential of data science to help them comply with age-restriction laws by preventing the sale of age-restricted products to underage customers. As part of this initiative, the task is to build and evaluate a model capable of verifying a person's age using computer vision methods.

- The franchise's stores are equipped with cameras in the checkout area, which will trigger a signal when a customer purchases an age-restricted product. 
- Computer vision techniques can be employed to determine a person's age from photos captured by these cameras.
- To commence the assignment, a set of photos of individuals along with their ages captioned will be provided for analysis and model development. 

The ultimate goal is to develop an effective model that assists Good Seed in ensuring legal compliance and responsible sales practices.

## Data Description
Dataset is stored in files `labels.csv`

- *File* `labels.csv` with 2 columns: `file_name` dan `real_age` 

Regarding the large number of pictures, the generator will be made with ImageDataGenerator

## Methodology
- Data Overview
- Exporative Data Analysis
  - Sample Images
- Modelling (with GPU platform)

## Result
- Excellent results were achieved from our model where our model avoided overfitting which has **MAE** at 7 with epochs=10
- The **adam** optimizer help to improve the result by lowering the training time
- With a lot of information and better quality of  the pictures, it is possible to make the **MAE** much lower
- The **ImageDataGenerator** also help to speed up the training process by reducing the image size

## Contact
For any questions or feedback regarding this project, feel free to reach out to me at mahendraalfathfirdaus@gmail.com.
