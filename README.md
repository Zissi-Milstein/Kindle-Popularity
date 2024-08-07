# 📚 Kindle Popularity - Exploring the Rise of Bestsellers

**Contributors**: Zissi Milstein, Daniella Berger

Welcome to Kindle Data, a comprehensive dataset capturing the essence of Kindle books across diverse genres and captivating themes. Each book is uniquely identified by its ASIN (Amazon's ISBN), accompanied by key details such as title, author, ratings, reviews, and category information.

## 🌟 Overview

Our data, referred to as Kindle Data, encompasses books spanning various genres, countries, and themes. The category column indicates the book's genre or theme. Our exploration delves into the dynamics of book categorization, ranging from broad genres like "Literature and Fiction" to more specific themes. We also analyze factors contributing to a book's popularity, including awards, pricing, and Kindle Unlimited availability.

### Objectives
We aim to analyze how different factors such as genre, authorship, awards, pricing, and Kindle Unlimited availability influence the popularity of Kindle books.

## 📋 Dataset Columns

- **ASIN (Amazon's ISBN)**: Unique barcode for each book on Amazon stored as a string/object. (It's a mix of letters and numbers)
- **Title**: The book's title. (string/object)
- **Author**: The author of the book. (string/object)
- **Img_url**: Link to the book's cover page. (string/object)
- **Product_url**: Link to the book's page on Amazon. (string/object)
- **Stars**: Number of stars (out of five) the book received on Amazon. (float/number)
- **Reviews**: Number of reviews the book received on Amazon. (integer)
- **Category_id**: Amazon's numerical categorization of books. (integer)
- **IsEditorsPick**: Indicates if the book is an Editor's Pick on Amazon. (boolean/true or false/ later converted to an integer)
- **IsGoodReadsChoice**: Indicates if the book won the Goodreads Choice Awards. (boolean/true or false/ later converted to an integer)
- **Published date**: Date the book was published. (object/ later converted to date)
- **Category name**: The category the book belongs to. (string/object)
- **IsBestseller**: Binary indicator if the book is a bestseller. (boolean/true or false/ later converted to an integer)
- **Price**: The cost of the book. (float/number)
- **IsKindleUnlimited**: Indicates if the book is part of Kindle Unlimited. (boolean/true or false/ later converted to an integer)

## 🛠️ Data Cleaning

### Steps:
1. **Removing Duplicates**: While Amazon does not allow two books to be registered with the same ASIN, some book titles appeared more than once. We retained duplicates only when they shared titles and authors, ensuring we kept the newest version of each book.
2. **Handling N/A Values**: We encountered very few N/A values and did not drop any, except for null values in the date category, which we did not use due to reliability concerns.
3. **Categorization Fixes**: Discrepancies in book categorization, especially in the Romance and Literature and Fiction categories, were addressed by reassigning books with the word "romance" in the title to the Romance category.

## 🔍 Analysis

The central concept of our analysis is identifying key factors contributing to a book's bestseller status, such as genre, ratings, awards, pricing, and Kindle Unlimited availability. We also acknowledge the influence of Amazon's recommendation algorithm.

### Visualizations

We utilized various data visualization tools to explore this topic thoroughly:
- **Histograms** 📊
- **Bar Charts** 📊
- **Line Charts** 📈
- **Heat Maps** 🌡️

For detailed code and cleaned data, refer to our code repository.

### Machine Learning Techniques

We employed the following machine learning techniques:
- **T-test**
- **Welch’s Test**
- **Logistic Regression**
- **Random Forest**

## 📊 Dashboard Creation

Our dashboard is designed with book publishers in mind, providing insights into Kindle books' success as bestsellers. Our Key Performance Indicator (KPI) is the percentage of books that are bestsellers compared to the total number of books in the Kindle Data, which stands at 1.66%. Graphs illustrating these points are available in Tableau.

## ⚖️ Ethical Concerns

We acknowledge ethical considerations regarding anonymized reviews and Amazon's recommendation system, which may impact data interpretation and book popularity.

## 🏁 Conclusion

This project has enriched our skills in data cleaning, analysis, visualization, and understanding Kindle bestsellers.

Thank you for exploring the rise of bestsellers with us!
