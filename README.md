
# **PubMed Fetcher**  

## **📌 Overview**  
**PubMed Fetcher** is a command-line tool that fetches research papers from **PubMed** based on user queries. It filters out academic institutions and extracts non-academic affiliations. The fetched data can be displayed in the terminal or saved as a CSV file.  

## **📂 Project Structure**  
cli.py → Defines the command-line interface using Typer.
fetch.py → Handles PubMed API requests, extracts paper details (authors, affiliations, emails), and filters out academic institutions.
utils.py → Contains helper functions such as email extraction, filtering affiliations, and handling text parsing.
tests/ → Includes unit tests to validate API calls and output correctness.
pyproject.toml → Manages dependencies and project settings using Poetry.

## **🚀 Features**  
✅ Fetches research papers from **PubMed API**  
✅ Extracts **authors, affiliations, and emails**  
✅ Filters out **academic institutions**  
✅ Saves results as a **CSV file**  
✅ Provides a **command-line interface** using **Typer**  

---

## **🛠 Installation**  

### **1️⃣ Install Poetry**  
If you haven't installed **Poetry**, install it first:  
```sh
pip install poetry
```

### **2️⃣ Clone the Repository**  

git clone https://github.com/pravallika-0201/pubmed_fetcher.git
cd pubmed_fetcher


### **3️⃣ Install Dependencies**  

poetry install


## **📌 Usage**  

### **Run the CLI**

poetry run get-papers-list "cancer research" -d -f papers.csv


✅ **Arguments:**  
- **`query`** → Search query for PubMed papers (e.g., `"cancer research"`)  
- **`-d / --debug`** → Enable debug logs  
- **`-f / --file <filename>`** → Save output as CSV  

### **Example Commands**

poetry run get-papers-list "COVID-19 vaccine" --debug
poetry run get-papers-list "machine learning in healthcare" --file results.csv


---
Tools & Libraries Used

Tool/Library | Purpose | Link |

 Poetry | Dependency management | [Poetry](https://python-poetry.org/) |
 Requests| API requests to PubMed | [Requests](https://docs.python-requests.org/) |
 Typer| CLI framework | [Typer](https://typer.tiangolo.com/) |
 Pandas | Data manipulation & CSV saving | [Pandas](https://pandas.pydata.org/) |


