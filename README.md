# Adidas Account Generator

## Note
This is a adjusted version of ryan9918's Adidas Account Generator (https://github.com/ryan9918/adidas-account-gen). I made quite a few changes that are listed in the Changes. Thanks to WeeSkilz for helping me with this.

## Description
A tool coded in Python that allows the user to generate accounts for Adidas US, Adidas UK and Adidas DE using a catch-all domain.
The tool supports the recent captcha requirement change by Adidas.  Accounts are created in the format `RANDOMLETTERRANDOMNUMBER@DOMAIN` with a random password.
The password and the domain can be edited in `config.json`.

## Changes
- I added Adidas DE as region. But you can still use UK and US.
- The HTML file was updated.
- The generator generates random letters instead of using a prefix for the first part of the email
- The E-Mail format was changed.
- You can now set a unique password for all accounts instead of random passwords.
- You can now change all personal details in the `config`.


## Requirements
- Python 3+
- `requests`
- `bs4`
- `flask`
- `colorama`
- `termcolor`

## Installation and Usage
- You need to add the below line to your hosts file (google how to do this if you do not know)
- `127.0.0.1 germanconnec.adidas.de`
- Make sure you have installed all of the modules listed above, using `pip install` (or `pip3 install` if you have python2 too) to do so
- Edit `config.json` with a suitable editor e.g. sublime or atom (NOT NOTEPAD)
- `cd` into the directory location
- `python main.py` or `python3 main.py` if you also have python2 installed and added to path
- You must SOLVE CAPTCHAS MANUALLY (one per account you want to create)


## Notes
- Try check your email inbox for adidas account creation emails to make sure the accounts are actually being created
- If you choose 100 accounts, be prepared to solve 100 captchas. If you exit the script before all accounts have been created they will NOT be saved
