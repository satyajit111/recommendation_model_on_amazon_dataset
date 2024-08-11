# recommendation_model_on_amazon_dataset

# Amazon Product Search

This repository contains a Python project that implements a text-based search functionality on Amazon product data. The project uses natural language processing (NLP) techniques to preprocess product titles and descriptions, and calculates the cosine similarity between a search query and product data to find the most relevant products.

## Features

- **Data Preprocessing**: The project uses the Natural Language Toolkit (nltk) library for tokenization and stemming of product titles and descriptions.
- **Cosine Similarity**: The project calculates cosine similarity between a user's search query and product data to rank the most relevant products.
- **TF-IDF Vectorization**: The project uses TF-IDF vectorization to transform the text data into numerical features that can be used for similarity calculations.

## Project Structure

- **Import Libraries**: The necessary libraries such as Pandas, NumPy, and NLTK are imported at the beginning of the notebook.
- **Data Loading**: The product data is loaded from a CSV file named `amazon_product.csv`.
- **Data Cleaning**: The data is cleaned by removing unnecessary columns like the `id` column.
- **Text Preprocessing**: A custom function `tokenize_stem` is defined to tokenize and stem the text from product titles and descriptions.
- **Cosine Similarity Function**: A function `cosine_sim` is defined to calculate the cosine similarity between two text inputs.
- **Search Function**: The main function `search_product` takes a query string as input and returns the top 10 most relevant products based on cosine similarity.

## Usage

1. **Load the Data**: Make sure to have your product data in a CSV file named `amazon_product.csv`. The file should contain columns like `id`, `Title`, `Description`, and `Category`.

2. **Run the Notebook**: Execute the Jupyter notebook to run the code cells. This will load the data, preprocess the text, and define the necessary functions.

3. **Search for Products**: Use the `search_product` function by passing a query string to search for relevant products. The function will return a DataFrame with the top 10 most relevant products.

## Example

Here's an example of how to use the search functionality:

```python
# Search for a product
search_product('PURELL ES8 Professional HEALTHY SOAP Foam Refill, Fresh Scent Fragrance, 1200 mL Soap Refill for PURELL ES8 Touch-Free Dispenser (Pack of 2) - 7777-02')
