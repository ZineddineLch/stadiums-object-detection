Overview
This challenge focuses on leveraging artificial intelligence to detect football stadiums using remote sensing imagery. Participants will apply object detection techniques to identify and classify stadiums from satellite and aerial datasets, addressing challenges such as varying scales, lighting conditions, and environmental factors. By advancing AI capabilities in remote sensing, this project has significant potential to enhance urban planning and sports infrastructure management.


Details:
Objective
The primary objective is to develop AI-powered object detection models capable of accurately identifying football stadiums in multispectral datasets. These solutions will contribute to advancements in urban planning by providing precise data for the allocation of resources and space. They will also support sports infrastructure management by enabling efficient monitoring and maintenance of stadiums, while driving innovation in remote sensing applications to tackle complex real-world problems.

Key Challenges:
Data Preparation: Preprocess multispectral datasets for model training, including data augmentation and normalization tailored for stadium features.
Model Development: Build and train AI-based object detection systems to accurately detect football stadiums in different scenarios and lighting conditions.
Comparative Analysis: Conduct a comparative study of multi-source versus single-source training, evaluating the trade-off between detection accuracy and generalization capacity.
Validation: Assess system performance using metrics such as , precision, recall, and F1-score, validating against ground truth data or expert-annotated datasets.
Submission Guidelines
To ensure a successful submission of your test set predictions, follow these structured steps:

Step 1: Understand Submission Format
The submission file must be a CSV file.
Required columns in the CSV:
ImageID_stadium_i: The unique identifier or filename of the image alongside with a stadium Id , unique assigned to each detected stadium in the image (e.g., stadium_1, stadium_2, etc.).
BoundingBox: The predicted bounding box for the stadium, represented as [x_center,y_center, width, height] in pixel coordinates.
Example of Submission CSV
ImageID_stadiumID	x_center	y_center	width	height
image1_png_stadium_1	0.506757	0.413007	0.104730	0.096284
image1_png_stadium_2	0.506757	0.413007	0.104730	0.096284
51610_png_stadium_1	0.506757	0.413007	0.104730	0.096284
51610_png_stadium_2	0.506757	0.413007	0.104730	0.096284
⚠️ Important: Ensure having 2 rows per image in the submission CSV!
Step 2: Generate Predictions
Run your model on the test set images.
For each test image:
Extract predictions in the required format.
Ensure bounding box coordinates are normalized to [0, 1].
Step 3: Upload to Kaggle
Navigate to the Submit Predictions section of the competition page.
Upload your submission.csv file.
Wait for Kaggle to evaluate your predictions and update the leaderboard.
