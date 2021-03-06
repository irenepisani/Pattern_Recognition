University of Pisa, UNIPI \
M.Sc. Computer science, Artificial Intelligence \
Academic year 2021/22 



# Intelligent System for Pattern Recognition
###### Midterm Assignments for ISPR course (Prof. Davide Bacciu)

## [Midterm 1](Midterm_1) 
### Image Processing: clustering of SIFT descriptors

  * **Dataset:** [External link](http://download.microsoft.com/download/A/1/1/A116CD80-5B79-407E-B5CE-3D5C6ED8B0D5/msrc_objcategimagedatabase_v1.zip), [Used images](Midterm_1/images_)
  * **Colab Notebook:** [`midterm_1_5.ipynb`](Midterm_1/midterm_1_5.ipynb)
  * **Assignment Overview:** Select four thematic subsets of your choice, out of the total 8 available, and collect all the associated images. For these images, extract the **SIFT descriptors** using the visual feature detector embedded in SIFT to identify the points of interest. Aggregate all the identified descriptors in a dataset and run **k-means** (or any clustering algorithm of your choice) on such data to partition the descriptors in **clusters**. Then analyze the obtained clusters by confronting the descriptors assigned to each cluster with the thematic classes of the images from which they were extracted (in other words, compute a confusion matrix between the clusters and the four thematic images). Discuss your findings. Choice of the number of clusters and of the clustering algorithm is on you (and should be discussed in the report).

## [Midterm 2](Midterm_2)
### Signal Processing: regime detection with Hidden Markov Model

  * **Dataset:** [External link](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction#), [DSET1](Midterm_2/energy_datasetv1.csv)
  * **Colab Notebook:** [`midterm_2_1.ipynb`](Midterm_2/midterm_2_1.ipynb)
  * **Assignment Overview:** Fit an **Hidden Markov Model with Gaussian emissions** to the data in [DSET1](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction#): it is sufficient to focus on the “Appliances” and “Lights” columns of the dataset which measure the energy consumption of appliances and lights, respectively, across a period of 4.5 months. Consider the two columnsin isolation, i.e. train two separate HMM, one for appliances and one for light.  Experiment with HMMs with a varying number of **hidden states** (e.g. at least 2, 3 and 4). Once trained the HMMs, perform **Viterbi** on a reasonably sized subsequence (e.g. 1 month of data) and plot the timeseries data highlighting (e.g. with different colours) the hidden state assigned to each timepoint by the Viterbi algorithm.  Then, try **sampling** a sequence of at least 100 points from the trained HMMs and show it on a plot discussing similarities and differences w.r.t. the ground truth data.

## [Midterm 3](Midterm_3)
### Text Processing: fake news classification with Bi-Directional LSTM Recurrent NN

  * **Dataset:** [External link](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)
  * **Colab Notebook:** [`midterm_3_6.ipynb`](Midterm_3/midterm_3_6.ipynb)
  * **Assignment Overview:** The dataset contains real and fake news, including their title, text, subject, and date. The objective is to train a binary classifier to recognize fake news. You are free to choose the model's architecture, but you should describe and justify your design choices.
Notice that the fake and real news in the dataset are balanced. However, in the real world, real news are much more frequent than fake ones (hopefully). Simulate the effect of the data imbalance by undersampling/oversampling one of the classes in the training set and compute the test accuracy on a (balanced) test set. Then, try to use a mechanism to make the training robust to imbalances, such as weighting the loss for the samples depending on their class. Discuss the results of this mitigation.You are allowed to preprocess the data however you want (e.g. using pretrained embeddings, dropping some features, just a bag-of-words), but the classification model must be trained by yourself.


## [Midterm 4](Midterm_4)
### Reinforcement Learning

  * **Paper:** [Carlos Florensa et al., Automatic Goal Generation for Reinforcement Learning Agents, ICML, 2019.](https://arxiv.org/abs/1705.06366)
  * **Presentation:** [`midterm_4_15.pdf`](Midterm_4/midterm_4_15.pdf)
  * **Assignment Overview:** Summarize in short presetation the main findings of the choosen paper. 

