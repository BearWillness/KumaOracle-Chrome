Kuma Oracle Extension
Version: 1.0
Overview
Kuma Oracle is an official Kuma Capital extension designed to automatically evaluate the impact of real-world events on risk assets. It extracts content from the active tab, analyzes the data using the OpenAI API, and provides insightful feedback on how different assets will be affected in the short, medium, and long term. This extension is ideal for traders, analysts, and those interested in understanding market sentiment and the impact of current events.

Features
Content Extraction: Automatically extracts content from web pages, including articles and main content blocks.
OpenAI Integration: Uses OpenAI's GPT model to analyze real-world events and determine the impact on various assets.
Asset Impact Analysis: Provides detailed short-term (STA), medium-term (MTA), and long-term (LTA) asset impact evaluations.
API Key Management: Allows users to input their own OpenAI API key, securely storing it for future analysis.
Interactive UI: Presents results with an intuitive, sleek design and allows users to expand each asset's section to see detailed reasoning behind the analysis.
Customizable Popup: A modern, trading-terminal-style interface to keep the user experience professional and visually appealing.
Installation
Download the Kuma Oracle Files: Clone or download the repository files into a folder on your local machine.

Load Unpacked Extension:

Open Chrome and navigate to chrome://extensions/.
Enable "Developer mode" in the top-right corner.
Click on "Load unpacked" and select the folder where you saved the extension files.
Pin the Extension: Once loaded, click the puzzle icon on the Chrome toolbar, find the Kuma Oracle extension, and click the pin icon to ensure it's easily accessible.

Usage
Extract Content: Visit any webpage that contains financial or news content related to markets, and click the Kuma Oracle extension icon in your toolbar.

Analyze Data:

Click "Extract & Analyze Content" to initiate the process.
The extension will extract the main content from the page and send it to the OpenAI API for analysis.
View Results:

The results will display affected assets and the expected impact across different time frames (STA, MTA, LTA).
Click on each asset to view the reasoning behind the analysis for short, medium, and long-term impacts.
API Key Setup:

On first use, or when you need to update the API key, click the "Settings" option in the dropdown.
Enter your OpenAI API key in the input field and click "Save API Key".
The key will be saved and used for future analyses.
Extension Components
manifest.json
Defines the core capabilities of the extension, including content scripts, background workers, and required permissions.

background.js
Handles the click event of the extension icon and communicates with the content script to initiate content extraction.

kuma.js
Extracts the relevant article or main content from web pages. It sends the extracted content back to the popup for analysis.

popup.html
The main user interface for the extension, featuring buttons, text outputs, and a sleek design using the Inter font.

popup.js
Handles interactions within the popup, such as calling the content script to extract data, sending the data to the OpenAI API, and displaying the results.

API Integration
The extension requires an OpenAI API key to function. You can supply your own key through the settings option in the popup.
Once the content is extracted from a webpage, it is sent to OpenAI's API to analyze market sentiment and asset impact.
Permissions
activeTab: Allows the extension to interact with the currently active tab to extract content.
storage: Used to store the OpenAI API key locally for future analysis without needing to re-enter it.
Development
If you'd like to contribute or make changes, here’s how you can set up your development environment:

Clone this repository.
Modify the source code as needed.
Load the unpacked extension in Chrome using chrome://extensions/.
Test your changes by clicking the extension icon and using the "Extract & Analyze" button.
Troubleshooting
If you see a message stating "Error: No content to analyze," ensure that you're on a page that contains an article or relevant content.
Make sure your OpenAI API key is valid. You can update the API key in the Settings popup.
If you encounter issues parsing the JSON response from OpenAI, ensure that the API response follows the correct format as specified in the request.
License
This extension is licensed under the MIT License. See the LICENSE file for more information.

Contact
For more information, visit Kuma Capital or reach out to us via the official website.
