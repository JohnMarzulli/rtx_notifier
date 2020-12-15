# A simple Python + Selenium Bot

This bot is intended to look for availability of GeForce RTX 3080 cards.

It's very straightforward to use but assumes a little knowledge of python.

Tested on Pop!\_OS.

## Installation

Installation is reasonable simple.

### Linux

1. Clone the code.
2. Validate that you have Python 3.8 or newer. This code uses newer Python features that are not compatible with Python 3.5
3. Run `sudo apt install firefox-geckodriver; pip3 install selenium`
4. Review the URLs that you would like to monitor in the `rtx_notifier.py` file
5. Run `python3 rtx_notifier.py`

### Windows

1. Clone the code.
1. Make sure you have Firefox installed.
1. Install Python 3.8 from https://www.python.org/downloads/release/python-386/
   1. Do not install Python 3.9
   1. Do not install from the Windows Store. This will cause permission issues.
1. Download the code and unzip it to a directory
1. Open a PowerShell prompt, navigate into the directory with the source code
1. Execute: `pip3 install selenium`
1. Download GeckoDriver from [https://github.com/mozilla/geckodriver/releases]
1. Unzip the folder and place `geckodriver.exe` into the folder `rtx_notifier`
1. Run the tool using `python3 rtx_notifier.py` using the command prompt.

Please note that this runs multiple, concurrent browsers simultaneously.

If a card is detected as available, the bot will attempt to add the product to your cart and pause all of the other browsers.

Good luck!
