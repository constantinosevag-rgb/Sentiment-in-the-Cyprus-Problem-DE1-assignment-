# Cloud Data Analysis: Sentiment in the Cyprus Problem

**Course:** Data Engineering 1  
**Assignment:** 3  
**Students:** Konstantinos Evagorou & Zariza Chowdhury  

---

## 1. Project Overview
This project leverages **AWS Cloud Services** to analyze the sentiment of media coverage regarding the 2025 UN negotiation deadlock on the Cyprus Problem. 

We compare narratives from two conflicting sides:
* **Greek Cypriot Media** (*Politis News*): Focus on Federal framework.
* **Turkish Cypriot Media** (*Kibris Postasi*): Focus on Two-State solution.

The solution implements a serverless pipeline using **AWS S3** (Storage), **AWS Translate** (Preprocessing), and **AWS Comprehend** (Sentiment Analysis).

## 2. Repository Structure
The repository is organized as follows:

```text
.
├── Cloud Data Analysis(Code).ipynb   # Main Jupyter Notebook with analysis pipeline & code
├── PDF report.pdf                    # Full report with methodology, deep analysis & cost breakdown
├── requirements.txt                  # List of Python dependencies
└── README.md                         # Project documentation

```
## 3. Key Findings (Summary)
Detailed results are available in the PDF report.pdf. In summary:

Greek Cypriot Coverage: Classified as NEUTRAL (~98% confidence). The language was objective and legalistic, focusing on UN resolutions.

Turkish Cypriot Coverage: Classified as MIXED (~95% confidence). The text contained high emotional variance, blending positive terms (Sovereignty) with negative context (Isolation).

## 4. How to Run
Prerequisites

Python 3.x installed.

An active AWS Account with Access Key and Secret Key.

AWS CLI configured (optional but recommended).

git clone <repository_url>
pip install -r requirements.txt
aws configure
jupyter notebook "Cloud Data Analysis(Code).ipynb"

For a detailed breakdown of costs and methodology, please refer to the attached PDF report.

## 5. References
The text analyzed in this project was derived from the following real-world news reports regarding the 2025 UN negotiation deadlock:

Greek Cypriot Source: Politis News (Nov 2025). "All Eyes on Two Leaders to Lead the Way to Talks".

Turkish Cypriot Source: TRNC Public Information Office (July 2025). "President Tatar: We maintain the two-state policy".
