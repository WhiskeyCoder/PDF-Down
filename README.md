# 🧾 pdf_down.py

**Description:**
This script scrapes a webpage and downloads all PDF files it finds. The files are saved in a local folder named after the domain of the target website, with periods replaced by underscores for safe directory naming.

---

## 📥 How It Works
- Sends a request to the target website.
- Parses the HTML with BeautifulSoup.
- Locates all hyperlinks ending in `.pdf`.
- Creates a folder based on the website's domain.
- Downloads each found PDF to that folder.

---

## 🔧 Requirements
- `requests`
- `beautifulsoup4`
- Python 3.x

You can install the dependencies using:
```bash
pip install requests beautifulsoup4
```

---

## 🚀 Usage

Edit the script and replace this line:
```python
url = 'https://YOUR_WEBSITE_ADDRESS_GOES_HERE/'
```
with your desired target URL.

Then run the script:
```bash
python pdf_down.py
```

Downloaded PDFs will appear in a folder named like the domain:
```
📂 example_com
  ├── somefile.pdf
  └── anotherfile.pdf
```

---

## 💡 Notes
- Handles HTTP 404 errors gracefully.
- Automatically creates the destination folder.
- Uses a common browser User-Agent to avoid basic bot blocks.

---

## 🧠 Example Output
```
https://example.com/files/report.pdf
Downloaded: example_com/report.pdf
```

---

## 🛡️ Disclaimer
This script is for **educational purposes only**. Respect robots.txt, site terms, and copyright laws when scraping or downloading content.

---

## 📜 License
MIT License

