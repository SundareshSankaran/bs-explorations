# BS Explorations: Web Scraping Tutorials with Beautiful Soup
#### The good kind of bs. For Beautiful Soup
Welcome to **BS Explorations**, a tutorial series designed to guide you through the fundamentals and advanced techniques of web scraping using Python, specifically with the Beautiful Soup package. This repository serves as both a hands-on learning resource and the foundation for [this article](https://medium.com/@sundaresh.Sankaran/rediscovering-bs-bs4-i-mean-eede765c9d12) on the basics of BS4.

## Overview

Web scraping is frequently undertaken by data scientists, analysts, and developers who need to extract valuable information from the web. With the increasing use of Large Language Models (LLMs), information retrieval techniques used in scraping are also useful in developing semantic segmentation approaches that can enhance or substitute standard chunking approaches.

This tutorial series uses BeautifulSoup (BS4) as the core library, complemented by tools like `requests` for HTTP interactions, `pandas` for data manipulation, and `Jupyter Lab` for interactive learning.

The tutorials progress from basic web requests to creating structured datasets, demonstrating real-world scraping scenarios while emphasizing ethical practices, error handling, and data integrity.

## Prerequisites

Before diving in, ensure you have:

- **Python 3.11+** installed on your system
- Basic understanding of Python programming
- Familiarity with HTML structure (helpful but not required)
- A Python editor (Visual Studio Code recommended) with Jupyter Notebook support

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/bs-explorations.git
   cd bs-explorations
   ```

2. **Set up the environment:**
   Run the provided build script to create a virtual environment and install dependencies:
   ```bash
   cd build
   chmod +x build.sh
   ./build.sh
   ```
   This will:
   - Create a Python virtual environment
   - Install all required packages from `requirements.txt`
   - Set up a Jupyter kernel
   - Launch Jupyter Lab

   If you wish to run quick tests or delete the virtual environment folders, refer to the last two commented lines in [`build.sh`](/build/build.sh)


3. **Alternative manual setup:**
   If you prefer manual installation:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r build/requirements.txt
   python -m ipykernel install --user --name=bs-explorations
   ```

## Tutorial Series

This series consists of 5 progressive tutorials, each building upon the previous one. Open the notebooks in the [`notebooks/`](/notebooks/) directory and follow along step by step.

### Tutorial 1: Making a Request
**File:** [`Tutorial_1_Making_A_Request.ipynb`](/notebooks/Tutorial_1_Making_A_Request.ipynb)

Learn the basics of making HTTP requests using the `requests` library. We'll cover:
- Setting up proper headers for web scraping
- Respecting website terms of service
- Handling HTTP responses
- Basic error handling


### Tutorial 2: Converting to Soup
**File:** [`Tutorial_2_Converting_to_Soup.ipynb`](/notebooks/Tutorial_2_Converting_to_Soup.ipynb)

Dive into HTML parsing with BeautifulSoup:
- Converting raw HTML to a BeautifulSoup object
- Basic navigation through HTML elements
- Extracting text and attributes from tags

### Tutorial 3: Create Basic Table
**File:** [`Tutorial_3_Create_Basic_Table.ipynb`](/notebooks/Tutorial_3_Create_Basic_Table.ipynb)

Start structuring scraped data:
- Extracting tabular data from web pages
- Basic data cleaning and formatting
- Creating pandas DataFrames to hold output
- Simple data export options

### Tutorial 4: Create Section-wise Long Table
**File:** [`Tutorial_4_Create_section_wise_long_table.ipynb`](/notebooks/Tutorial_4_Create_section_wise_long_table.ipynb)

Handle complex, multi-section data:
- Scraping data from multiple sections
- Using HTML attributes to your advantage
- Advanced BeautifulSoup selectors

### Tutorial 5: Create Granular Table
**File:** [`Tutorial_5_Create_granular_table.ipynb`](/notebooks/Tutorial_5_Create_granular_table.ipynb)

- Fine-tuned element selection
- Handling nested data structures
- Data validation and quality checks


## Running the Tutorials

1. After installation, Jupyter Lab should open automatically
2. Navigate to the `notebooks/` folder
3. Open tutorials in order (Tutorial 1 → Tutorial 5)
4. Execute cells sequentially using Shift+Enter
5. Experiment with the code and modify examples

**Pro Tip:** Use `%store` magic commands to pass variables between notebooks as demonstrated in the tutorials.

## Key Libraries Used

- **BeautifulSoup (bs4):** HTML/XML parsing
- **requests:** HTTP library for Python
- **pandas:** Data manipulation and analysis
- **jupyter:** Interactive computing
- **pyarrow/fastparquet:** Efficient data storage
- **duckdb:** Analytical database
- **scikit-learn:** Machine learning utilities

In case you don't see any of these packages used directly in the notebooks, expect examples making use of them in future.

## Best Practices Covered

Some foundational practices demonstrated in these tutorials include:
- Ethical scraping (respect robots.txt, rate limiting)
- Error handling and retry logic
- Data validation and cleaning
- Efficient data structures
- Performance optimization techniques

## Project Structure

```
bs-explorations/
├── build/
│   ├── build.sh              # Environment setup script
│   ├── requirements.txt      # Python dependencies
│   └── buildproj/            # Virtual environment (created by build.sh)
├── notebooks/
│   ├── Tutorial_1_Making_A_Request.ipynb
│   ├── Tutorial_2_Converting_to_Soup.ipynb
│   ├── Tutorial_3_Create_Basic_Table.ipynb
│   ├── Tutorial_4_Create_section_wise_long_table-Copy1.ipynb
│   └── Tutorial_5_Create_granular_table.ipynb
└── README.md
```

## Contributing

Contributions are welcome! If you find issues or want to enhance the tutorials:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

Please ensure your code follows the existing style and includes appropriate documentation.

## License

This project is licensed under the Apache 2.0 License - see the LICENSE file for details.

## Disclaimer

This tutorial is for educational purposes only. It makes use of Wikipedia to serve as an illustration but does not focus on a specific Wikipedia page or article.  Wikipedia pagge structures are subject to changge.  Always respect website terms of service, robots.txt files, and applicable laws when scraping websites. The authors are not responsible for misuse of the techniques presented.

<!--
## Upcoming Article

This repository forms the basis for an in-depth article exploring advanced web scraping techniques, including:
- Handling JavaScript-heavy sites
- Dealing with anti-scraping measures
- Large-scale scraping architectures
- Legal and ethical considerations

Stay tuned for the full article publication!
-->
---
Contact:
- [Sundaresh Sankaran](sundaresh.sankaran@gmail.com)


Happy scraping! 🕷️📊