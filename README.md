# Tango with Django 2 (UofG WAD2 Rango Assessment)

This repository is used for WAD2 Assessment that requires to learn Django Web Framework by reading **Tango with Django 2 by Leif Azzopardi and David Maxwell (Version 2020-01a)**.
Progress is tested through [the Model Solution](https://github.com/maxwelld90/tango_with_django_2_code) by [David Maxwell (maxwelld0)](https://github.com/maxwelld90).

## Using this Repository
Since this repository uses a virtual environment with specific packages, it is essential to activate it specifically.

### Virtual Environment
If you haven't already created a virtual environment, you can do so using either of the following:
* Anaconda Prompt

    `$ conda create -n rango python=3.7.2`

* Python (Windows)

    `$ py -m venv rango`

* Python (macOS / Linux)

    `$ python3 -m venv rango`


You can then activate the environment once created.
* Anaconda Prompt

    `$ conda activate rango`

* Python (Windows)

     `$ .\env\Scripts\activate`

* Python (macOS / Linux)

     `$ source env/bin/activate`


This project uses Anaconda Prompt specifically as instructed.

### Installing packages
A `requirements.txt` file mentions all the packages along with their versions used for this project. You can install them using:

`$ pip install -r requirements.txt`


### Running the App
The main Python file is `manage.py`. The app can be run using

`$ python manage.py runserver`

and then use a browser to go to http://127.0.0.1:8000/


### Running the Tests
As mentioned in [the Model Solution](https://github.com/maxwelld90/tango_with_django_2_code/tree/master/progress_tests), the following needs to be done:
1. The `rango` virtual environment needs to be active.
2. From the model solution repository, the chapter test should be copied to the rango folder on this repository which is at the same level as `manage.py`.
3. Run the following command

    `$ python manage.py test rango.tests_chapterX.py`

    where X is the chapter number. If an error appears mentioning a .py attribute, run

    `$ python manage.py test rango.tests_chapterX`

    The test will mention all fails or print `OK` at the end if the app passes.



## About the Assessment
This repository will be assessed through automated testing.

### Checkpoint 1
The first test, scheduled for 31 January 2020, would include tests for Chapters 3-10. This checkpoint is worth 10% of the overall mark. Passing any chapter test would award full marks.

### Checkpoint 2
The second test, scheduled for 14 February 2020, would include tests for Chapters 3-10 (again), however, all tests must pass. This is worth 90% of the overall mark. In basic terms, the Rango app should be **successfully** completed.

### Commits
It is expected to have **at least** one commit per chapter. Commit times will also be checked as they allow to detect plagiarism. For instance, a GitHub repository where all commits were
made on the same day and over one week, will be flagged, and will be closely inspected through code, commit messages and history to determine course of action.

### Marking Scheme
When the automated tests are run after Rango checkpoint 2, 1 mark will be awarded for each test passed and 0 marks for each test failed (or terminated early due to an error). The total
marks gained will then be expressed as a percentage of the total number of tests N. The percentage P will then be adjusted to take account of the number of commits C made. The overall percentage Q for checkpoint 2 will then be P multiplied by min{C,8}/8. So, for example, for only 4 commits, Q will be P divided by 2.
The final percentage R will be made up of the mark from checkpoint 1 weighted at 10% and the mark (i.e., Q) from checkpoint 2 weighted at 90%. R will then be converted to a band which will be the mark for this component of the assessment.