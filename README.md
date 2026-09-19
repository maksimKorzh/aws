# Alternative Web Scraping
<a href="https://maksimkorzh.github.io/aws/">READ ONLINE</a>

## Building Web Scrapers Inside the Browser

**Alternative Web Scraping** is a practical book about web scraping and an alternative approach to building scrapers: running the scraper directly inside the Chrome browser.

## About the Book

Traditional web scraping usually places the scraper outside the browser and attempts to reproduce the browser's behavior.

This book explores a different approach:

> Put the scraper inside the browser.

The browser already handles cookies, sessions, JavaScript, redirects, rendering, DOM manipulation, and navigation. Instead of reproducing all of this from an external program, we can use the browser itself as part of the scraping environment.

The book builds a complete Chrome extension that uses this approach.

## What You'll Learn

- Web scraping fundamentals
- How data appears on modern websites
- Listing and detail-page structures
- Traditional scraping with Scrapy
- Chrome extension architecture
- Browser local storage
- Visual element selection
- CSS selector generation
- Listing URL discovery
- Pagination
- Browser-based crawling
- Persistent scraper state
- Data extraction
- Testing
- Real-world scraping

## The Browser-Based Approach

The central idea of the book is that the browser itself can become part of the crawler.

Instead of building an external scraper that attempts to imitate a browser, our extension runs directly on the web page.

This is particularly useful when anti-scraping measures make traditional external scraping difficult.

It is not, however, a replacement for traditional scraping.

If a website can be scraped reliably with normal HTTP requests and a conventional parser, a traditional scraper is usually simpler, faster, and easier to maintain.

The goal is to choose the right tool for the problem.

## The Example Extension

Throughout the book we build a Chrome extension consisting of:

- `manifest.json`
- `menu.html`
- `menu.css`
- `menu.js`
- `ui.js`
- `scraper.js`

The extension allows the user to configure a scraper visually, store its configuration locally, discover listing URLs, navigate through pages, extract data, and download the collected results.

## Testing

The completed extension is demonstrated on two websites.

### Quotes

The first example uses:

https://quotes.toscrape.com/

This provides a simple environment for testing the extension and understanding the complete scraping workflow.

### Idealista

The second example uses:

https://www.idealista.com/

This demonstrates the same browser-based approach on a real-world website.

## Support

If you found the book useful and would like to support the project, donations are welcome through PayPal:

**PayPal:** maksymkorzh@gmail.com