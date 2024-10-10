# App Directory

This directory contains the core code for the Cold Email Generator, including the logic for scraping, portfolio matching, and email generation, as well as the Streamlit app.

## File Overview

- **main.py**: The entry point of the Streamlit app. This script defines the user interface where users input the job posting URL, and it calls functions from other modules to scrape the job description, query the portfolio, and generate the email.
- **chains.py**: Contains the logic for creating and managing prompt chains, using **Llama 3.1** to extract job details and generate cold emails.
- **portfolio.py**: Handles the **ChromaDB** setup and queries, matching job skills to the company's portfolio projects.
- **utils.py**: Contains utility functions for cleaning HTML tags and formatting text extracted from job descriptions.

## How to Run

To run the Cold Email Generator app, execute the following command from the project root directory:

```bash
streamlit run app/main.py
