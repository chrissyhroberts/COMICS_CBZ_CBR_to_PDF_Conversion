# Comic to PDF Converter

This tool converts `.cbz` (ZIP-based) and `.cbr` (RAR-based) comic book files into PDF format. It extracts images from comic archives and merges them into a single PDF file. The tool supports batch processing, allowing you to convert all `.cbz` and `.cbr` files in a directory.

## Prerequisites

- Python 3.x
- `unar` (for extracting `.cbr` files on macOS/Linux)
  
  ### Install `unar` (macOS/Linux):
  - On macOS (via Homebrew):
    ```bash
    brew install unar
    ```

  - On Linux (Debian-based distributions):
    ```bash
    sudo apt-get install unar
    ```

## Setting up the Virtual Environment

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/comic-to-pdf-converter.git
   cd comic-to-pdf-converter```

Create a Python virtual environment:
```python3 -m venv venv```

Activate the virtual environment:
On macOS/Linux:
```source venv/bin/activate```
On Windows:
```venv\Scripts\activate```
Install the required Python packages:
```pip install -r requirements.txt```


## Usage

Place your .cbz and .cbr files in a folder (e.g., input/).
Run the tool to convert all .cbz and .cbr files in a specified input directory to PDFs in the output directory:

```python3 convert_comics.py```

Replace the input_directory and output_directory with your desired paths in the script before running.

Example Directory Structure:

Input directory (where your comics are stored):

input/
├── comic1.cbz
├── comic2.cbr
└── comic3.cbz

Output directory (where PDFs will be saved):

output/
├── comic1.pdf
├── comic2.pdf
└── comic3.pdf

### Customization

You can modify the input_directory and output_directory variables in the script to point to your preferred directories.


### Licence 
This project is licensed under the MIT License. See the LICENSE file for details.

