# Hansel 🍪
**Your Favorite Persona Extension**

<img src=https://github.com/keremgirenes/persona-extension-comp491/assets/69321438/611b4e5b-3ec3-4b69-9346-31794caf2af3 alt="Banner Image" height="300">
<img src=https://github.com/keremgirenes/persona-extension-comp491/assets/69321438/6b1381ee-4b8f-421e-a82b-60eb356644d5 alt="Demo GIF" width=600 height=300>

## Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Setting Up Web-Crawling](#setting-up-web-crawling)
   - [Installing Packages](#installing-packages)
   - [Running the API](#running-the-api)
4. [Building the Chrome Extension](#building-the-chrome-extension)
   - [Building the Extension](#building-the-extension)
   - [Loading the Extension in Chrome](#loading-the-extension-in-chrome)
5. [Usage](#usage)
6. [Troubleshooting](#troubleshooting)
7. [Contributing](#contributing)
8. [License](#license)

## Introduction
Hansel 🍪 is a Chrome extension designed to fool web trackers based on user-created personas. This guide will help you set up and run the extension on your local machine.

## Prerequisites
Before you begin, ensure you have the following installed on your machine:
- Python 3.8 or higher
- pip (Python package installer)
- Flutter SDK
- Google Chrome browser

## Setting Up Web-Crawling
To set up the web-crawling component of the project, follow these steps:

### Installing Packages
1. Open your terminal or command prompt.
2. Navigate to the `web-crawling` directory:
   ```bash
   cd web-crawling
3. Install the required packages using pip:
   ```bash
   pip install -r requirements.txt

### Running the API
1. Start the API server using uvicorn:
   ```bash
   uvicorn main:app --reload
2. Your local host is now running and ready to accept requests from the web extension.

## Building the Chrome Extension
To build and load the Chrome extension, follow these steps:

### Building the Extension
1. Navigate to the `ui` directory:
   ```bash
   cd ui
2. Build the extension using Flutter:
   ```bash
   flutter build web --web-renderer html --csp

### Loading the Extension in Chrome
1. Open Google Chrome and navigate to `chrome://extensions`.
2. Enable `Developer mode` by toggling the switch in the top right corner.
3. Click on the `Load unpacked` button.
4. Select the build directory within the `ui` directory.

## Usage
Once the extension is loaded in Chrome, you can start using it by clicking on the extension icon in your browser. Follow the on-screen instructions to begin fooling web-trackers.

## Troubleshooting
If you encounter any issues during the setup or usage of the extension, refer to the following steps:

- Ensure all dependencies are installed correctly.
- Check the terminal or command prompt for error messages.
- Restart the API server and reload the extension in Chrome.

## Contributing
We welcome contributions to enhance the functionality and performance of Hansel 🍪. If you would like to contribute, please fork the repository, create a new branch, and submit a pull request with your changes.

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

Feel free to reach out if you have any questions or need further assistance. Enjoy your free cookie 🍪!
