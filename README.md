## JS Scan - "Scans hidden secrets and urls in JavaScript!"
This script is a sophisticated security tool designed for today's digital defenders. It has the capability to uncover hidden URLs and sensitive data within JavaScript files, providing security researchers, bug hunters, and developers with the means to enhance web security. Utilize this script to transform every line of code into a map of potential vulnerabilities ready to be explored.

### Installation JS Scan :

To install JS Scan, run the following commands:

```bash
git clone https://github.com/hackelite01/JS-Scan.git
cd JS-Scan
pip3 install -r requirements.txt
```

## Usage JS_Extract
Mass JS Link Scanner [JS_Extract] is a simple tool made to scan .js file links from a list of URLs automatically. Just provide a .txt file containing a list of target URLs, and the tool will collect all .js file links found on each page!

## Usage JS Scan :

Find urls with single target :
If you just want to find .js files from a specific URL, you can use curl and grep like this,
```bash
curl -s http://testphp.vulnweb.com | grep "\.js"
```
To run JS Scan, use the following command :

```bash
python3 JS_scanner.py -u http://testphp.vulnweb.com/urls.js --secrets --urls
```
Mass scanning with .txt file :
```bash
python3 JS_scanner.py [filejs.txt] --secret --urls
```

### Command-Line Options:
- `-u` or `--url`: Specify a single JavaScript URL to fetch.
- `--secrets`: Look for sensitive information in the JavaScript content.
- `--urls`: Extract URLs from the JavaScript content.
- `-o` or `--output_file`: Specify the file to save extracted links (default: `extracted_links.txt`).
