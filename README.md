<snippet>

# rs_assistant.py
Runescape helper tool for mass account request usage.

-Email request: Places email set on to current account.

-Password request: Places password reset request on to the current account.

-Twitch request: Working script. Ping for maintenance

-Launcher request: Creates shell script for all accounts listed in "accounts.txt"

-Verify request: TODO


## Usage
You must have python3 installed. Please go here for a direct download: https://www.python.org/download/releases/3.0/

You must have the latest chromedriver placed in the current directory of where your running the pything script.
Please go here for a direct download: https://chromedriver.chromium.org/

Stuff to edit:

Edit 'rs_assistant.py' if you want custom file names (Read in from the current directory).
Edit captcha_key field with your 2captcha key.

Parameters

- parser.add_argument('--email', help='adds a email request to the account(s)')
- parser.add_argument('--password', help='adds a password request to the account(s)')
- parser.add_argument('--twitch', help='adds a twitch request to the account(s)')
- parser.add_argument('--launcher', help='adds a launcher request from the account list')

e.g, python3 rs_assistant.py --twitch True

## Output
``` 
"passed_accounts.txt" - all accounts that have been ran through will be inside this file in the current directory.

