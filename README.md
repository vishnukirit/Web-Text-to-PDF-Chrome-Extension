# Web Text to PDF Chrome Extension in Node.js
This project demonstrates how to create a Chrome extension that converts webpage text into a downloadable PDF. It integrates with a Node.js backend to handle PDF generation using the PDFKit library. Users can convert the entire webpage’s text or selected text by right-clicking or making a selection.

## Key Features:
- Chrome Extension: Converts selected or entire webpage text into a PDF via right-click.
- Node.js Backend: A REST API powered by Express.js generates PDFs from the text data.
- PDF Download: Automatically downloads the generated PDF.
- CORS Support: Backend handles cross-origin requests for extension compatibility.

## Setup Instructions:

### Part 1: Chrome Extension
Set Up the Project Directory: Organize the extension files (manifest.json, background.js, popup.html) in a folder (e.g., chrome-extension).
- Manifest File: Create manifest.json to define metadata and permissions for the extension.
- Background Script: Implement logic in background.js to handle the context menu and trigger PDF generation.
- Popup HTML: Design a simple interface in popup.html for displaying extension details.
- 
### Part 2: Node.js Backend
- Node.js Setup: Set up an Express.js server with PDFKit and CORS for API requests and PDF generation.
- PDF Generation: Create an endpoint (/api/generate-pdf) that generates PDFs based on received text.
- File Handling: Store PDFs on the server and provide download links.
- PDF Listing: Implement routes to list and download generated PDFs.

## Technologies:
- Frontend: Chrome Extension (HTML, JavaScript)
- Backend: Node.js, Express, PDFKit
- Libraries: CORS, Body-Parser

## Instructions to Run:
Backend Setup:
Install Dependencies:
- Ensure Node.js and npm are installed.
- Run npm install to install dependencies from package.json.
Start Server:
-Run node server.js to start the backend server on http://localhost:5000/.

### Chrome Extension Setup:
- Go to chrome://extensions/, enable Developer Mode, and click Load unpacked.
- Select the chrome-extension/ folder to load the extension.

## Contributions:
Feel free to fork, open issues, and submit pull requests. Contributions are welcome!

## License:
This project is licensed under the MIT License.
