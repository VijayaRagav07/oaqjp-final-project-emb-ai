# Repository for final project

## Emotion Detector

This project is a Flask-based web application that uses the IBM Watson NLP Emotion Prediction API to analyze the emotional content of user-provided text.

### Features

* Detects the following emotions:

  * Joy
  * Anger
  * Disgust
  * Fear
  * Sadness
* Determines the dominant emotion.
* Handles blank input gracefully.
* Includes unit tests.
* Supports static code analysis with PyLint.
* Deploys the application locally using Flask.

### Project Structure

```
oaqjp-final-project-emb-ai/
│
├── EmotionDetection/
│   ├── __init__.py
│   ├── emotion_detection.py
│   └── test_emotion_detection.py
│
├── static/
│   └── mywebscript.js
│
├── templates/
│   └── index.html
│
├── server.py
├── README.md
└── LICENSE
```

### Requirements

* Python 3.x
* Flask
* Requests

Install dependencies:

```bash
pip install flask requests pylint
```

### Run the application

```bash
python server.py
```

Open your browser and visit:

```
http://localhost:5000
```

### Example Output

Input:

```
I love my life.
```

Output:

```
For the given statement, the system response is 'anger': 0.006274985, 'disgust': 0.0025598293, 'fear': 0.009251528, 'joy': 0.9680386 and 'sadness': 0.049744144. The dominant emotion is joy.
```

### Author

IBM Skills Network Final Project
