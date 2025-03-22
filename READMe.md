# Jupyter Notebook Code Extractor

## Description
This script extracts code cells from a Jupyter Notebook (.ipynb) file and combines them into a single Python script for analysis. It reads the notebook's JSON structure, filters out the code cells, and merges them into a readable format.

## Features
- Reads a Jupyter Notebook file (.ipynb)
- Extracts all code cells
- Combines extracted code into a single script
- Displays a preview of the first given value of characters from the extracted code

## Prerequisites
Before running this script, ensure that you have:
- Python installed
- JSON module (comes pre-installed with Python)

## Installation
No external installation is required since the script only uses Python’s built-in `json` module.

## How to Run
1. Save your Jupyter Notebook file (.ipynb) in a known location.
2. Update the `file_path` variable in the script to the correct path of your notebook file.
3. Run the script using Python:
   ```sh
   python code_extractor.py
   ```
4. The extracted code will be stored in `code_combined` and a preview (first given range characters) will be displayed.

## User Manual
### Input
- A valid Jupyter Notebook (.ipynb) file containing code cells.

### Output
- Extracted code displayed on the console.
- The variable `code_combined` contains the entire extracted script.

### Customization
- Modify the `code_combined[:20000]` part to adjust the preview size.
- Save the extracted code to a `.py` file if needed:
   ```python
   with open("extracted_code.py", "w") as output_file:
       output_file.write(code_combined)
   ``` 



