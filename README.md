# Cryptocurrency Pair Analysis Tool
Cryptocurrency Pair Analysis Tool

Join the [Dexlens DAO](https://dexlens.io/)

![alt text](./images/dexclient.png "dexclient")

## Overview
This Python tool is designed to analyze and manage cryptocurrency pair data from various blockchains. It retrieves trending, top gaining, and newest pairs, offering functionalities like generating files, printing data frames, and adding data to Supabase.

## Features
- **Blockchain Compatibility:** Works with multiple blockchains, defaulting to Solana.
- **Data Analysis:** Retrieves and analyzes data on cryptocurrency pairs.
- **File Generation:** Capable of generating files for further analysis or record-keeping.
- **Data Visualization:** Prints data frames for easy visualization.
- **Supabase Integration:** Option to add data to Supabase for centralized data management.

## Dependencies
- Ensure you have Python installed with necessary libraries for data handling and API requests.

## Usage

### Function: `i_am_the_watcher_free_version`
This is the main function of the tool. It allows users to specify the blockchain, control file generation, data frame printing, and Supabase integration.

#### Parameters:
- `chain` (str): The blockchain to retrieve data from (e.g., "solana", "bsc"). Default is "solana".
- `shouldGenerateFiles` (bool): If `True`, generates files based on the retrieved data. Default is `True`.
- `shouldPrintDataFrames` (bool): If `True`, prints the data frames. Useful for visualizing the data. Default is `False`.
- `shouldAddToSupabase` (bool): If `True`, adds the data to Supabase. Default is `False`.

#### Example Usage:
```python
i_am_the_watcher_free_version("bsc", shouldGenerateFiles=False, shouldPrintDataFrames=True, shouldAddToSupabase=False)
```

## Modules Description
- **consts:** Contains constants like slugged string pairs for various categories.
- **create_data_frame:** Functionality to create data frames from the retrieved data.
- **data_frames_array_print:** Prints array of data frames with labels.
- **generate_files:** Generates files from data frames.
- **get_newest_pairs, get_top_gaining_pairs, get_trending_pairs:** Retrieve newest, top gaining, and trending pairs from a specified blockchain.
- **pairs_loop:** Used for adding data to Supabase.

## Getting Started
1. Clone the repository.
2. Install required dependencies.
3. Run the script with desired parameters. 
