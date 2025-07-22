# PDF OCR Searcher

## Overview

Keyword search solution for PDF document collections using optical character recognition. Delivers comprehensive Excel reporting with complete data privacy assurance.

Open in [Google Colab](https://colab.research.google.com/github/smypmsa/pdf-searcher/blob/main/PDF_searcher.ipynb).

## Security Framework

**Data Processing**: Fully local execution environment with zero external data transmission

**Privacy Architecture**:
- EasyOCR for offline character recognition
- PyMuPDF for local PDF text processing
- OpenPyXL for local Excel generation

All document processing occurs within client infrastructure, ensuring complete confidentiality of sensitive materials.

## Technical Requirements

### Installation Dependencies
1. Install [uv package manager](https://docs.astral.sh/uv/getting-started/installation/)
2. Execute dependency installation:
   ```bash
   uv sync
   ```

## Implementation

### Configuration Setup
1. Create keyword configuration file:
   ```bash
   cp keywords.txt.example keywords.txt
   ```
2. Define search terms (one keyword per line in keywords.txt)
3. Position PDF files in `inputs/` directory

### Execution Process
```bash
uv run main.py
```

### Results Retrieval
Generated reports available in `outputs/` directory

## Output Specifications

**Primary Deliverable**: `keyword_search_results.xlsx`

**Report Contents**:
- Keyword occurrence mapping by document
- Location references within source files
- Search term frequency analysis
- Document coverage metrics

## Operational Benefits

Enables rapid content discovery across large document repositories while maintaining strict data governance and privacy compliance standards.
