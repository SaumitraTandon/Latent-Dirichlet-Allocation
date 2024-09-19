
# Topic Modeling using LDA on BBC News Dataset

This project demonstrates the application of Latent Dirichlet Allocation (LDA) for topic modeling on the BBC News dataset. The dataset contains news articles and their corresponding categories, and the goal is to uncover the underlying topics within the articles using LDA.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)

## Project Overview
Latent Dirichlet Allocation (LDA) is a generative probabilistic model used to find a mixture of topics that best describe a set of documents. In this project, we apply LDA to a collection of BBC news articles to extract dominant topics and analyze their distribution across different categories of news (e.g., business, sports, politics).

## Dataset
The dataset used for this project is the **BBC News dataset**, consisting of two columns:
- `text`: The full text of news articles.
- `labels`: The category (label) to which each article belongs (e.g., `business`, `sports`).

The dataset is located in the `bbc_text_cls.csv` file.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/topic-modelling-lda.git
   cd topic-modelling-lda
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the `nltk` stopwords:
   ```python
   import nltk
   nltk.download('stopwords')
   ```

## Usage

1. Load the dataset and preprocess the text:
   - Stopwords are removed using the NLTK library.

2. Perform LDA:
   - Use the `LatentDirichletAllocation` class from `sklearn` to model the topics.
   
3. Visualize and interpret the topics:
   - Use the LDA model to extract the dominant topics and analyze their distribution.

To run the analysis, open the `Topic_Modelling_using_LDA.ipynb` notebook and execute the cells step by step.

## Results
The results of the LDA model will display the most frequent words per topic and their respective weights. These results can be used to interpret the key themes within the dataset, such as finance, politics, and more.

Example output:
```
Topic 1: ['company', 'shares', 'market', 'profit', 'stock']
Topic 2: ['government', 'minister', 'policy', 'law', 'election']
...
```

You can visualize the topics using word clouds or other plotting techniques to gain better insights into the content of the news articles.

## Contributing
If you would like to contribute to this project, feel free to fork the repository and submit a pull request. Contributions in the form of bug fixes, additional features, or improved visualizations are welcome.
