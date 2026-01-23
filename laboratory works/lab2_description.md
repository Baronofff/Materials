# Lab 2. Solving Advanced NLP Tasks with RNNs

## Tasks
> _Multilabel classification_

> _Regression_

In this laboratory work you need to complete a multilabel classification task or regression task using neural networks with recurrent layers.

- Version 1: Movie genres identification (multilabel classification)
- Version 2: Movie rating prediction (regression)

Every student completes one of the two versions of laboratory work, a student can see what version they must complete in the table in the "[Versions](#versions)" block.

## Dataset
> _Please, refer to the link below for data downloading and additional information on dataset_.

Dataset (same for both versions): [Movie plots from Wikipedia in Russian](https://www.kaggle.com/datasets/maksimpotorochin/movie-plots-from-wikipedia-in-russian)

**What columns to use**

In the table below you can see what columns in the dataset you should use in accordance with the version you are given. "Target" row defines the target column in the dataset containing labels/values you should predict, the "Source" row defines the columns you should use as feature source.

|Type|Version 1|Version 2|
|---|:---:|:---:|
|Target|"genre"|"imdb_rating"|
|Source|"plot"|Any columns|

## Pipeline
> *This time there won't be any strictly defined steps to take, do whatever you think is useful for completing your task, but please follow the pipeline below.*

1. **EDA**: check basic statistical information over the dataset and try to learn specific info for your task to get helpful insights. Don't forget to remove/fill empty values and take steps to prevent data leak.
2. **Preprocessing**: prepare source texts and labels if needed, apply any data transformations you find suitable. Students working on multilabel classification task should define the labels they will learn to predict (minimum 5).
3. **Indexation**: in order to work with RNN you must first prepare a dictionary and convert each text into list of indexes. 
4. **Vectorization**: use any word-level vectorization technique, explain your choice.
5. **Baseline**: first, fit a simple regression model and measure* its performance.
6. **Neural Network**: then, build a neural network with recurrent layers, train it, find optimal architecture/hyperparameters, assess* its performance and compare it with baseline performance. 

\* You can use standard classification metrics (precision, accuracy, F1-score) to assess model's performance on multilabel classification task and mean average error (MAE)/ mean squared error (MSE) for regression task. Additionally, you can refer to [sci-kit learn's metrics list](https://scikit-learn.org/stable/modules/model_evaluation.html#string-name-scorers) to choose the appropriate metric for your task (please, explain your metric choice if you use some other metric instead of the mentioned here).

## Additional Materials
If you need examples, I recommend you to have a look at the following notebooks:
- **Multilabel classification:**
    - [Multi-label classification with neural networks](https://www.kaggle.com/code/residentmario/multi-label-classification-with-neural-networks/notebook) — a simple pipeline with comments that shows how to conduct multilabel classification.
    - [Extreme Multilabel Text Classification 12 models](https://www.kaggle.com/code/supasunkumpraphan/extreme-multilabel-text-classification-12-models) — a big notebook with experiments on basic ML models and neural networks (has LSTM example).
- **Regression:**
    - [Regression with Neural Networks using PyTorc](https://www.kaggle.com/code/stefancomanita/regression-with-neural-networks-using-pytorc) — can be used as a simple pipeline reference.
    - [Deep neural networks for spectral data regression with TensorFlow](https://nirpyresearch.com/deep-neural-networks-spectral-data-regression-tensorflow/) — here you can look at what metrics can be used for the task.

The example are not ideal, but they should help you to get a basic understanding of how to conduct the given tasks.

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
- Low-level implementation of attention layer with basic functions. Your layer must be compatible with your neural network, activation functions, etc. and tested in action, i.e. it must be appropriately used in your neural network.
- Implementation of analysis method for assessment of words influence on predictions. Check LIME algorithm ([paper](https://arxiv.org/pdf/1602.04938), [GitHub](https://github.com/marcotcr/lime))

## Versions
|Student|Variant|
|-------|-------:|
|Азимкова Анна Дмитриевна|2|
|Баронов Евгений Евгеньевич|1|
|Вельмисова Маргарита Николаевна|2|
|Ермак Елена Игоревна|2|
|Зайцев Денис Владимирович|1|
|Карпова Алиса Анатольевна|2|
|Логунова Анастасия Ильинична|1|
|Мокина Марина Сергеевна|2|
|Нагорная Ульяна Алексеевна|2|
|Нуртдинова Софья Алексеевна|1|
|Онофриенко Софья Андреевна|1|
|Переяславцева Ирина Сергеевна|1|
|Савина Арина Сергеевна|2|
|Угольников Вячеслав Александрович|1|
|Хомутова Екатерина Сергеевна|2|

## Deadlines
- Soft — 07.02.26
- **Strict — 08.02.26** (1 point penalty)

## Upload link
> https://forms.yandex.ru/u/696a5de249363924495b4cd1

**NB!** The form will automatically close on 08.02.26 at 23:59 and you won't be able to send your work!
