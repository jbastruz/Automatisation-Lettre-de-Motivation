This document is a Jupyter notebook that aims to prove the feasibility of setting up an automated tool for generating cover letters based on a Linkedin job offer link and the user's CV description.

## Loading Packages

The following packages are used in this document:

* `BeautifulSoup` for web scraping
* `requests` for HTTP requests
* `json` for JSON data manipulation
* `os` for accessing environment variables
* `MistralClient` and `ChatMessage` from `mistralai` for text generation
* `load_dotenv` from `dotenv` to load environment variables

## Extracting Data from Linkedin

The document uses `BeautifulSoup` and `requests` to extract the links of data analyst job offers in Geneva from Linkedin.

## List of Job Offers

A list of job offer links is created and the first link is displayed.

## Retrieving Job Description

For each link in the list, the document uses `BeautifulSoup` and `requests` to extract the job description. The descriptions are stored in a list.

## List of Required Skills

The document then uses `MistralClient` and `ChatMessage` to generate a list of required skills for each job offer, based on the job description.

## Generating the Cover Letter

Finally, the document uses `MistralClient` and `ChatMessage` to generate a cover letter using the required skills and the user's CV information. The generated cover letter is displayed.
