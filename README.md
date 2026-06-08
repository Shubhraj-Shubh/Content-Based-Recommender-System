# Content-Based Movie Recommender System

An end-to-end machine learning project that recommends movies based on content similarity. It utilizes the TMDB 5000 Movie Dataset to extract contextual metadata and computes multi-dimensional semantic distances using Cosine Similarity.

## 🚀 System Architecture
*   **Data Processing:** Extracted and cleaned nested JSON metadata (genres, cast, crew) using Pandas.
*   **Vectorization:** Implemented `CountVectorizer` (Bag-of-Words) to convert text tags into a 5,000-dimensional feature matrix.
*   **Similarity Engine:** Computed `cosine_similarity` to find nearest neighbors with O(1) inference time via serialized `.pkl` matrices.
*   **Frontend & API:** Built an interactive web interface using Streamlit, integrating the TMDB REST API to dynamically fetch movie posters.

## ⚙️ How to Run Locally

1. **Clone the repository:**
```bash
   git clone https://github.com/Shubhraj-Shubh/Content-Based-Recommender-System.git
   cd Content-Based-Recommender-System
 ``` 
2. **Install dependencies:**
```bash
   pip install -r requirements.txt
   ```
3. Generate the Similarity Matrix:
Run all cells in model_training.ipynb to process the data and generate the movie_list.pkl and similarity.pkl files inside a /model directory.

Run the Streamlit App:

```bash
   streamlit run app.py
   ```
