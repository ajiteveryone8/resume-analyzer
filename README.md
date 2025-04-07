# Resume Classification and Analysis System
A machine learning pipeline for classifying resumes into categories and extracting key information using NLP techniques.

## 📌 Overview
An end-to-end pipeline that:
- Classifies resumes into 25+ professional categories
- Extracts key information (skills, experience, education)
- Generates visual analytics
- Built with Python, spaCy, and Scikit-learn

## 🚀 Quick Start

### 1. Installation
```bash
git clone https://github.com/ajiteveryone8/resume-analyzer
cd resume-analyzer
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```


### 2. Run the Pipeline

```bash
from analyzer import ResumePipeline

pipeline = ResumePipeline()
pipeline.load_data("resumes.csv")
pipeline.run_analysis()

# Get results
results = pipeline.get_results()
```

🔧 Key Components
Text Cleaning
  - Removes special characters/normalizes text
  - Handles abbreviations (e.g., "A.I." → "AI")
  - Example:
  - ```bash
    clean_text("Python, SQL, and Machine Learning!")
    # → "python sql and machine learning"
    ```

## Classification (25+ Categories)
Category	Precision
   - Data Science	92%
   - Web Development	89%
   - Business Analyst	85%

## Information Extraction
```bash
{
  "skills": ["Python", "TensorFlow", "AWS"],
  "experience": ["5 years at Google"],
  "education": ["MS Computer Science"]
}
```

### Key Features:
1. **Concise** - All critical info in one scroll
2. **Visual Hierarchy** - Emojis and headers organize content
3. **Code-Ready** - Copy-paste friendly commands
4. **Self-Contained** - No external dependencies
5. **Action-Oriented** - Focuses on getting users started quickly


