# ReadFlowBlocks

**ReadFlowBlocks** is an open-source web application for reading text files (.txt, .pdf, .docx, .html, .epub, .rtf) with customizable reading speed, word count, and navigation. It is designed to make reading engaging and accessible.

> **⚠️ Important**: This application processes files locally in your browser and does not upload data to any server. However, it uses external libraries that may transmit metadata (e.g., IP addresses) to third-party CDNs. See [Privacy Policy](#privacy-policy) for details.

## Features
- **Local File Processing**: Files are processed entirely in your browser, ensuring no data is sent to servers.
- **Customizable Reading**: Adjust reading speed (words per second), text size, and number of words displayed.
- **Navigation**: Supports chapter navigation for EPUB files and page navigation for PDFs.
- **Supported Formats**: .txt, .pdf, .docx, .html, .epub, .rtf.

## Installation
1. Clone the repository: `git clone https://github.com/MaksimDidukh/ReadFlowBlocks.git`
2. Start a local server (required due to browser CORS restrictions):
   - Python: `python -m http.server 8000`
   - VS Code Live Server
3. Open `http://localhost:8000` in your browser.
   > **Note**: Do not open `index.html` directly via `file://`, as it will not work due to CORS restrictions.

## Usage
1. Upload a supported file using the file input.
2. Adjust reading speed, text size, and word count using the sliders.
3. Use the navigation controls to jump to specific chapters (EPUB) or pages (PDF).

## For Developers and Users
### ⚠️ Important Notices
- **Privacy**: Files are processed locally, but the application uses external libraries loaded via CDNs (`unpkg.com`, `cdnjs.cloudflare.com`). These may transmit metadata to third parties. To avoid this, host the libraries locally (see [Contributing](#contributing)).
- **Copyright**: You are responsible for ensuring you have the right to use the files you upload. ReadFlowBlocks does not track or store uploaded content, and we are not liable for any copyright violations.
- **Limitations**: The application only supports the listed formats and requires a local server for operation.

## Privacy Policy
ReadFlowBlocks processes all files locally in your browser. No data is uploaded to servers. However:
- The application loads libraries (`pdf.js`, `mammoth`, `epubjs`, `rtf.js`) from external CDNs, which may collect metadata (e.g., IP addresses).
- Reading progress is stored in your browser's `localStorage` and can be cleared manually.
For more details, see [PRIVACY.md](PRIVACY.md).

## Terms of Use
By using ReadFlowBlocks, you agree to:
- Upload only files you have the legal right to use.
- Accept that the application is provided "as is," without warranties.
- Understand that we are not responsible for any data loss or misuse of the application.
For full terms, see [TERMS.md](TERMS.md).

## Third-Party Libraries
ReadFlowBlocks uses the following libraries:
- `pdf.js` (Apache 2.0)
- `mammoth.js` (BSD-2-Clause)
- `epubjs` (BSD-2-Clause)
- `rtf.js` (MIT)
All libraries are loaded via CDNs in the default setup. To host them locally, download the files from their respective repositories and update the script paths in `index.html`.

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch: `git checkout -b my-feature`.
3. Commit your changes: `git commit -m 'Add feature'`.
4. Push to the branch: `git push origin my-feature`.
5. Open a Pull Request.
To host libraries locally, download them from their official repositories and update `index.html` to use local paths (e.g., `/lib/pdf.min.js`).

## License
This project is licensed under the [MIT License](LICENSE). See [LICENSE](LICENSE) for details.

## Contact
- **Author**: Maksym Didukh
- **Email**: didukh.maxim@gmail.com
- **GitHub**: [MaksimDidukh](https://github.com/MaksimDidukh)
- **Issues**: Report bugs or ask questions via [GitHub Issues](https://github.com/MaksimDidukh/ReadFlowBlocks/issues)

## Acknowledgements
This project was created to make reading more accessible and enjoyable. I hope it brings you a satisfying and selfless experience with your favorite books!

---
Created with ❤️ by Maksym Didukh
