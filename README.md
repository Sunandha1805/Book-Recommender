# 📚 Book Recommender Web App

A **machine learning-based book recommendation system** built using **Python, Flask, and Scikit-learn**, that suggests similar books based on user input.
This project uses the [**Book Recommendation Dataset**](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset) from Kaggle and applies **content-based** and **collaborative filtering** techniques.
The web app is deployed live on **Render**.

---

## 🚀 Live Demo

🔗 **[Try the App on Render](https://your-app-link.onrender.com)**
*(Replace with your actual deployed Render URL)*

---

## 🧠 Features

* 📖 **Book Search:** Enter any book title to get similar recommendations.
* ⚙️ **Hybrid Recommendation System:**

  * **Content-Based Filtering:** Uses **cosine similarity** based on book title, author, number of users who rated it, and average rating.
  * **Collaborative Filtering:** Suggests books based on the **average user ratings** of similar readers.
* 🏆 **Top 50 Books Dashboard:** Displays most popular books using **priority ranking** (ratings + votes).
* 💾 **Pickle Integration:** Saves pre-trained ML model files for deployment.
* 🌐 **Web App Interface:** Built using **Flask**, **HTML**, and **CSS** for a simple and interactive UI.
* ☁️ **Deployed on Render:** Fully accessible online.

---

## 🏗️ Tech Stack

| Category             | Technology Used                                                                                             |
| -------------------- | ----------------------------------------------------------------------------------------------------------- |
| Programming Language | Python                                                                                                      |
| Libraries            | Pandas, NumPy, Scikit-learn                                                                                 |
| Framework            | Flask                                                                                                       |
| Model Export         | Pickle                                                                                                      |
| Frontend             | HTML, CSS                                                                                                   |
| Deployment           | Render                                                                                                      |
| Dataset              | [Kaggle: Book Recommendation Dataset](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset) |

---

## ⚙️ Workflow

1. **Dataset Loading:**

   * Imported data from Kaggle including book details, ratings, and user interactions.

2. **Data Cleaning & Preprocessing:**

   * Removed duplicates, handled missing values, and filtered relevant features such as *title, author, ratings count, and average rating.*

3. **Model Development:**

   * Created a **cosine similarity matrix** for content-based recommendations.
   * Implemented **collaborative filtering** using user rating averages.

4. **Model Serialization:**

   * Exported processed data and similarity matrix using `pickle`.

5. **Flask Integration:**

   * Developed `app.py` to handle user requests, process input, and render recommendations dynamically.

6. **Frontend Design:**

   * Created `index.html` and `recommend.html` templates using **HTML** and **CSS**.

7. **Deployment:**

   * Hosted on **Render** for live access.

---

## 📁 Folder Structure

```
Book-Recommender/
│
├── app.py                   # Main Flask application
├── books.pkl                # Processed book dataset
├── similarity.pkl           # Cosine similarity matrix
├── templates/
│   ├── index.html           # Home and dashboard page
│   └── recommend.html       # Recommendation result page
├── static/
│   └── style.css            # Stylesheet
├── da149452-e697-4ba4-bb87-34d6d920f826.ipynb  # ML model Jupyter notebook
├── requirements.txt         # Dependencies
└── README.md                # Documentation
```


## 📊 Example

**Input:** `Harry Potter and the Sorcerer’s Stone`
**Recommended Books:**

* The Hobbit
* Eragon
* Percy Jackson & The Olympians
* The Chronicles of Narnia
* The Golden Compass

---

## 🌟 Future Improvements

* Integrate **Google Books API** for book cover images and descriptions.
* Add **user login and personalized recommendations**.
* Include **genre and author filters**.
* Implement **hybrid model tuning** for better accuracy.

---

## 👩‍💻 Author

**Sunandha**
