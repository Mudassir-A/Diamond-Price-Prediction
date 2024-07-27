## Diamond Price Prediction with Flask

This project utilizes Flask to create a web application for predicting diamond prices based on various diamond characteristics.

### Project Structure
```
diamond_price_prediction/
├── app.py
├── artifacts
│   ├── model.pkl
│   ├── preprocessor.pkl
│   ├── raw.csv
│   ├── test.csv
│   └── train.csv
├── notebooks
│   ├── EDA.ipynb
│   ├── data
│   │   └── gemstone.csv
│   └── model_training.ipynb
├── requirements.txt
├── setup.py
├── src
│   ├── __init__.py
│   │   ├── __init__.py
│   │   ├── exception.py
│   │   ├── logger.py
│   │   └── utils.py
│   ├── components
│   │   ├── __init__.py
│   │   │   ├── __init__.py
│   │   │   ├── data_ingestion.py
│   │   │   ├── data_transformation.py
│   │   │   └── model_trainer.py
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   ├── exception.py
│   ├── logger.py
│   ├── pipelines
│   │   ├── __init__.py
│   │   ├── __pycache__
│   │   │   ├── __init__.py
│   │   │   └── prediction_pipeline.py
│   │   ├── prediction_pipeline.py
│   │   └── training_pipeline.py
│   └── utils.py
└── templates
    ├── form.html
    └── index.html
```

### Dependencies

This project requires the following Python libraries:

* Flask
* Scikit-Learn
* Pandas
* Numpy


These dependencies are listed in the `requirements.txt` file.

### Usage

**1. Setting Up the Environment**

Create a virtual environment to isolate project dependencies:

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate.bat  # Windows
```

**2. Install Dependencies**

Install the required libraries from the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

**3. Setting up the environment**

Setup project directory

```bash
python setup.py install
```

**4. Run the Application**

Navigate to the project directory and run the Flask application:

```bash
python app.py
```

This will launch the Flask development server, typically accessible at `http://127.0.0.1:5004/` by default. You can then visit this URL in your web browser to interact with the application.


### Additional Notes

* The `app.py` file will contain the Flask application logic, defining routes, handling user input, and making predictions using your chosen machine learning model.
* The `templates/` directory contains the HTML templates for your web interface.
* The `static/` directory can store static files like CSS stylesheets and JavaScript code used in your web application.

