# Bots Can Marry Too
Wedding Automaton Using Twilio, Python 2.x, and Google 

## How to Run
First, you will need to install a few dependencies. Refer to the table below for links:

### Dependency Table
Dependency | Installation Guide
---------- | ------------------
Python 2.x | [python installer](https://www.python.org/downloads/release/python-272/)
Pip Package Manager | [pip installer](https://pypi.org/project/pip/)
Twilio | [free trial](https://www.twilio.com/)
Flask | [Sahil Rajput's Flask Web API tutorial](https://dev.to/sahilrajput/install-flask-and-create-your-first-web-application-2dba)
Google Spreadsheet | [gspread tutorial](https://www.twilio.com/blog/2017/02/an-easy-way-to-read-and-write-to-a-google-spreadsheet-in-python.html)

## Overview
Employs [Twilio](https://www.twilio.com/) SMS for outbound messaging at scale and quick response handling. 

Replies to outbound messaging R.S.V.P requests, which are parsed conditionally (y/N) using [Flask](https://flask.palletsprojects.com/en/1.1.x/quickstart/) as a webserver, pointing the Twilio Messaging Request URL to a **./messages** url.

Calculates attendance list in real-time, producing an instant-feedback feature. 

Guests who've confirmed their R.S.V.P are subsequently encouraged to select their food options from a listing. 

Food choices are updated and communicated to the sender by the same statistical logic as the R.S.V.P.

Once a confirmed list of guests, each having submitted their confirmed food of choice, the stats are made public to ease the demand on the catering company.

If there happens to be one or several guests who procrastinate their R.S.V.P or food choice, SMS messages will be deployed as reminder.

A final SMS will remind guests of the commitment they have undertaken, basic details, and regulations.

