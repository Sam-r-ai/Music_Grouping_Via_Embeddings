# Music_Grouping_Via_Embeddings

This project aims to group songs by embeddings, enabling insights and analysis based on their characteristics. Due to the deprecation of certain Spotipy features, this process requires manual dataset creation or the use of pre-existing spreadsheets.

### Prerequisites

Ensure you have Python installed (version 3.7 or higher is recommended).

### Installation

Install the necessary Python packages by running the following command:

pip install pandas scikit-learn matplotlib sentence-transformers spotipy python-dotenv

### Dataset Preparation

Since Spotipy's API for fetching data directly has been deprecated (partially due to changes in policies around AI data usage), you need to prepare your dataset manually. Here are the steps:

### Create Your Dataset:

Use a spreadsheet program (e.g., Microsoft Excel, Google Sheets) to create a dataset.

Include columns like Track Name, Artist, Album, and any other features relevant to your analysis.

Save the file as a .csv file.

Find Pre-existing Data:

Search for publicly available song datasets that suit your needs.

### Project Workflow

Clone this repository:

git clone <repository_url>
cd Music_Grouping_Via_Embeddings

Place your .csv dataset in the project directory.

Configure environment variables for Spotipy:

Create a .env file in the project root.

Add the following keys with your Spotipy credentials:

SPOTIPY_CLIENT_ID=your_client_id
SPOTIPY_CLIENT_SECRET=your_client_secret

Note: Spotipy functionality for fetching new data might be limited due to API restrictions.

Open and run the 2021-2022embeddedsongs.ipynb Jupyter notebook to execute the project workflow. Ensure your dataset path is correctly set in the notebook.

### Notes

The Spotipy API may not work as intended for fetching new song data due to their policy against AI training. Manual preparation of datasets is recommended.

Make sure the dataset format aligns with the project's requirements (e.g., column names and data types).

### Output

The notebook will output visualizations and groupings of songs based on their embeddings.

For any issues or contributions, feel free to open an issue or create a pull request.

