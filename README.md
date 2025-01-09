# Project Title: Social Media Scraper for Reddit and Red (With Image)

## Overview
This project involves building a robust social media scraper to collect and analyze data from platforms like Reddit and Red using Google Cloud Platform (GCP). The scraped data is processed and stored for further analysis, with visual insights generated using Looker Studio. The scraper successfully collects posts, comments, and images from both platforms.

## Key Features
- Data Extraction: Utilized APIs and web scraping techniques to gather posts, comments, and images from Reddit and Red.
- Data Transformation: Processed raw data to clean and structure it using Python scripts in Jupyter Notebook.
- Data Storage: Leveraged Google Cloud Storage and BigQuery for scalable storage and efficient querying. Includes support for an empty file named "reddit" to store Reddit-related content during operations.
- Data Visualization: Created dynamic dashboards in Looker Studio to showcase insights such as trending topics, engagement metrics, and user sentiment.

## Tools and Technologies
- **Google Cloud Platform**:
  - **Google Cloud Storage**: To store raw and processed data.
  - **BigQuery**: For structured storage and SQL-based querying.
  - **Looker Studio**: For creating interactive dashboards.
- **Python**:
  - Libraries: BeautifulSoup, PRAW (Python Reddit API Wrapper), Pandas.
- **Jupyter Notebook**: For developing and testing ETL pipelines.

## Workflow
1. **Extract**:
   - Gathered posts, comments, and images from Reddit using PRAW.
   - Scraped posts, metadata, and images from Red using BeautifulSoup.

2. **Transform**:
   - Cleaned and formatted the scraped data using Python.
   - Standardized data fields like timestamps, text length, and user engagement metrics.

3. **Load**:
   - Uploaded structured data to Google Cloud Storage.
   - Imported data into BigQuery for further analysis.

4. **Analyze and Visualize**:
   - Queried BigQuery to extract insights such as the most active subreddits, trending topics, and user sentiment analysis.
   - Designed a dashboard in Looker Studio to present key findings interactively.

## Results
The final output includes:
- A clean dataset of posts, comments, and images from Reddit and Red.
- A Looker Studio dashboard showcasing:
  - Top-performing posts and subreddits.
  - Engagement metrics (likes, comments, shares).
  - Sentiment analysis results.

### Sample Data Output:
| Platform | Post Title              | Comments | Likes | Sentiment |
|----------|-------------------------|----------|-------|-----------|
| Reddit   | "How to learn Python"  | 150      | 320   | Positive  |
| Red      | "Best travel tips"     | 85       | 210   | Neutral   |

## Repository Structure
- **QL Post Scraper.ipynb**: Jupyter Notebook containing the scraper code and data transformation logic.
- **Sample Output**: Example of the structured dataset.
- **Dashboard Screenshot**: Visual representation of the Looker Studio dashboard.
- **Reddit Empty File**: An empty file named "reddit" to store Reddit-related content.

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/jiao-xx/your-repo-name.git
   ```
2. Install required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Create an empty file named `reddit` in the repository root:
   ```bash
   touch reddit
   ```
4. Run the `QL Post Scraper.ipynb` notebook to extract and process data.

## Future Enhancements
- Incorporate more social media platforms like Twitter and Instagram if possible.
- Implement real-time data scraping and dashboard updates.
- Add advanced analytics, such as network analysis and topic modeling.
