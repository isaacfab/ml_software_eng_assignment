# Software Engineering for Machine Learning Assignment

### Project Context

You are in the process of developing a ‘new’ system that will improve the CMU graduate student admission process. During this development effort your team has identified several key areas where machine learning could improve the product. Specifically, the population of applicants is large as is the size of packets submitted. Historically, the down select effort has required significant manual analysis. Because CMU has collected student performance data your team can use this information to help predict which applicants will have the highest likelihood of success. This information can then be used to help make the selection process more streamlined. 

### Tasks

You and your team have been given the historical dataset of CMU student performance and need to explore it in order to understand what information is available. You will use the sci-kit learn python package to build and train a model once you have sufficient understanding of the dataset. After your model is built you need to evaluate the model quality. Once you determine the model quality is sufficient your team needs to build a microservice that takes as input a student’s information and then returns some likelihood of success. This service needs to be incorporated into your existing admissions product.

### Data and Code

The **data** folder contains the raw dataset as a csv (this is an augmented version of the dataset [found here](https://archive.ics.uci.edu/ml/datasets/Student+Performance)). The student performance is determined by their grades (G1, G2, and G3). G3 is the final year grade and is the target performance metric. Grades are given on a scale of 0-20 where 20 is the best.

There is an example flask api with docker file in the **dockerfile/apps** folder. Use this as a template to build and deploy the microservice. Use [this article](https://towardsdatascience.com/a-flask-api-for-serving-scikit-learn-models-c8bcdaa41daa) and [this repo](https://github.com/amirziai/sklearnflask/blob/master/main.py) as a resource to build and save a **sci-kit learn** model then deploy it using flask.
