SBOM Viewer README
==================

Overview
--------
SBOM Viewer is a simple, standalone web application designed to display Software Bill of Materials (SBOM) information in a user-friendly manner. It specifically supports CycloneDX SBOM JSON files and extracts key metadata and component details to display in a structured table format.

Features
--------
• **SBOM Metadata Display:** Shows the timestamp and author information (derived from the first tool’s metadata) from the SBOM file.

• **Components Table:** Lists each component with its supplier name, component name, version, unique identifiers (purl and cpe), and dependency relationships.

• **Visual Indicators:** Highlights missing or “N/A” values with a red background for easy identification.

How to Run
----------
1. **Download the Files:**
   - Ensure you have the `index.html` file (which contains all HTML, CSS, and JavaScript code) saved on your computer.

2. **Open in a Browser:**
   - Simply double-click the `index.html` file or right-click and choose your preferred web browser (Chrome, Firefox, Edge, etc.).
   - Alternatively, you can serve it via a local web server (using tools like [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code or a simple Python HTTP server) to avoid any local file restrictions:
     - Using Python 3:
       ```
       python -m http.server
       ```
     - Then navigate to `http://localhost:8000` in your browser.

3. **Using the SBOM Viewer:**
   - Once the page loads, click the **Choose CycloneDX SBOM** button.
   - Select a valid CycloneDX SBOM JSON file from your computer.
   - The SBOM metadata (timestamp and author) will be displayed at the top.
   - The components and their details will appear in the table below.
   - Missing values are highlighted in red to indicate incomplete data.

File Structure
--------------
Since this is a standalone application, the file structure is minimal:
• `index.html` - Contains the HTML, CSS, and JavaScript for the SBOM Viewer.

Dependencies
------------
• No external libraries or frameworks are required.
• The application runs entirely in the browser with standard HTML5, CSS3, and vanilla JavaScript.

Troubleshooting
---------------
• **JSON Parsing Errors:** If you encounter an error parsing your SBOM file, ensure the JSON is properly formatted.
• **File Format:** Only CycloneDX SBOM JSON files are supported. Ensure your file has the correct `.json` extension.
• **Browser Compatibility:** The application should work in any modern web browser with JavaScript enabled.

License
-------
This project is open source. You are free to use, modify, and distribute the code as per the license provided in the project repository (if applicable).

Contact
-------
For any questions, issues, or contributions, please contact pellegrini.ch@northeastern.edu or submit an issue via the project's repository (if available).

--------------------------------------------------
Enjoy using SBOM Viewer!
