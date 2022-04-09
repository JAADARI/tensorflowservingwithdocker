# tensorflowservingwithdocker
Serve and deploy text classification model with TensorFlow Serving , Docker and Perform model inference with REST

# Docker commands used to pull the tensorflow/serving image and to run the container :

docker pull tensorflow/serving

docker run -p 8500:8500
-p 8501:8501
--mount type=bind,\ source=amazon_review/,\ target=/models/amazon_review
-e MODEL_NAME=amazon_review
-t tensorflow/serving


