# Timesheet Reminder Bot

Sends a reminder via Discord webhook to remind you to submit your timesheet. Assumes timesheets are due on the 15th and last days of the month, or the closest non-holiday weekday before.

## How to Run:

`python -m venv env`

`source env/bin/active`

`pip install -r requirements.txt`

`python timesheet_bot.py`

The idea is to set up a venv and run timesheet_bot.py with a cronjob each weekday. If you'd rather just leave a program running somewhere, check out [The apscheduler version](https://github.com/ThorntonMatthewD/timesheet_bot/tree/use-apscheduler). You might have to set `daemon=true` depending how you want to use it.
