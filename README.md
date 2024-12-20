# YouTube Watch History Analysis

This Jupyter notebook analyzes your YouTube watch history to provide insights about your viewing patterns and interests. The notebook processes your watch history data from a JSON file and uses OpenAI's GPT model to generate personalized insights.

## Features

- Filters and processes YouTube watch history from the last year
- Removes duplicate entries and short-form content
- Identifies most frequently rewatched videos
- Generates AI-powered insights about:
  - Your personality and habits
  - Passions and interests
  - Notable patterns in your viewing history
  - Values and focus areas
- Provides personalized recommendations for future learning and content consumption

## Prerequisites

- Python 3.x
- Jupyter Notebook
- Required Python packages:
  - json
  - datetime
  - python-dateutil
  - python-dotenv
  - openai
  - IPython

## Setup

1. Export your YouTube watch history as a JSON file from Google Takeout
2. Place the `watch-history.json` file in the same directory as the notebook
3. Create a `.env` file with your OpenAI API key:
   ```
   OPENAPI_KEY=your_api_key_here
   ```

## Usage

1. Run the notebook cells in sequence
2. The notebook will:
   - Process your watch history
   - Generate statistics about your viewing patterns
   - Use OpenAI to analyze your viewing habits
   - Provide recommendations for future content consumption

## Output

- Total and unique video counts
- List of most frequently rewatched videos
- AI-generated analysis of your viewing patterns
- Personalized recommendations for future learning

## Note

The notebook filters out:
- Videos watched more than a year ago
- Short-form content
- Videos with emoji in titles
- Videos watched within 1 minute of each other
- URLs and hashtag content
