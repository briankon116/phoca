# Phoca
Tool to analyze and classify websites as originating from a MITM phishing toolkit or not.

## Requirements
* python3.7

## Installation
Install Python dependencies using `python3.7 -m pip install -r requirements.txt`

## Usage
To access low-level network functions to create and send raw TCP packets, this tool requires sudo privilages.

Scan one website by specifying the domain or URL of the site:

`sudo ./phoca www.google.com`

Bulk scan multiple websites by supplying a csv containing one URL or domain per line:

`sudo ./phoca -r domains.csv`

Output results to a CSV file rather than terminal output:

`sudo ./phoca -r domains.csv -w results.csv`
