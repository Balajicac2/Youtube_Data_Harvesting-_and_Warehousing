# YouTube Data Harvesting and Warehousing

## Overview

This project is a comprehensive application designed for harvesting and warehousing data from YouTube. Using the YouTube Data API, it collects extensive information about YouTube channels, their playlists, videos, and comments. The data is initially stored in MongoDB and then migrated to PostgreSQL for advanced querying and analysis. The user interface, built with Streamlit, allows users to interactively collect, store, migrate, and query data.

## Features

- **API Integration**: Connects to the YouTube Data API to fetch detailed information about channels, videos, playlists, and comments.
- **Data Storage**: Utilizes MongoDB for storing raw data and PostgreSQL for structured data management.
- **Data Manipulation**: Employs Pandas for data manipulation and transformation.
- **Interactive UI**: Streamlit-based user interface for easy interaction with the data.
- **Predefined Queries**: Allows users to run predefined SQL queries to gain insights from the data.

## Technologies Used

- **Python**: Core programming language.
- **Google API Client**: For interacting with the YouTube Data API.
- **PyMongo**: For MongoDB interactions.
- **Psycopg2**: For PostgreSQL interactions.
- **Pandas**: For data manipulation and transformation.
- **Streamlit**: For building the interactive web application.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/https://github.com/Balajicac2/Youtube_Data_Harvesting-_and_Warehousing.git
   cd youtube-data-harvesting
   ```

2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up MongoDB and PostgreSQL:

   - Ensure MongoDB and PostgreSQL are installed and running.
   - Update the MongoDB and PostgreSQL connection strings in the code as needed.

## Usage

1. Run the Streamlit application:

   ```bash
   streamlit run app.py
   ```

2. Open the application in your web browser.

3. Use the sidebar to enter a YouTube channel ID and collect data.

4. Migrate data to SQL for advanced querying.

5. View data and run predefined SQL queries from the interactive UI.

## Code Explanation

- **API Connection**: Establishes a connection to the YouTube Data API.
- **Data Collection**:
  - `get_channel_info(channel_id)`: Fetches channel information.
  - `get_videos_ids(channel_id)`: Fetches video IDs from the channel.
  - `get_video_info(video_ids)`: Fetches detailed video information.
  - `get_comment_info(video_ids)`: Fetches comments for videos.
  - `get_playlist_details(channel_id)`: Fetches playlist details.
- **Data Storage**:
  - Stores collected data in MongoDB.
  - Functions to create and populate PostgreSQL tables with the collected data.
- **Streamlit Interface**:
  - User inputs channel ID to collect data.
  - Options to view data and migrate it to PostgreSQL.
  - Predefined queries for analysis.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Thanks to the developers of the libraries and tools used in this project.
- Special thanks to the Streamlit community for their support and resources.
```
