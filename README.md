```markdown
# CareerBridge — AI-Powered Resume & Job Match Platform

CareerBridge is an intelligent web application that helps users understand how well their resume matches real job descriptions.  
It uses **Natural Language Processing (NLP)** and **Machine Learning** to analyze resumes, extract key skills, and provide:
- Match scores against multiple job postings
- Missing skill insights
- Tailored career recommendations

---

## Features

- **Resume Upload:** Upload your PDF resume directly through the interface.  
- **Skill Extraction:** Uses NLP (spaCy / transformers) to identify and categorize skills.  
- **AI Job Matching:** Compares resumes to job postings using TF-IDF or BERT embeddings.  
- **Match Score Dashboard:** Displays top job matches with skill match percentages.  
- **Improvement Suggestions:** Highlights missing skills and provides career insights.  
- **Future Enhancements:** GPT-powered resume rewriting & real-time job integration via Job APIs.

---

## Project Structure

```

careerbridge/
│── app.py                  # Flask backend
│── model.py                # AI/NLP logic
│── utils.py                # Helper functions (PDF parsing, preprocessing)
│── requirements.txt        # Dependencies
│── README.md               # Documentation
│
├── data/
│   └── jobs.csv            # Job postings dataset
│
├── templates/
│   ├── index.html          # Upload form
│   └── results.html        # Results page
│
└── static/
└── style.css           # Custom styling

````

---

## Tech Stack

| Category | Technology |
|-----------|-------------|
| **Backend** | Flask / FastAPI |
| **NLP** | spaCy, scikit-learn, sentence-transformers |
| **Parsing** | PyPDF2 / pdfplumber |
| **Data Handling** | Pandas, NumPy |
| **Frontend** | HTML, CSS, Bootstrap |
| **Visualization** | Plotly, Matplotlib |
| **Deployment (optional)** | Render / Streamlit Cloud |

---

## Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/inezalutgardis/careerbridge.git
   cd careerbridge
````

2. **Create and activate a virtual environment**

   ```bash
   python3 -m venv venv
   source venv/bin/activate   # For Mac/Linux
   venv\Scripts\activate      # For Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the app**

   ```bash
   python app.py
   ```

5. **Open in browser**
   Visit: `http://127.0.0.1:5000`

---

## Example Output (coming soon)

| Job Title    | Match Score | Matched Skills       | Missing Skills     |
| ------------ | ----------- | -------------------- | ------------------ |
| Data Analyst | 87%         | Python, SQL, Tableau | PowerBI, Excel     |
| ML Engineer  | 74%         | Python, Scikit-learn | TensorFlow, Docker |

---

## Future Enhancements

* Integration with JobRight API for real-time listings.
* GPT-powered resume rephrasing.
* Skill recommendations via embeddings & clustering.
* Streamlit dashboard deployment.

---

## Author

**Lutgardis Ineza Ukangutse (Beck)**
Aspiring Computer Scientist | AI & Data Enthusiast
Northwestern University Alum
📧 [inezalutgardis@gmail.com](mailto:inezalutgardis@gmail.com)

---

## License

This project is licensed under the **MIT License** — feel free to use and modify for learning and research purposes.

````
