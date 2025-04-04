# Review_scraper_project 

 G2 Product Review Scraper (Google Colab-Ready)

This Python script allows you to scrape product reviews from G2.com for any SaaS company using ScraperAPI. It is built to run easily on Google Colab and outputs the reviews in a structured JSON file.

---

## 📌 Features

- ✅ Scrapes product reviews from G2.com using a company slug
- ✅ Outputs a JSON file containing:
  - Product name
  - Total number of reviews
  - Individual reviews with username, summary, review body, rating, date, and review URL
- ✅ Downloadable file via Google Colab
- ✅ Uses ScraperAPI to bypass IP bans and scraping protection

---

## 🚀 How to Use

1. Open the script in Google Colab.

2. Install required libraries:
   You only need to run the first code cell once:
   ```python
   !pip install requests beautifulsoup4 lxml
Run the main script. It will prompt you to enter:

🔑 Your ScraperAPI Key 3a55462bcbf5ecc5534d373ab351391c

🏢 The company slug (example: amazon-web-services, slack, zoom, etc.)

Once executed, it will:

Fetch reviews from G2.com

Save the results as a JSON file (e.g., amazon-web-services_g2_reviews.json)

Automatically download the file to your machine

🧠 What is a "Company Slug"?  https://www.g2.com/
A company slug is the name used in the G2 product URL. For example:

G2 URL: https://www.g2.com/products/amazon-web-services/reviews

Slug: amazon-web-services

Some other examples:

Slack → slack

Zoom → zoom

Google Workspace → google-workspace

🔐 Get Your ScraperAPI Key
Go to: https://www.scraperapi.com

Sign up for a free account (no card required)

Copy your API key from the dashboard

💡 Notes
This script only scrapes the first page of reviews. For full pagination support, enhancements will be needed.

Always check the G2.com Terms of Service before scraping.

Works only with products listed on G2.

📁 Output
The output is a downloadable JSON file with the following structure:

json
Copy
Edit
{
  "product_name": "Amazon Web Services",
  "number_of_reviews": "1,230 Reviews",
  "reviews": [
    {
      "username": "Jane D.",
      "summary": "Powerful cloud platform",
      "review": "AWS provides a scalable solution...",
      "date": "March 2024",
      "url": "/products/amazon-web-services/reviews/abc123",
      "rating": "5"
    },
    ...
  ]
}
🛠 To-Do (Optional Enhancements)
Add pagination to scrape multiple pages of reviews

Filter reviews by date range

Add support for other platforms (e.g., Capterra, TrustRadius)

👨‍💻 Author
Built with ❤️ by Yash 



after run this
Output: A file like Slack_capterra_reviews.json will appear in the Explorer pane.

Option 2: Run with VS Code Run Button
Output appears in the terminal, and the JSON file is saved in the project folder.
