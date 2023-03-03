# Machine learning workflow for vehicle image classification on AWS  

The goal of this project is to build an image classification model that can distinguish delivery vehicles between bicycles and motorcycles. This model can then be used to 
improve the delivery process by assigning orders more efficiently to drivers.

The model was trained on 1,000 images of bicycles and motorbcycles extracted from the [CIFAR-100](https://www.cs.toronto.edu/~kriz/cifar.html) dataset using the SageMaker’s built-in image classification algorithm.

Additionally, the model was deployed to a SageMaker endpoint and an automated workflow was set up using Lambda and Step Function to serialize input images, invoke the endpoint, and filter the inferences according to their confidence levels. SageMaker Monitor was also implemented to track the endpoint’s performance.

The development of this project can be found in the following Jupyter notebook:  
[project2_solution.ipynb](./project/project2_solution.ipynb)




