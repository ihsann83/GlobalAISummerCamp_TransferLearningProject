# GlobalAISummerCamp_TransferLearningProject

Data Set: https://www.microsoft.com/en-us/download/details.aspx?id=54765

Firstly, I loaded necessary libraries.

Then, I checked the images. I showed them, I checked their types and shapes. 

# Data Preprocessing

I resized the images (128,128,3) as MobileNetV2 requires and I normalized the images. After that, I got 1000s samples for both categories ( cat, dog) because I might have struggled with working more data. So, I chose 1000s samples for both categories.

# Train Test Split

I suffled the images with random.suffle in order to avoid a leakage. Because model might be abused with the splitted samples categories.

I splitted the images to the X train and X test, then the indexes into Y train and Y test.After that, I changed the types to the array to be able to put them in to the model. Lastly, I saved the train, validation and test data with pickle dump.

# Model Training and Evaluation

Then, I opened a new collab and called the saved data sets ( train, validation and test).

I built a base model and transfered MobileNetV2 to my base model as transfer learning model. Then I built a head model as well and  made the necessary arrangements to use transfered model's input hypermeters in that head model.

Finally I trained my model, got the scores and visualized them.


