# Student Exam Score Prediction
Project is about multilabel classification of different cats and dogs breeds. Data derives from  oxford's pet dataset available [here](https://www.robots.ox.ac.uk/~vgg/data/pets/).


## Preview
![](images/preview.jpg)


## Libraries
Below are presented python packages used for that project:
* `torch` - construction of neural networks
* `numpy` - handling numerical data
* `pandas` - working with tables
* `sklearn` - machine learning tools
* `optuna` - model tuning
* `matplotlib` - the base for plotting
* `seaborn` - more sophisticated, pretty looking graphs


## Project Structure
```txt
├── data/
├── models/
├── images/
├── frontend/
├── notebooks/
│   └── eda.ipynb
├── src/
│   ├── __init__.py
│   ├── preprocessing.py
│   ├── experiment.py
│   ├── tuning.py
│   └── tools.py
├── main.py
├── experiments.md
└── requirements.txt
```

| Component | Description |
| --- | --- |
| `data/` | Directory in which `.csv` files are stored |
| `models/` | Stores models trained from first fold of cross-validation |
| `images/` | Keeps graphs from data analysis and tuning history |
| `frontend/` | Represents web application made in `React` |
| `notebooks/` | Directory with `.ipynb` files for data exploration |
| `eda.ipynb` | Includes exploratory data analysis |
| `src/` | Contains core logic for experiments |
| `preprocessing.py` | Provides data preprocessing column transformer with scaling and encoding |
| `experiment.py` | Enables experimenting with models, saves experiments to `experiments.md` |
| `tuning.py` | Uses `optuna` for specific model tuning |
| `tools.py` | Provides data loading, splitting and other useful methods |
| `main.py` | Core file to start flask server and web application |
| `experiments.md` | Presents whole experiments history |
| `requirements.txt` | Lists libraries required to use this project |


## Configuration
Project has been made using `Python` TODO. Ensure that you also have `npm` installed.

Create Python virtual environment:
```bash
python -m venv venv
```

Then activate it using this command:
```bash
source venv/bin/activate
```

Or if you are on windows paste that:
```bash
./venv/Scripts/activate
```

Ensure to install `requirements.txt` by running the following command:
```bash
pip install -r requirements.txt
```

Download `.csv` data from [here](https://www.robots.ox.ac.uk/~vgg/data/pets/). Ensure that it is placed inside `/data` folder.


## Data Analysis
Firstly I have made some exploratory data analysis to get more familiar with dataset. Data consists of 13 columns, either numerical or categorical. In `eda.ipynb` there are lots of plots showing data distribution and correlations.

Here are a few plots showing relation of some features to the target `exam_score`:
![](images/combined_analysis_chart.jpg)

## Preprocessing



## Models
Models tested (chronologically):



## Experiments



## Tuning


**Optimization history**

![](images/optimization_history.jpg)


## Conclusions
