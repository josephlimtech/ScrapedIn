# ScrapedIn
Tool to scrape LinkedIn

This tool assists in performing reconnaissance using the LinkedIn.com website/API for red team or social engineering engagements. It performs a company specific search to extract a detailed list of employees who work for the target company. Enter the name of the target company and the tool will help determine the LinkedIn company ID, which will be used to perform the search.

**NOTE:** The tool extracts the maximum results of any search (1,000 contacts) by sendings less than 20 requests. 

Output is stored as an XLSX file, however it is intended to be used with Google Spreadsheets and includes a formated report with profile pictures, etc. After importing the XLSX into Google Spreadsheets there will be a "dataset" worksheet and a "report" worksheet.

## How to install
```
sudo apt-get install python3-pip -y
sudo pip install -r requirements.txt
```

## How to run

```
export LI_USERNAME={username}
export LI_PASSWORD={password}
```

`python3 ScrapedIn.py`

[ScrapedIn Demo.webm](https://github.com/dchrastil/ScrapedIn/assets/26440487/6f7888f9-2fe3-49d7-b6a3-229e508a9da3)

![ScrapedIn_running](https://github.com/dchrastil/ScrapedIn/assets/26440487/dc99742e-0b73-4aa7-ae1c-34ee6ab1eb25)

![ScrapedIn_report](https://github.com/dchrastil/ScrapedIn/assets/26440487/ac563397-391d-4059-89df-cb7305b6163a)


## dataset
- first name
- last name
- occupation
- location
- industry
- profile URL
- picture URL

## report
- Picture (displayed)
- Full Name, Occupation
- Link to Profile

## Sponsorship
<a href="https://nubela.co/proxycurl?utm_campaign=influencer_marketing&utm_source=github&utm_medium=social&utm_content=daniel_chrastil_scrapedin">
<img src="https://github.com/josephlimtech/linkedin-profile-scraper-api/blob/master/Proxycurl_scrape_LinkedIn.png" width="350px" height="100%" alt="Proxycurl APIs enrich people and company profiles with structured data" />
</a><br><br/>

> Scrape public LinkedIn profile data at scale with [Proxycurl APIs](https://nubela.co/proxycurl?utm_campaign=influencer_marketing&utm_source=github&utm_medium=social&utm_content=daniel_chrastil_scrapedin).
> - Scraping Public profiles are battle-tested in court in HiQ VS LinkedIn case.
> - GDPR, CCPA, SOC2 compliant
> - High rate Limit - 300 requests/minute
> - Fast APIs respond in ~2s
> - Fresh data - 88% of data is scraped real-time, other 12% are not older than 29 days
> - High accuracy
> - Tons of data points returned per profile
>
> Built for developers, by developers.

### Disclaimer
this tool is for educational purposes only and violates LinkedIn.com's TOS. Use at your own risk.


