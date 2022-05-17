# Machine Learning Model for the Stylistic Classification of Fine Art

## UT Austin CS 370 Undergraduate Research Project Spring 2022
### Researcher: Tejas Saboo <br> Supervisor: Professor Angela Beasley

Check out the CS370 Research Slides pdf file for a quick summary of my research project or explore the actual model and its architecture by opening the CS370 ipynb files.

### Introduction

Emerging technologies are disrupting the art industry and changing the way we create and experience art. As a computer science, mathematics, and statistics student with a deep appreciation for arts and culture, I am fascinated by how technology shapes our society. One recent technological advancement I am excited about is OpenAI's Dall-E 2, an AI system that can create realistic images and art from a description in natural language. I enjoy learning about innovative inventions and discoveries, and I love applying my learnings to build impactful technologies. For my undergraduate research project, I decided to explore the intersection of art, design, and technology to identify and address opportunities to augment human creativity. The project entailed architecting a deep convolutional neural network model to classify visual fine artwork by its artistic style.

### Results

The final machine learning model presented is a deep convolutional neural network for the multi-class classification of fine art by its artistic style. The style of an artwork refers to its distinctive visual elements, techniques, and methods, typically corresponding with an art movement or school group that the artist is associated with.

The cs370-tejassaboo-ml-for-stylistic-classification-of-fine-art-multiclass model is used to distinguish between the artistic styles of Cubism, Ukiyo-e, Northern Renaissance, and Pointillism. The model is highly successful with a 97.1250% accuracy on the training set and 46.0000% accuracy on the test set after 70 epochs of training.

The cs370-tejassaboo-ml-for-stylistic-classification-of-fine-art-binary model is used to distinguish between the artistic styles of Realism and Pointillism. The model is highly successful with a 95.6250% accuracy on the training set and 64.5000% accuracy on the test set after 78 epochs of training.

The cs370-tejassaboo-ml-for-stylistic-classification-of-fine-art-binary-v2 model is used to distinguish between the artistic styles of Realism and Cubism. The model is highly successful with a 97.1250% accuracy on the training set and 66.0000% accuracy on the test set after 77 epochs of training.


### Experimental Process

I experimented with a variety of different technical approaches and model architectures throughout this project. First, I reviewed neural networks and machine learning concepts, learned about computer vision, and determined the relevant libraries. I decided that using Python's PyTorch library would be ideal for creating a customizable and scalable model for image classification tasks. Then, I scoped out my project and established a timeline of major milestones. Next, I searched for art databases and found a dataset with images of flower and marina paintings. After finding a relevant dataset, I set up a custom data loader using the torchvision library's ImageFolder and torch library's DataLoader functions. Then, I performed a manual train-test split. For each stylistic category, I moved 80 images into the training set and 20 images into the test set. Next, I designed a simple linear neural network model, created a training function, and implemented an evaluation function. I trained the model on the flower and marina painting dataset, then performed hyperparameter tuning. Then, I realized that the model was too simple, so I experimented with various architectures such as linear and non-linear neural networks, convolutional neural networks, fully convolutional neural networks, and deep convolutional neural networks. By limiting the size of the initial train and test sets, I was able to quickly train the models and continuously prototype the model architecture. Next, I searched for a dataset with artwork categorized by its artistic style, and I discovered the Wikiart database and found a corresponding Wikiart dataset that I decided to use for my final model. I updated the model to be compatible with the wikiart dataset and retrained it. However, I realized that manually moving images from the wikiart directory to the train and test directories would be tedious and impractical at scale, so I decided to automate the process. I learned how to use the shutil.move functionality to automate moving files from one directory to another, resulting in a scalable train-test split that also randomly shuffles the images. This allowed me to have train and test datasets on the order of hundreds and thousands of images in seconds. Then, I retrained the model on the larger dataset for a binary classification problem. Noting the low training accuracy, I updated the model to use blocks. While this improved the training accuracy significantly, I now had the problem of overfitting since there was a significant disparity between the training and testing accuracies. I implemented data augmentation in the training image transform function, experimented with various criterion loss functions, tested stochastic gradient descent versus adam for the optimizer, investigated regularization techniques, added dropouts, and tried various learning rates throughout my hyperparameter tuning process. This successfully reduced overfitting and improved model train and test accuracy. Then, I modified the model for multi-class image classification tasks. Finally, I modularized my functions, added documentation, and made final improvements. 

### Future Plans

My future plans to build on this project include experimenting with computer vision to extract visual features and elements of the artwork such as line, shape, texture, form, space, color, value, composition, perspective, and subject matter to create algorithms that suggest tags for artwork. Next, I will create an algorithm that generates original and relevant titles for the artwork using the tags and extracted visual features. I will also investigate recent artificial intelligence and machine learning advancements to create an algorithm that measures the creativity and craftsmanship expemplified in the artwork and provides actionable feedback to help artists improve. Furthermore, I plan on learning more about blockchain and NFTs and possibly launching my own project.

### Involvement in the Scientific Community

Throughout the semester, I made a conscious effort to become more involved and engaged with the scientific community. My first step was to learn and contribute to academia through this undergraduate research project. Next, I read research publications and articles about technological advancements in industry. I decided to take this a step further by attending research conferences and symposiums, faculty talks, industry events, and honors thesis defenses. These include:

<br>
- Institute for Foundations of Machine Learning: AI for Accurate and Fair Imaging with Alex Dimakis
<br>
- Good Systems Annual Symposium: Defining, Evaluating, and Building Ethical AI Systems
<br>
- 2022 UT Machine Learning Laboratory Research Symposium
<br>
- Quantum Computing Triple Play at UT Austin (Quantum Conference with Dr. Aaronson, Atom Computing, and Strangeworks)
<br>
- Tesla Cyber Rodeo
<br> 
- Chat with Jahmy Hindman, the CTO of John Deere
<br>
- Bloomberg Engineering: Inclusive Branch (Re)Naming at Scale
<br>
- Hosting UT Entrepreneurship Week and Moderating the Democratizing Healthcare Innovation Panel
<br>
- Undergraduate Honors Thesis Defense
<br>
- Quantum Information Science Final Presentations
