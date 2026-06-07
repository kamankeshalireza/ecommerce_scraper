🛒 E‑commerce Scraper
A professional web scraper built with Scrapy to extract product data from online stores – perfect for price monitoring, market research, or learning web scraping.

⚠️ For educational & personal use only. Always check the target website's robots.txt and terms of service before scraping.

✨ Features
Extracts product title, price, availability, images, descriptions

Saves data to JSON, CSV, or XML

Handles pagination (follows "next page" links automatically)

Respectful scraping with custom User-Agent and DOWNLOAD_DELAY to avoid getting blocked

🚀 Quick Start
1. Clone the repo

git clone https://github.com/kamankeshalireza/ecommerce_scraper.git
2.
cd ecommerce_scraper

3. Install dependencies

pip install -r requirements.txt

4. Run the spider (example)

scrapy crawl product_spider -o products.json
💡 Replace product_spider with the actual name of your spider (check inside the spiders/ folder).

📁 Project Structure
text
ecommerce_scraper/

├── ecommerce_scraper/

│   ├── spiders/          # Individual spiders (one per website)

│   ├── items.py          # Product data model

│   ├── middlewares.py    # Proxy & header management

│   ├── pipelines.py      # Data cleaning & processing

│   └── settings.py       # Scrapy settings

├── requirements.txt      # Python dependencies

└── scrapy.cfg            # Scrapy configuration
🧠 Why I built this
To get hands‑on experience with web scraping and the Scrapy framework. This project taught me how to extract clean, structured data from complex websites efficiently – without hammering the target server.

📈 What's next
Add rotating proxies to avoid IP bans

Store data in PostgreSQL or MongoDB

Build a simple Streamlit dashboard to visualize price changes

🤝 Contributing
Found a bug or have an idea? Feel free to:

Open an Issue

Submit a Pull Request

📜 License
MIT – use it, modify it, learn from it.
