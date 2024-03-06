# Microsoft Assessment - Daily News Downloader

## Overview
This Selenium IDE script automates the seamless retrieval of the latest PDF from DailyEPaper, a platform regularly updating public-accessible PDF files. Specifically designed for the Times of India section, the script navigates through the website, efficiently clicking through pages, and initiating downloads.

## Process 
1. **Open Main Site:**
   - The script starts by opening the main [DailyEPaper](https://www.dailyepaper.in/daily-news/) website.

2. **Navigate to Times of India Section:**
   - It proceeds to click on the Times of India link, which in turn leads to a webpage housing PDFs organized by date.

3. **Select Latest PDF for the Current Month:**
   - The script identifies and selects the latest available PDF.

4. **Open Selected Newspaper in a New Tab:**
   - After identifying the PDF, the script opens it in a new tab for further processing.

5. **Initiate Download:**
   - It initiates the download process for the selected newspaper PDF.

6. **Close Unnecessary Tabs:**
   - The script closes unnecessary tabs, leaving the downloaded PDF accessible.

## Website
- [DailyEPaper](https://www.dailyepaper.in/daily-news/)
  - I chose this website because:
    - It hosts free PDFs.
    - Daily newspapers often update PDFs, making it suitable for testing our script.

## Prerequisites
- [Selenium IDE](https://www.selenium.dev/selenium-ide/) - Install this to view Selenium scripts.
- [Selenium Side Runner](https://www.seleniumhq.org/selenium-ide/docs/en/introduction/command-line-runner/) - Install this to run Selenium scripts from the command line.
- ChromeDriver or GeckoDriver - Choose the appropriate driver based on your preferred browser.
- [Commands](https://www.seleniumhq.org/selenium-ide/docs/en/api/commands) - Commands for creating scripts in Selenium IDE

## Usage
1. **Install Dependencies:**
   - Install Selenium-side-runner in the terminal:
     ```bash
     > npm install -g selenium-side-runner
     ```
   - For Chrome, install chromedriver:
     ```bash
     > npm install -g chromedriver
     ```
   - For Firefox, install geckodriver:
     ```bash
     > npm install -g geckodriver
     ```

2. **Run Selenium Script:**
   - Open a terminal and navigate to the project directory.
   - Execute the following command to run the Selenium script:
     ```bash
     > selenium-side-runner -c "browser=chrome" Daily_news_downloader.side
     ```

3. **Note**:
   - On the first run, you might be prompted to 'allow pop-ups for this site.' Please grant permission to prevent any potential interference with the script's functionality in the future.

## Feedback
   - If you encounter any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License
   - This project is licensed under the MIT License - see the LICENSE.md file for details.
