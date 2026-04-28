## Topic Modeling & Sentiment Analysis of Appliance Reviews

1. Project Overview : This project applies Natural Language Processing (NLP) to a dataset of washing machine reviews of Amazon Appliance Reviews to uncover what drives customer satisfaction and brand loyalty. By combining Latent Dirichlet Allocation (LDA) for topic discovery with VADER Sentiment Analysis, we bridge the gap between numerical star ratings and actual user experience. This analysis is critical for manufacturers and retailers to identify mechanical pain points—like vibration and reliability—that disproportionately influence consumer purchasing decisions through "helpful" social proof.
   
2. Main Deliverable👉 The main deliverable is main_notebook.ipynb
3. Research Questions
   - RQ1: Which product features are most important to customers based on discussion frequency and community influence (helpful votes)?
   - RQ2: How does customer sentiment vary across different product aspects (e.g., Reliability vs. Ease of Use)?
   - RQ3: To what extent do star ratings align with textual sentiment, and what do inconsistencies reveal about data reliability?
     
4. Data Section
   Dataset: [https://amazon-reviews-2023.github.io/].
   Preprocessing:Tokenization and removal of stop words.
   Lemmatization using NLTK/SpaCy to normalize technical terms (e.g., "broken" $\rightarrow$ "break").
   Bigram/Trigram creation (e.g., "spin_cycle", "easy_install").
   Aspect-based filtering using a custom feature dictionary.
   
6. How to Reproduce: This project was built in Google Colab.
   To reproduce the results:
   - Clone this repository.
   - Install dependencies: pip install -r requirements.txt.
   - Open the main notebook in Colab or Jupyter.
   - Run cells in sequential order.
 7. Key Dependencies 🌱
    - Python 3.12.13
    - Pandas 2.1.0
    - NLTK 3.8.1
    - Gensim 4.3.2 (for LDA Modeling)
    - vaderSentiment 3.3.2 (for Sentiment Analysis)
 8. Repo Structure
├── notebooks/              
│   ├── checkpoint_1.ipynb  # first checkpoint of the project
    ├── checkpoint_2.ipynb  # Second checkpoint of the project
│   └── main_notebook.ipynb  # Primary analysis & results
├── requirements.txt        # Full list of dependencies


8. Results Summary ✨
   - The "Utility-Reliability Gap": While Capacity & Load are the most discussed and highly-rated features, Reliability issues (noise, vibration, and mechanical failure) carry the most weight in community influence.
   - Despite high overall sentiment, inconsistent reviews (where ratings contradict text) reveal that technical frustrations often go unnoticed when looking at star ratings alone.

