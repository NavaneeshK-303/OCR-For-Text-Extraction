# OCR-For-Text-Extraction

A Streamlit-based OCR app that extracts key details from GATE scorecard images using Tesseract and OpenCV. It preprocesses images, extracts text, and classifies fields like Name, Registration Number, Gender, and GATE Score. Results are shown in a table and can be exported as CSV.

## Features
- Upload GATE scorecard images (.png, .jpg, .jpeg)
- Preprocessing of images using OpenCV
- Text extraction with Tesseract OCR
- Extraction of structured data: Name, Reg. No., Gender, Score
- Download results as CSV

## Tech Stack
- Python 3
- Streamlit
- OpenCV
- Tesseract OCR

## Installation & Usage
1. Clone the repository  
   `git clone https://github.com/NavaneeshK-303/OCR-For-Text-Extraction.git && cd OCR-For-Text-Extraction`
2. Create and activate a virtual environment (optional but recommended)  
   On Windows: `python -m venv venv && venv\Scripts\activate`  
   On Linux / macOS: `python3 -m venv venv && source venv/bin/activate`
3. Install dependencies  
   `pip install -r requirements.txt`
4. Run the app  
   - If your folder path has no spaces: `streamlit run main.py`  
   - If your folder path contains spaces (e.g. `C:\Users\My Folder\...`):  
     `streamlit run ".\main.py"`  
     or  
     `streamlit run "C:\Users\My Folder\Downloads\OCR-For-Text-Extraction\main.py"`
5. Open the app in your browser at `http://localhost:8501`

## Project Structure
OCR-For-Text-Extraction/
├── main.py # Core Streamlit app with OCR logic
├── frontend.py # Additional UI/frontend code
├── requirements.txt # All required Python packages
├── README.md # Project documentation
├── venv/ # Virtual environment (if used)
└── .idea/ # IDE files (optional)

## Troubleshooting
- If you see "File does not exist: main.py", check:
  1. You are in the correct directory (where `main.py` is).
  2. If there is a space in any folder name in the path, wrap the path or filename in quotes as shown above.
  3. Use `streamlit run .\main.py` (Windows) or `streamlit run ./main.py` (Linux/Mac) if relative paths are safer.

