# PDF Data Extraction
This UiPath project is designed to automate the extraction of data from PDF files and save the extracted information into text files
Use Cases:
1.Invoice Processing: Automates the extraction of invoice data from PDFs for further processing or analysis.

2.PDF Digitization: Converts scanned documents into editable text files.

# Key Features:

User Interaction:
Provides an interactive dialog for users to choose between different extraction options (extracting invoices or general PDF data).

Dual Extraction Methods:
Text-Based PDFs: Extracts text directly from PDFs using the Read PDF Text activity.

Scanned PDFs (OCR): Uses Optical Character Recognition (OCR) via the Read PDF With OCR activity to extract text from scanned or image-based PDFs.

Dynamic File Handling:

The workflow dynamically identifies and processes all PDF files in a specified folder.

It creates corresponding .txt files for each PDF, storing the extracted text in the same directory.

Retry Mechanism:

Implements a retry mechanism to handle transient errors during the extraction process.

Users can configure the number of retries and the interval between retries.

Error Handling:

Robust error handling using TryCatch blocks to log exceptions and ensure the workflow continues or fails gracefully.

Logs detailed error messages, including the source and description of exceptions.

Logging:

Extensive logging is implemented to track the progress of the workflow, including the start and end of processes, file existence checks, and success/failure of data extraction.
