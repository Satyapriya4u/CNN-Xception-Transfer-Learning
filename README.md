# CNN-Xception-Transfer-Learning
Crack Detection Image Classification To develop a Binary Image Classification Model that can classify images containing Cracks from those without Cracks

Instructions: Use Google Colab to work on this assignment using Python language. All cell outputs and visualizations should be visible and necessary comments should be put to make the code readable. Please mention your name and roll number in your colab jupyter notebook file. Also, mention your Kaggle username which you have used for participating in the competition.

This assignment is on Image classification problem using deep convolutional neural networks. The dataset consists of images obtained from concrete bridge decks, pavements, and walls. The images can contain either cracks or no cracks. Your objective in this challenge is to develop a binary image classification model that can classify from a given image if it contains any cracks or not.
This assignment is hosted in Kaggle as an in-class competition. You should upload your output file (in the specified format mentioned later) in the Kaggle competition link for finding out the evaluation score (F1-score) for test dataset. You can modify your code and submit your output multiple times to obtain higher scores. A maximum of 20 submission is allowed per day (UTC timing). Bonus marks will be given to the top performer(s) (subject to evaluation of the code). All details on the dataset and submission format are also provided in the Kaggle competition link.
Kaggle Competition Link: https://www.kaggle.com/t/856f08a20e0f47c7b3445fb1b477b4e0
Data The dataset consists of 2 folders: 'train' and 'test'. The folder 'train' is a labeled dataset and consists of 2 sub-folders: 'cracked' and 'uncracked'. The sub-folder 'cracked' consists of a total of 7501 images containing cracks, while the 'uncracked' sub-folder contains 7467 images with no cracks. All images are of the ‘.jpg’ format. The ‘test’ folder consists of the test dataset images. There are a total of 2000 images in this folder (all ‘.jpg’ files). These images are unlabelled i.e., the labels are not provided, whether they contain cracks or not. The objective of this challenge is to predict the class of each of these test images. The class can be either ‘cracked’ or ‘uncracked’. The filenames of these test images are given as 1.jpg, 2.jpg, 3.jpg, …, 2000.jpg. The dataset is uploaded in the Kaggle competition link.
Evaluation The evaluation metric for this challenge is Mean F1-Score. The F1 score, commonly used in information retrieval, measures accuracy using the statistics precision p and recall r. Precision is the
ratio of true positives (tp) to all predicted positives (tp + fp). Recall is the ratio of true positives to all actual positives (tp + fn). 𝐹1=2𝑝𝑟𝑝+𝑟 𝑤ℎ𝑒𝑟𝑒 𝑝=𝑡𝑝𝑡𝑝+𝑓𝑝,𝑟=𝑡𝑝𝑡𝑝+𝑓𝑛 The F1 metric weights recall and precision equally, and a good retrieval algorithm will maximize both precision and recall simultaneously. Thus, moderately good performance on both will be favored over extremely good performance on one and poor performance on the other. 50% of the test images will be used for public leaderboard performance calculation and the remaining 50% will be used for private leaderboard. Public scores will be shown on the public leaderboard, while only the private scores will be used for final evaluation. The private leaderboard score is not shown until the end of the competition. You can hand-select any 2 of the eligible submissions for private leaderboard score, or it will otherwise default to the best public scoring submissions. Submission Format Submission files should be in .csv format and contain two columns: filename and class. ‘filename’ should be in string format and will contain the image filename (1.jpg, 2. jpg, etc.). The ‘class’ will also be in string format and contain the corresponding class name. It can take two values: ‘cracked’ or ‘uncracked’. Since there are 2000 images in the test dataset, your submission should have 2000 rows (excluding the header), each with 2 columns. A sample submission file is also provided in the dataset. The file should contain a header and have the following format:
filename
class
1.jpg
cracked Acknowledgements This dataset is adapted from SDNET 2018 dataset. Dorafshan, S., Thomas, R. J., & Maguire, M. (2018). SDNET2018: An annotated image dataset for non-contact concrete crack detection using deep convolutional neural networks. Data in Brief, 21, 1664–1668. https://doi.org/10.1016/j.dib.2018.11.015
