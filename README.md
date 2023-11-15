# flaky_tests_AI
-----------------
 In this project, we use different ML classifiers from sklearn to classify flaky test among several opensource projects from github. 

 ##
 <ol>
   <li> Dataset </li>
   Our data comes from github and Flaky dataset, (see this Link <https://zenodo.org/record/6994692>). The projects are of 5 different programming languages: Java, Python, C++, Go and JavaScipt. We label them to be "Flaky" and "NonFlaky" in our dataset.<br>
   <li>Preprocessing</li>
   Here is the workflow of our methods.
   <img src='./utils/method flow.png'> <br>
   <li>Classifiers</li>
   See the figure above. <br>
   </ol>

-----------------------
## Environment
  <ul>
  <li>Jupyter Notebook</li>
  <li>Python 3.11</li>
  <li> sklearn==0.20 </li>
  <li>pandas==2.1.1</li>
  <li>matplotlib</li></ul>


-----------------------------------------


## Files
-----------------------------------------
<ul>

###  <li>classification.ipynb</li>

The jupyter notebook file is used to create our sub-datasets and classify. All the results are stored in "output". You can custom the figure by commenting some lines in the last part of the file, and if you want to visualize other results data, you can change the value of "vis_data". </br>

### <li>cross_test.ipynb</li>

In this notebook, the data of a programming language is training set, and another language is testing set. For example, we use Java as training set, and python as testing set. </br>

### <li>flaky_data.xlsx</li>

The original dataset we used. It contains Java, Python, Go, C++ and JS code snippets. Each sample contains "Language", "Project name", "test case name", "label" and "test case content". We label the data to be "Flaky" and "NoFlaky".</br>

### <li>results.xlsx</li>

We collated the results for analysis. It contains results of train-test split 70-30, 80-20, and cross-projects, statistics and cross-validation.</br>



