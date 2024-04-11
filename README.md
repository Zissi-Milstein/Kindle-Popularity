Zissi Milstein
Daniella Berger

## Title: Kindle Popularity - Exploring the Rise of Bestsellers

Welcome to Kindle Data, a comprehensive dataset capturing the essence of Kindle books across diverse genres and captivating themes. Each book is uniquely identified by its ASIN (Amazon's ISBN), accompanied by key details such as title, author, ratings, reviews, and category information.

Our data, referred to as Kindle Data, encompasses books spanning various genres, countries, and themes. The category column indicates the book's genre or theme. Our exploration delves into the dynamics of book categorization, ranging from broad genres like "Literature and Fiction" to more specific themes. We also analyze factors contributing to a book's popularity, including awards, pricing, and Kindle Unlimited availability.

We aim to analyze how different factors such as genre, authorship, awards, pricing, and Kindle Unlimited availability influence the popularity of Kindle books.

Below is a list of the columns included in the dataset and the information they contain:

1. ASIN (Amazon's ISBN): Unique barcode for each book on Amazon stored as a string/object. (It's a mix of letters and numbers)
2. Title: The book's title. (string/object)
3. Author: The author of the book. (string/object)
4. Img_url: Link to the book's cover page. (string/object)
5. Product_url: Link to the book's page on Amazon. (string/object)
6. Stars: Number of stars (out of five) the book received on Amazon. (float/number)
7. Reviews: Number of reviews the book received on Amazon. (integer)
8. Category_id: Amazon's numerical categorization of books. (integer)
9. IsEditorsPick: Indicates if the book is an Editor's Pick on Amazon. (boolean/true or false/ later converted to an integer)
10. IsGoodReadsChoice: Indicates if the book won the Goodreads Choice Awards. (boolean/true or false/ later converted to an integer)
11. Published date: Date the book was published. (object/ later converted to date)
12. Category name: The category the book belongs to. (string/object)
13. IsBestseller: Binary indicator if the book is a bestseller. (boolean/true or false/ later converted to an integer)
14. Price: The cost of the book. (float/number)
15. IsKindleUnlimited: Indicates if the book is part of Kindle Unlimited. (boolean/true or false/ later converted to an integer)

Cleaning the data:

Our initial step involved removing duplicates. While Amazon does not allow two books to be registered with the same ASIN, some book titles appeared more than once. We retained duplicates only when they shared titles and authors, ensuring we kept the newest version of each book.

We encountered very few N/A values in the dataset and did not drop any, except for null values in the date category, which we did not use due to reliability concerns.

When reviewing the data, we observed discrepancies in book categorization, especially in the Romance and Literature and Fiction categories. To address this, we implemented a query to reassign books with the word "romance" in the title to the Romance category.

The central concept of our analysis is identifying key factors contributing to a book's bestseller status, such as genre, ratings, awards, pricing, and Kindle Unlimited availability. We also acknowledge the influence of Amazon's recommendation algorithm.

We utilized various data visualization tools, including histograms, bar charts, line charts, and heat maps, to explore this topic thoroughly.

For detailed code and cleaned data, refer to [our code](https://github.com/Zissi-Milstein/Kindle-Popularity).

We employed T-test, Welch’s test, Logistic Regression, and Random Forest as part of our machine learning analysis.

Dashboard Creation:

Our dashboard is designed with book publishers in mind, providing insights into Kindle books' success as bestsellers.

Our Key Performance Indicator (KPI) is the percentage of books that are bestsellers compared to the total number of books in the Kindle Data, which stands at 1.66%. 
Graphs illustrating these points are available in [Tableau](https://public.tableau.com/app/profile/z.milstein/viz/DataVisualizationFinalProject_17120222037040/KindlePopularity).

Ethical Concerns:

We acknowledge ethical considerations regarding anonymized reviews and Amazon's recommendation system, which may impact data interpretation and book popularity.

In conclusion, this project has enriched our skills in data cleaning, analysis, visualization, and understanding Kindle bestsellers.





