# Lab 1. Basic Text Classification Methods

## Task
> _Binary/Multiclass classification_

In this laboratory work you need to complete a classification task using fully connected neural network models.

- Variant 1: Fake news detection (binary classification)
- Variant 2: Authorship identification (multiclass classification)

## Datasets
> _Unfortunately, I cannot upload dataset files directly on github due to file size limits. Please, refer to the links below for downloading and for additional information on datasets_.
- Variant 1: [Fake News](https://www.kaggle.com/datasets/hassanamin/textdb3)
- Varinat 2: [AuthorsTexts](https://www.kaggle.com/datasets/tatianafofanova/authorstexts)

|Brief description|Variant 1|Variant 2|
|-----|:-----:|:-----:|
|Task|Binary classification|Multiclass classification|
|$n$ Samples|$6335$|$65152$|
|$n$ Classes|$2$|$38$*|
|Lang|en|ru|
|Target column|label|writer|

\*Please, truncate the dataset, leaving only $5$ most frequently occuring authors in train set.

## Pipeline and tasks
1. **EDA**
    - **Dataset overview**: check size, number of classes, balance, average text length.
    - **Inspect text quality**: manually inspect a random sample of texts from each class. Write down your observations.
    - **Quantitative Checks**: check the number of duplicates, missing values. Plot a histogram of text lengths.
2. **Preprocessing**
    - Fix any problems you’ve found during EDA step
    - Apply any data transformations you find suitable (punctuation removal, stemming/lemmatization, etc.)
3. **Vectorization**
    - Apply the following vectorization techniques: TF-IDF, Word2Vec, FastText.
    - Apply a PCA method to your vectors.
    - Visualize and explore the vectors you’ve got. Make comparisons.
    - Choose one vector type for experiments and explain your choice.
4. **Classification**
    - Split the dataset, choose relevant metrics for the task.
    - If you've chosen Word2Vec or FastText embeddings, get the text embeddings by taking the mean of appropriate words embeddings.
    - Take logistic regression as a baseline model.
    - Try to find an optimal architecture for your neural network (Use the correct split for experiments).
    - Demonstrate how your model works: show examples of you model's outputs and compare them to true labels.

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

## Bonus Task
Student can make an additional task to get a mark for bonus part. Students can suggest their own tasks or try to complete the one given as an example. The bonus task must be discussed with the teacher beforehand!

A student gets:
- A full bonus task mark if they completed the bonus task successfully, some minor shortcomings are acceptable.
- A half of bonus task mark if they tried to complete the tasks, but made serious mistakes that affected the results.

### Example bonus tasks for this laboratory work:
- Low-level implementation of linear layer with basic functions. Your layer must be compatible with your neural network, activation functions, etc. and tested in action, i.e. it must be appropriately used in your neural network.
- Implementation of cross-validation.

## Variants
|Student|Variant|
|-------|-------:|
|Азимкова Анна Дмитриевна|2|
|Баронов Евгений Евгеньевич|1|
|Вельмисова Маргарита Николаевна|2|
|Ермак Елена Игоревна|1|
|Зайцев Денис Владимирович|1|
|Карпова Алиса Анатольевна|1|
|Логунова Анастасия Ильинична|2|
|Мокина Марина Сергеевна|1|
|Нагорная Ульяна Алексеевна|2|
|Нуртдинова Софья Алексеевна|2|
|Онофриенко Софья Андреевна|2|
|Переяславцева Ирина Сергеевна|1|
|Савина Арина Сергеевна|2|
|Угольников Вячеслав Александрович|1|
|Хомутова Екатерина Сергеевна|1|

## Deadlines
- Soft — 09.01.26
- **Strict — 10.01.26**

## Upload link
> https://forms.yandex.ru/u/693c5582eb614640007ef9f7

**NB!** The form will automatically close on 10.01.26 at 23:59 and you won't be able to send your work!