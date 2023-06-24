# Classifier
## Description
- This project utilizes machine learning to classify images of dogs and cats. It consists of two main components: training a model using Google's Teachable Machine and integrating this model into a Django web application. The deployed application allows users to upload images of dogs or cats, and the model predicts the class of the uploaded image, providing the output on the web interface.
- The project is deployed on Microsoft Azure using Nginx as a web server and Gunicorn as a WSGI HTTP server.

## Table of Contents
- Installation
- Usage
- Technologies
- Screenshots
- Deployment Link


## Installation
To run this project locally, follow these steps:

1.Clone the repository:
```
git clone https://github.com/Tarik-Bhateja/ThaparSummerSchool_2k23.git
```

2.Create Virtual Environment

```
python -m venv 'Your_Environment_Name(without '')'
```

3.Install the required dependencies:
```
pip install -r requirements.txt
```

## Usage

1.Navigate to the project directory:
```
cd ThaparSummerSchool_2k23/ModelDeployment/Classifier
```

2.Start the Django development server:
```
python manage.py runserver
```

3.Access the web application by visiting http://localhost:8000 in your web browser.

4.Upload an image of a dog or a cat and observe the model's classification output on the web interface.

## Technologies
The project utilizes the following technologies:

- Python
- Django
- Google's Teachable Machine
- Microsoft Azure
- Nginx
- Gunicorn

## Screenshots

![Classifier](https://i.imgur.com/d5nNi1r.jpg)
![Classifier](https://i.imgur.com/eXPBSLl.png)
![Classifier](https://i.imgur.com/LM20S7B.png)


## Deployment Link

[WebApp](https://ml.bhateja.tech)
