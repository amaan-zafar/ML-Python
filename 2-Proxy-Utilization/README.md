# Proxy-utilisaton

Web URLs block IP's that programmatically (web scrapers, bots etc) try to scrape their web content. This is because it overloads their websites and thus brings their site response time down and strains underlying infrastructure.

What is the solution ?

Rotating IP's via proxy is a standard solution used along with timer interval introduced while scraping :

Go through this link: https://www.scrapehero.com/how-to-rotate-proxies-and-ip-addresses-using-python-3/

## Problem Statement

Hit the URL : https://fossbytes.com/10-best-free-music-websites-to-download-songs-legally/ ( or any particular URL of your choice), multiple times from your scraper and note the requests response ! While you 're getting 200 OK as response it's fine , but when it blocks you (as it did to me in session) then you 're going to re-route your IP via a proxy

To obtain various proxies , scrape https://free-proxy-list.net/ : free proxies listed over there via the html content which get refreshed every 10 mins (as per the site).

Use each of the proxy to access the web page that has blocked your IP and record the response of the webpage i.e 200 OK or some other response.We're trying to evaluate what percentage of these proxies work ( not all will) and the success hit ratio

Do this for around 100 different proxies and summarize what %age were successful and what were not, along with your observations.