# YOLO-Malaria

## Description

In the computational inteligence subject we got on the master's degree of computer science, we had to develop a deep learning system for a real world problem. After little searching I came up with this dataset in Kaggle about Malaria and I got interested on that topic so I went for it!

Here you can find all the details https://www.kaggle.com/kmader/malaria-bounding-boxes but I will explain briefly what the dataset and the context is like.

Malaria is one of the deadliest diseases in the world causing 400000 deaths per year. The inspections of cells manually remains the gold standard for parasite detection and this could lead to human bias and poor performance caused by this laborious task. Automating this task is one of the remaining goals to achieve due to the lack of replication and comparision combined to the the absence of a gold standard and the negative of some researching centres to publish some images has made this process hard to accomplish.

In order to address this problem, the dataset provided contains 1364 images (around 80000 cells) from diferent researching centers divided in two different sets: train and test. The data is labelled in 6 classes: 2 type of uninfected cells and 4 type of infected cells (a "difficult" class is also appear when the annotators did not know the label). Besides this, a class label and a set of bounding boxes are given for each cell. So our main goal is to identify the type of cell and its coordinates for the test set provided.


## Code

I split the main goal in two different ones to deep in step by step.

First, I created a Jupyter notebook to see the data, preprocess it and write it back to make it compatible with the detection algorithm I was going to use: YOLO.

After that, I created another notebook (this time in Google Collab) to run all the experiments and to get the final results over the test set.

You can find those notebooks and the rest of the files needed to make it run on the repository. I attached the document I wrote there as well (only available in spanish so far 😅)


## Conclusions and Results

The results were not so bad taking into account the unbalanced dataset given (around 95/5) and the limited factors I had to face: time to deadline and Google Collab resources. The best model I trained got a 41.45% in the mAP metric for the test test! Nothing to be ashamed of!

As a recap of everything just mentioned:
+ The problem itself was not trivial at all and it was quite a challenge. Specially the preprocessing stage.
+ The unbalanced dataset limited the results and oversampling and undersampling techniques could have been tried to improve that.
+ Training with more muscle surely would have ended up in better results: bigger images, training longer, training with big model and so on.
+ Different hyperparameters selection could have pushed a litte more the metric.
+ Obtaining more data usually a good idea. However, it should have some quality and in our case it should be public. So, we did not use any external help but I am pretty sure it would have helped a bit more.
