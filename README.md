<snippet>

# rs_assistant.py
Runescape helper tool for mass account request usage.

-Email request: Places email set on to current account.

-Password request: Places password reset request on to the current account.

-Twitch request: Working script. Ping for maintenance

-Launcher request: Creates shell script for all accounts listed in "accounts.txt"


## Usage
Program grabs account list from the current directory.

"accounts.txt" - the list of runescape accounts to run through

"twaccounts.txt" - the list of twitch accounts to run through iff twitch_request = True

Parameters

- parser.add_argument('--email', help='adds a email request to the account(s)')
- parser.add_argument('--password', help='adds a password request to the account(s)')
- parser.add_argument('--twitch', help='adds a twitch request to the account(s)')
- parser.add_argument('--launcher', help='adds a launcher request from the account list')

e.g, python3 rs_assistant.py --email True

## Output
``` 
"passed_accounts.txt" - all accounts that have been ran through will be inside this file in the current directory.

