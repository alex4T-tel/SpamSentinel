# SpamSentinel

SpamSentinel is a lightweight web-based spam and phishing message detection tool. It analyzes user-provided text and assigns a risk score based on predefined spam indicators, suspicious phrases, links, and formatting patterns.

## Overview

SpamSentinel is designed to provide a quick assessment of whether a message may contain spam or phishing-related characteristics.

The application analyzes messages locally in the browser and displays:

* Risk score from 0 to 100
* Detected suspicious indicators
* Spam or safe classification
* Basic analysis details

## Features

* Spam and phishing message analysis
* Weighted risk scoring system
* Detection of suspicious keywords and phrases
* Detection of external links
* Detection of excessive capitalization
* Detection of suspicious punctuation patterns
* Detection of currency-related indicators
* Character counter with a 2,000-character limit
* Light and dark mode
* Responsive and minimal interface
* No external backend required

## Detection System

SpamSentinel uses a rule-based scoring system.

### Critical Risk

Certain indicators immediately increase the risk score significantly. Examples include:

* OTP
* ATM PIN
* CVV
* Account suspended
* KYC update
* Send money
* Claim prize

### Severe Risk

High-risk keywords contribute additional points, including:

* Congratulations
* Password
* Urgent action
* Crypto
* Bitcoin
* Bank account
* Lottery
* Wire transfer

### Medium Risk

The system also checks for common promotional or suspicious phrases such as:

* Winner
* Won
* Guaranteed
* Cash bonus
* Limited time
* Act now
* Click here
* Investment

### Low Risk

Less severe promotional indicators include:

* Free
* Promo
* Discount
* Offer
* Clearance

### Formatting Analysis

The system also considers:

* External URLs
* Excessive uppercase words
* Repeated exclamation marks
* Repeated question marks
* Currency symbols

## Risk Classification

The default risk threshold is **60**.

Messages with a score of 60 or higher are classified as high-risk. Messages below the threshold are classified as having no detected threat.

The final score is capped at 100 for display purposes.

## Technology

* HTML5
* CSS3
* JavaScript
* Client-side rule-based analysis

## How to Run

No installation or server configuration is required.

1. Download or clone the project.
2. Open the HTML file in a modern web browser.
3. Enter a message in the input field.
4. Select **Run Spam Analysis**.
5. Review the risk score and detected indicators.

## Limitations

SpamSentinel is a rule-based detection system and should not be considered a complete security solution.

Its accuracy depends on the rules and indicators defined in the application. Messages using unfamiliar wording or avoiding known indicators may not be detected.

For production use, the system could be improved by integrating a trained machine-learning model, larger datasets, URL reputation analysis, natural language processing, and continuously updated threat intelligence.

## Project Purpose

This project demonstrates how a browser-based security tool can combine multiple indicators to perform basic spam and phishing message analysis.

It is intended for educational purposes, security experimentation, and demonstrating rule-based threat detection concepts.

## License

This project can be used and modified for educational and personal projects. Add an appropriate open-source license if the project is published publicly.
