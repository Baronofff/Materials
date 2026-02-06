# Lab 3. Advanced Machine Translation

## Task

> _Code to text translation_

In this laboratory work you need to train a neural network to generate docstrings for python functions.

## Dataset
> _Please, refer to the link below for data downloading and additional information on dataset_.

- [google/code_x_glue_ct_code_to_text](https://huggingface.co/datasets/google/code_x_glue_ct_code_to_text).

Use subset for Python.

## Pipeline
> *Once again, there is no strictly defined steps to take, do whatever you think is useful for completing your task, your basic pipeline can look as follows:*
1. **EDA**: check the dataset for any missing values, check the texts to get the idea of what you're going to work with, check for any broken texts.
2. **Preprocessing**: prepare text data if needed.
3. **Vocabulary preparation**: prepare a vocabulary for both natural text and code examples. Pay attention to not allow data leakage.
4. **Indexation**: prepare word indices.
5. **Vectorization**: use a trainable vectorizer or use pretrained vectors.
6. **Build and train neural network**.
7. **Assess generation** - you can use standard translation metrics to assess the generation quality (BLEU, Rouge, etc.) Also, please manually check and analyse some of the generation examples (from test set or for your custom input).

## Formal Requirements
- Reproducibility
- Adequacy
- Comments and descriptions
- Conclusions
- Adequate code execution time (checkpoints)
- Adequate model sizes
- Absence of overfitting*
- Plagiarism is forbidden
- Inappropriate use of dataset splits will result in penalties
- Use `PyTorch` framework to work with neural networks

## Bonus Task
Student can make an additional task to get a mark for bonus part. Students can suggest their own tasks or try to complete the one given as an example. **Students must inform their instructor of their willingness to complete a bonus task beforehand!**

A student gets:
- A full bonus task mark if they completed the bonus task successfully, some minor shortcomings are acceptable.
- A half of bonus task mark if they tried to complete the tasks, but made serious mistakes that affected the results.

### Example bonus tasks for this laboratory work:

- Apply bytepair encoding (BPE) by writing your own tokenizer. Use it in your pipeline.

## Deadlines
- Soft — 28.02.26
- **Strict — 01.03.26** (1 point penalty)

## Upload link
> https://forms.yandex.ru/u/6985f66b90fa7b3e71546094

**NB!** The form will automatically close on 01.03.26 at 23:59 and you won't be able to send your work!