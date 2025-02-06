# AI-Powered Job Matching System

A sophisticated job-candidate matching system using NLP and Machine Learning to match job postings with candidate profiles, featuring semantic understanding and multi-criteria matching.

## Quick Setup Guide

### 1. Environment Setup

```bash
# Create and activate a new conda environment
conda create -n job_matching python=3.8
conda activate job_matching

# Install required packages
pip install pandas numpy scikit-learn gensim spacy streamlit plotly thefuzz

# Download required spaCy model
python -m spacy download en_core_web_sm
2. Running the Notebook
Open Jupyter Notebook:
BASH

jupyter notebook
Navigate to the notebook file and open it

Run all cells:

Click "Kernel" in the top menu
Select "Restart & Run All"
Click "Restart and Run All Cells" in the confirmation dialog
3. Expected Output
The notebook will:

Process job postings and candidate profiles
Generate match scores based on multiple criteria
Display interactive visualizations for:
Overall match scores
Detailed score breakdowns
Top candidate comparisons
Features
Advanced NLP Processing: Uses spaCy and Word2Vec for semantic understanding
Multi-criteria Matching: Considers skills, education, experience, location, and salary
Interactive Visualizations: Plotly-based visualizations for match analysis
Comprehensive Scoring: Weighted scoring system with fuzzy matching
Data Structure
The system processes:

5 job positions (WordPress Developer, Graphic Designer, etc.)
11 candidate profiles with varying skills and experience
Multiple matching criteria including:
Technical skills
Education requirements
Experience levels
Location preferences
Salary ranges
Troubleshooting
If you encounter any issues:

Package Installation Errors:
BASH

pip install --upgrade pip
pip install -r requirements.txt
SpaCy Model Error:
BASH

python -m spacy download en_core_web_sm --force
Memory Issues:
Restart the kernel
Run cells sequentially
Notes for Evaluation
The system demonstrates practical application of NLP and ML concepts
Implements industry-standard matching algorithms
Features both technical sophistication and user-friendly output
Includes comprehensive error handling and data validation
Provides clear visualization of results
Technical Implementation
Key components:

Word embeddings for semantic understanding
Fuzzy string matching for skill comparison
Weighted scoring system for multiple criteria
Interactive data visualization
Comprehensive data preprocessing
Performance Metrics
The system evaluates matches based on:

Skill match accuracy (40% weight)
Education compatibility (15% weight)
Experience alignment (15% weight)
Location match (15% weight)
Salary fit (15% weight)
Requirements

pandas==1.5.3
numpy==1.23.5
scikit-learn==1.2.2
gensim==4.3.1
spacy==3.5.3
plotly==5.14.1
thefuzz==0.19.0
Time Complexity
Data Processing: O(n) where n is the number of profiles
Matching Algorithm: O(m×n) where m is number of jobs and n is number of candidates
Visualization Generation: O(k) where k is the number of matches
