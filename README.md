GITHUB LINK: https://github.com/meye7066/3832_autocomplete_project.git

COLAB LINK: https://colab.research.google.com/drive/1MWHX6D1b6plaKB9PyenQWJdUelKxCNms

# Text Auto-Completion Project

## Overview

This project implements a simple word-level text auto-completion system using a frequency-based model trained on the WikiText-2 dataset. Given a prefix, the system returns the top-k most frequent matching words. The model is evaluated using simulated typing experiments with metrics such as Top-5 accuracy and keystroke savings.

---

## How to Run the Code

This project was developed in Google Colab and can be accessed here:

COLAB LINK: https://colab.research.google.com/drive/1MWHX6D1b6plaKB9PyenQWJdUelKxCNms

It is available on GitHub as a python file named "autocomplete_project.py".

I had trouble downloading the code from Colab as a ipynb file, so I have made it available here as a python file just in case. There is a link at the top of the python file to the notebook in Colab as well. I recommend running it there since it uses a relatively large dataset (4.72MB of downloaded dataset files, 13.54MB of generated dataset, and it uses a total of 18.26MB of disk space)

If running locally, make sure to check the Dependencies. The python file can be run in the terminal with:
`python3 autocomplete.py` or `python autocomplete.py`

There are some sanity checks I left in there to demonstrate how the `get_suggestions` function works.
I put a 'EXPERIMENT STARTS HERE' comment  where the experiment's code starts. There are definitions
for the keystroke savings and accuracy functions, and then there is a section that will run 1 experiment as another sanity check. At the bottom is where the loop is to repeat the experiment 5 more times.

*Please note that the project code took me about 10 minutes to run*

## Dependencies

The project uses the following Python libraries:

* `datasets` (Hugging Face)
* `collections`
* `re`
* `random`

## Files and Structure

* `autocomplete_project.ipynb` on Colab or `autocomplete_project.py` here on GitHub
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
