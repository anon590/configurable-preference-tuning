# Configurable Preference Tuning ⚙️📝

Code for the paper "Configurable Preference Tuning with Rubric-Guided Synthetic Data".

> tl;dr: Configurable Preference Tuning (CPT) uses rubric-guided synthetic data and DPO to enable LLMs to dynamically adjust behavior (e.g., writing style) at inference via system prompts.


## Structure

* `train.py`: fine-tuning code, using the preference data from the experimental section in the paper.

* `rubric_tamplates.py`: the rubrics used for the experiments in the paper.


## Datasets

The synthetic dataset used in the paper is released in the HugginfaceHub, under two different variants:

* [vicgalle/creative-rubrics-preferences](https://huggingface.co/datasets/vicgalle/creative-rubrics-preferences): this is the DPO-compatible version, in which the generations have been arranged into contrasting pairs.
* [vicgalle/creative-rubrics](https://huggingface.co/datasets/vicgalle/creative-rubrics): raw version, each row has the prompt, the rubric and the score target for the rubric, plus the response and the model used to generate it.

## Fine-tuned Models

To be released soon...
