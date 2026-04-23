# Text Auto-Completion Project

## Overview

This project implements a simple word-level text auto-completion system using a frequency-based model trained on the WikiText-2 dataset. Given a prefix, the system returns the top-k most frequent matching words. The model is evaluated using simulated typing experiments with metrics such as Top-5 accuracy and keystroke savings.

---

## How to Run the Code

This project was developed in Google Colab.
It is available here as a python file named "autocomplete_project.py".

I had trouble downloading the code from Colab as a ipynb file, so I have made it available here as a python file.
There is a link at the top of the python file to the notebook in Colab. I recommend running it there since it uses a 
relatively large dataset (4.72MB of downloaded dataset files, 13.54MB of generated dataset, and it uses a total of 18.26MB of disk space)

The python file can be run in the terminal with:
`python3 autocomplete.py` or `python autocomplete.py`

There are some sanity checks I left in there to demonstrate how the `get_suggestions` function works.
I put a 'EXPERIMENT STARTS HERE' comment  where the experiment's code starts. There are definitions
for the keystroke savings and accuracy functions, and then there is a section that will run 1 experiment
as a sanity check. At the bottom is where the loop is to repeat the experiment 5 more times.

*Please note that the project code took me about 10 minutes to run*

## Dependencies

The project uses the following Python libraries:

* `datasets` (Hugging Face)
* `collections`
* `re`
* `random`

## Files and Structure

* `autocomplete_project.ipynb` or `autocomplete_project.py`
  Main implementation containing preprocessing, model construction, and evaluation.

* `README.md`
  Project documentation and instructions.

* Output:
  Generated results from experiments, including accuracy and keystroke savings metrics.

---

## Notes

* The model uses a frequency-based prefix matching approach
* Experiment is performed using simulated user typing on sampled words from the dataset.
* Results may vary slightly depending on random sampling.
* Evaluation is based on top-k accuracy and average keystroke savings.
