# GitHub Repository Metadata Analysis

##Overview
This project demonstrates my web scraping and data analysis skills.It utilizes the GitHub API to collect and analyze metadata from repositories that match specific search criteria. The goal is to explore patterns such as popular programming languages and gain insights into how repository features correlate with developer interests.cleaned and tokenized the descriptions, and analyzed keyword frequency to identify common trends in repo documentation.

# #Dataset
- Source: GitHub API
- Collected using custom Python scripts with the requests library.
- Key data columns include Name, Repo Url, Description, Language, Stars, and Topics.

## Tools Used
- Python
- Requests
- Pandas
- Matplotlib 
- Nltk
- re
- Collections
- Jupyter Notebook

## Key Steps
- Queried GitHub API with specific search parameters to retrieve up to 100 repositories.
- Parsed and flattened JSON responses into a structured pandas DataFrame.
- Dropped duplicate and null values to clean the dataset.
- Added a cleaned description column using re.sub() for potential future text analysis.
- Analyzed the most commonly used programming languages among the repositories.
- Saved the final dataset to CSV for further exploration or visualization.

## Visualizations
### Popular Programming Languages
A bar chart showcasing the most frequently used languages among the selected repositories. Highlights trends in developer preferences based on GitHub activity.

### Most Common words
the bar chart displays the most used words in the repository's descriptions

>Note: The results reflect a small sample (100 repos) and are influenced by the search criteria and sorting method used in the API call.

## Key Insights
- Python, JavaScript, and Jupyter Notebook appeared most frequently among the sampled repositories.
- GitHub APIs provide rich metadata that can be easily structured for analysis.
- Descriptions offer potential for NLP-driven project categorization, though inconsistencies in text make preprocessing essential.

## Limitations
- GitHub API returns only 100 results per page; this sample was limited for simplicity.
- Repository descriptions are inconsistent and often incomplete, which impacts deeper text analysis.
- Projects vary widely in type and purpose, making uniform classification difficult.

## Future Work
- Implement pagination to collect more data across multiple pages.
- Perform NLP-based clustering on repository descriptions.
- Compare repositories by star counts, topics, and contributor activity.
- Build a dashboard to interactively explore repositories by language, popularity, or description keywords.
