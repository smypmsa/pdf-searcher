# PDF OCR Searcher

Search for keywords in PDF files using OCR and generate Excel reports.

## Privacy & Local Processing

All data processing happens locally on your machine. No files or data are sent to external servers. The tool uses:
- [EasyOCR](https://github.com/JaidedAI/EasyOCR) for offline OCR processing
- [PyMuPDF](https://github.com/pymupdf/PyMuPDF) for local PDF text extraction
- [OpenPyXL](https://openpyxl.readthedocs.io/) for local Excel file generation

Your sensitive documents remain completely private and secure.

## Setup

1. Install [uv](https://docs.astral.sh/uv/getting-started/installation/)
2. Install dependencies:
   ```bash
   uv sync
   ```

## Usage

1. Copy `keywords.txt.example` to `keywords.txt` and add your keywords (one per line)
2. Place PDF files in the `inputs/` folder
3. Run the script:
   ```bash
   uv run main.py
   ```
4. Check the `outputs/` folder for the Excel report

## Output

The tool generates `keyword_search_results.xlsx` showing which keywords were found in each PDF file.