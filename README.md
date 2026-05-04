IT23210288 – IT3040 Assignment 1
Project Title
Automated Testing for Singlish to Sinhala Transliteration System
Repository
https://github.com/Isuri123Dewmini/IT3040-Assignment-1

Project Structure
IT3040_Assignment_1/
├── test_automation.py          → Playwright automation script
├── IT23210288 - Test cases.xlsx → Excel file with test cases & results
├── requirements.txt            → Python dependencies
└── README.md                   → Project documentation

Technologies Used

Python
Playwright (UI Automation)
OpenPyXL (Excel handling)


How to Run the Project
Step 1: Open terminal inside the project folder
Step 2: (Optional) Activate virtual environment
bashvenv\Scripts\activate
Step 3: Install dependencies
bashpip install -r requirements.txt
playwright install
Step 4: Run the automation script
bashpython test_automation.py --excel "IT23210288 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator"

Output
Results are automatically written back to the Excel file after each test run.
Columns updated:

Actual output – The Sinhala text returned by the application
Status – PASS or FAIL based on comparison with expected output


Test Case Details

Total Test Cases: 50
Test Type: Negative Testing (FAIL cases only)

Covered Scenarios
CategoryExamplesMixed language inputsSinglish + English words/phrasesSpelling variationsAbbreviated, truncated, and phonetic variantsEmojis & symbolsEmoji-embedded Singlish sentencesReal-world scenariosBanking, travel, platform names, person namesNumeric & date inputsCurrency, time formats, ordinal numbersOnline identifiersURLs, email addresses, @mentions

Important Notes

This system uses strict string comparison between expected and actual output
Even minor differences in Sinhala output (spacing, formatting, spelling) will result in FAIL
Some failures are expected due to:

Transliteration inconsistencies in the application
Complexity of mixed-language (Singlish + English) inputs
UI timing delays during automation




Student Information
FieldDetailsStudent IDIT23210288ModuleIT3040 – IT Project ManagementAssignmentAssignment 1 (Option 1)

Final Status
TaskStatusAutomation script✅ WorkingExcel-based validation✅ CompletedTest coverage (all 24 input types)✅ Covered with ≥ 2 test cases each

Submission Notes

Virtual environment (venv/) is excluded from submission
All required files are included in the submission folder
Project is fully runnable using requirements.txt
