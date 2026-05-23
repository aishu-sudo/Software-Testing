# CSE430 Lab & Selenium Assignment Repository
This repository contains course work artifacts for CSE430, including:
- A Selenium automation assignment (Jupyter notebook + generated dataset/report files)
- A small `pytest` practice project (`Calculator` class with tests)
- Supporting media/files for assignment submissions

## Repository Structure
- `2022-3-60-216_SeleniumAssignment.ipynb.ipynb` — Main Selenium assignment notebook
- `books_data.csv` — Scraped output dataset (books from `books.toscrape.com`)
- `2022-3-60-216_SeleniumReport.pdf` / `.docx` — Assignment report documents
- `pytest/calculator.py` — Basic calculator implementation
- `pytest/test.py` — Unit tests for calculator methods
- `pytest/test_fixture.py` — Fixture-based pytest examples
- `assignment_2/` — Assignment-related video artifacts
- `lab_exam/` — Duplicate/packaged notebook copy

## Features
### Selenium Assignment (Notebook)
The notebook demonstrates:
- Browser launch and navigation checks
- Element location using multiple selectors (`CLASS_NAME`, `CSS_SELECTOR`, `XPATH`, `TAG_NAME`)
- Multi-page scraping from `https://books.toscrape.com`
- Data extraction (`title`, `price`, `rating`, `availability`)
- CSV export (`books_data.csv`)
- Basic end-to-end validation on selected book pages

### Pytest Practice Project
Implements and tests:
- `add(a, b)`
- `subtract(a, b)`
- `multiply(a, b)`
- `divide(a, b)` (raises `ValueError` on divide-by-zero; uses integer division)

## Prerequisites
- Python 3.10+ (project files indicate Python 3.10.11 was used in the notebook)
- Google Chrome installed
- Python packages:
  - `selenium`
  - `pytest`
  - `jupyter` (for running the notebook)

Install dependencies:
```bash path=null start=null
pip install selenium pytest jupyter
```

## How to Run
### 1) Run Pytest Suite
From the repository root:
```bash path=null start=null
pytest pytest
```

### 2) Run Selenium Notebook
Start Jupyter:
```bash path=null start=null
jupyter notebook
```
Then open:
- `2022-3-60-216_SeleniumAssignment.ipynb.ipynb`

Run cells sequentially to execute scraping and test steps.


