---

layout: page
title: Book Recommendation System
description: A book recommendation system using collaborative filtering with a Streamlit frontend.
img: assets/img/frontend.png
category: Machine Learning

---



### Features
- Collaborative filtering for personalized book recommendations.
- Interactive Streamlit web interface.
- Utilizes book ratings, book information, and user details for recommendations.

### Dataset
- **Books**: Includes details like author, title, and publication year.
- **Users**: Contains user IDs and locations.
- **Ratings**: Ratings provided by users for various books.

### Preprocessing
- Removed unnecessary columns.
- Renamed columns for ease of use.
- Filtered to include users with at least 200 ratings and books with at least 50 ratings.

### Collaborative Filtering
Collaborative filtering is a method used to make automatic predictions about the interests of a user by collecting preferences or taste information from many users. The underlying assumption of the collaborative filtering approach is that if a person A has the same opinion as a person B on an issue, A is more likely to have B's opinion on a different issue than that of a randomly chosen person.

In this project, collaborative filtering is used to find similarities between users based on their book ratings. Books are then recommended to a user based on the ratings from similar users. This technique helps in making personalized book recommendations even when the user has not rated many books themselves.

### Model Building
- Created a pivot table with user IDs as columns, book titles as rows, and ratings as values.
- Converted the pivot table to a sparse matrix.
- Trained a Nearest Neighbors model using the sparse matrix.

### Streamlit Interface
- Select a book from the dropdown menu.
- Click the "Show Recommendation" button to view recommended books and their images.

### GitHub Repository

Explore the source code and contribute to the project on GitHub:
<a href="https://github.com/ughrima/Book-Recommendation" class="btn btn-secondary" target="_blank">View on GitHub</a>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/frontend.png" title="Book Recommendation System Interface" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Above are sample recommendations for the book "1984". 
</div>

### Conclusion
The system effectively recommends books based on user preferences and provides an intuitive interface for obtaining book suggestions.

---