# Playwright Python Work

This project demonstrates a clean and scalable **UI test automation framework** using:

* **Python**
* **Playwright**
* **Pytest**
* **Page Object Model (POM)**
* **Parametrized test data**

The framework performs automated searches on **DuckDuckGo**, validates results, and serves as a template for modern browser automation.

## 📁 Project Structure

├── pages/\
│   ├── search.py                  # DuckDuckGoSearchPage object\
│   ├── result.py                  # DuckDuckGoResultPage object\
│\
├── tests/\
│   └── test_search.py             # Parametrized DuckDuckGo search tests\
│\
├── conftest.py                    # Shared fixtures (Playwright page, POM)\
├── requirements.txt\
└── README.md

## 🧪 Test Scenario

Each test performs the following steps:

1. Open DuckDuckGo
2. Enter a search phrase
3. Verify:

* The phrase appears in the search bar
* The search results contain related links
* The page title includes the search phrase

Searches run against a set of animals using pytest.mark.parametrize.

## 🛠 Installation
**1. Create virtual environment**

python -m venv .venv\
source .venv/bin/activate   # macOS / Linux\
.venv\Scripts\activate      # Windows

**2. Install dependencies**\
`pip install -r requirements.txt`

**3. Install Playwright browsers**\
`playwright install`

## ▶️ Running the Tests
**Run all tests**\
`pytest`

**Run with Playwright’s HTML report**\
`pytest --headed`

**Run a single test**\
`pytest tests/test_search.py::test_basic_duckduckgo_search`

**Run with screenshots and tracing**\
`pytest --tracing on --screenshot on`

## ⚙️ Technologies Used
| Technology     | Purpose                        |
| -------------- | ------------------------------ |
| **Playwright** | Browser automation framework   |
| **Pytest**     | Test runner, fixtures, marking |
| **Python**     | Core programming language      |
| **POM**        | Scalable test design pattern   |

   
## 🤝 Contributing
Pull requests and suggestions are welcome!\
Feel free to open issues for improvements, bugs, or feature requests.


