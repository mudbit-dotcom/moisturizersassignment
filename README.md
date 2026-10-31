# This is an ingredient analysis of moisturizers available on Sephora.com on March 2023.

The data was found from this dataset from Kaggle via python scraper: https://www.kaggle.com/datasets/nadyinky/sephora-products-and-skincare-reviews?resource=download

## Methodology

I first had to break down the data from its multiple categories. I decided to intially to filter for product_name, brand_name, ingredients, and price_usd just to get an idea of what I'm working with

I then filtered for moisturizers. Using Claude, I created a dictionary of moisturizer_ingredients by using the defaultdict function. Cladue then cleaned and parse the raw ingredient data by using the split_outside_parens(text) to split commas outside of parenthesis and the clean(ing) function to standarize spelling variations.

parse_ingredients(raw) returns everything into a clean Python list.

## Outputs

You can see the outputs of the full data set which contains fragrance, skincare, haircare and more in product_info.csv

## Running the analysis yourself

You can run the analysis yourself. To do so, you'll just need python and either Microsoft Excel or Google sheets to access the .csv file.


## License
All code in this repository is available under the MIT License. The data file in the output/ directory is available under the Creative Commons Attribution 4.0 International (CC BY 4.0) license. All files in the data/ directory are released into the public domain.