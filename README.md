University of Pisa, UNIPI \
M.Sc. Computer science, Artificial Intelligence \
Academic year 2021/22 



# Intelligent System for Pattern Recognition
###### Midterm Assignments for ISPR course (Prof. Davide Bacciu)

## [Midterm 1](Midterm_1) 
### Image Processing: clustering of SIFT descriptors

**Dataset:** [Link](http://download.microsoft.com/download/A/1/1/A116CD80-5B79-407E-B5CE-3D5C6ED8B0D5/msrc_objcategimagedatabase_v1.zip), [File](xx)

**Assignment Overview:** \
Select from the given [dataset](http://download.microsoft.com/download/A/1/1/A116CD80-5B79-407E-B5CE-3D5C6ED8B0D5/msrc_objcategimagedatabase_v1.zip) four thematic subsets of your choice, out of the total 8 available, and collect all the associated images. For these images, extract the **SIFT descriptors** using the visual feature detector embedded in SIFT to identify the points of interest. Aggregate all the identified descriptors in a dataset and run **k-means** (or any clustering algorithm of your choice) on such data to partition the descriptors in **clusters**. Then analyze the obtained clusters by confronting the descriptors assigned to each cluster with the thematic classes of the images from which they were extracted (in other words, compute a confusion matrix between the clusters and the four thematic images). Discuss your findings. Choice of the number of clusters and of the clustering algorithm is on you (and should be discussed in the report).

## [Midterm 2](Midterm_2)
#### Signal Processing: regime detection with Hidden Markov Model

**Assignment Overview.** 
Fit an **Hidden Markov Model with Gaussian emissions** to the data in [DSET1](https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction#): it is sufficient to focus on the “Appliances” and “Lights” columns of the dataset which measure the energy consumption of appliances and lights, respectively, across a period of 4.5 months. Consider the two columnsin isolation, i.e. train two separate HMM, one for appliances and one for light.  Experiment with HMMs with a varying number of **hidden states** (e.g. at least 2, 3 and 4). Once trained the HMMs, perform **Viterbi** on a reasonably sized subsequence (e.g. 1 month of data) and plot the timeseries data highlighting (e.g. with different colours) the hidden state assigned to each timepoint by the Viterbi algorithm.  Then, try **sampling** a sequence of at least 100 points from the trained HMMs and show it on a plot discussing similarities and differences w.r.t. the ground truth data.

