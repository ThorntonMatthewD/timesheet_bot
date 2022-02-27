# Timesheet Reminder Bot

Sends a reminder via Discord webhook to remind you to submit your timesheet. Assumes timesheets are due on the 15th and last days of the month, or the closest non-holiday weekday before.

## How to Run:

`python -m venv env`

`source env/bin/activate`

`pip install -r requirements.txt`

`python timesheet_bot.py`

The idea is to set up a venv and run timesheet_bot.py with a cronjob each weekday. If you'd rather just leave a program running somewhere, check out [the apscheduler version](https://github.com/ThorntonMatthewD/timesheet_bot/tree/use-apscheduler). You might have to set `daemon=true` in the scheduler config depending how you want to use it.

Example crontab setup with a venv running the script at 09:30 Monday thru Friday:
![Example crontab setup with a venv running at 09:30 Monday thru Friday](https://user-images.githubusercontent.com/44626690/155641707-079e8744-fb2a-45e0-8d7a-8fb2ee674917.png)
