# Ai-powered-resume-parser-using-python

# Overview

The AI-Powered Resume Parser is a tool designed to extract key information from resumes and match them with job descriptions using Natural Language Processing (NLP) techniques and machine learning. This project leverages Python, SpaCy, Scikit-learn, and other libraries to provide an intelligent recruitment solution.

# Features

- Resume Parsing: Extracts essential details from resumes such as name, skills, education, and experience.
- Job Description Matching: Compares resumes with job descriptions to generate a match score.
- CSV Output: Results are saved in a CSV file for easy review and analysis.

# Getting Started

# Prerequisites

- Google Colab account
- Basic understanding of Python and NLP

# Setup
1. **Open the Project in Google Colab**:
   - [Open Google Colab](https://colab.research.google.com/).
   - Click on "File" > "Open notebook" > "GitHub".
   - Enter the GitHub repository URL and open the notebook.
2. **Install Required Libraries**:
   Run the following code in a Colab cell to install the necessary libraries:

   **python**
   !pip install spacy nltk scikit-learn pandas
   !python -m spacy download en_core_web_sm

**Explanation of the Code**
**Overview**
The code provides a framework for building an AI-powered resume parser using Natural Language Processing (NLP). It processes resumes and job descriptions to extract key information and calculate the relevance of each resume to the job description. This functionality is implemented using Python and executed in Google Colab.

**Key Components**
**1.Getting Set Up:**

Installing Libraries: We use several libraries like spacy for natural language processing, nltk for extra text handling, scikit-learn for machine learning, and pandas for managing data. These are installed and set up at the start.

**2.Cleaning Up Text:**

Preprocessing: This step involves cleaning the resume and job description texts. We remove any special characters and numbers, convert everything to lowercase, and trim any extra spaces to make sure the text is in good shape for analysis.

**3.Extracting Information:**

Finding Key Details: Using SpaCy’s NLP tools, we extract specific details from the resume text, such as names. This part can be expanded to pull out other information like contact details, skills, education, and work experience.

**4.Comparing Resumes to Job Descriptions:**

Matching Process: We use a technique called TF-IDF to convert the resume and job description into numerical vectors. Then, we calculate how similar these vectors are to each other. This similarity score helps us understand how well the resume matches the job description.

**5.Working with CSV Files:**

Processing Data: The code reads a CSV file with resumes and job descriptions, processes each resume, matches it with the job description, and extracts important details. Finally, it saves all this information, including how well each resume matches the job, into a new CSV file.

**Workflow:**
Setup: Install necessary libraries and download required models.
Preprocessing: Clean and prepare resume and job description texts.
Entity Extraction: Identify and extract relevant entities from resumes.
Matching: Compute similarity scores between resumes and job descriptions.
Output: Save the results, including extracted entities and match scores, into a CSV file for further analysis or reporting.
