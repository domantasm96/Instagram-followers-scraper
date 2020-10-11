# Instagram followers scraper

Instagram scraping tool that collects information about users followers and unfollowers. Some remarks about IG srapping flow:

* **Instagram may temporary block after x continuous requests** - this tool is designed for scraping small profiles( < ~ 600 followers). If you want to scrape bigger profiles, then you would need IG accounts pool to rotate after x requests for preventing temporary blocks.
* **Only public accounts or people that you are following are visible** - If you want to scrape another IG profile, make sure that this profile is public or this user is in your following list
* **PLEASE DO NOT USE THIS APP FOR STALKING REASONS** - it is possible but it is wrong.

I designed this app for marketing analysis but IG have strict restrictions for each account requests so it is hard to scrape bigger profiles without getting temporary blocked. Do not worry if you get temporary blocked because of too much requests, after ~15 minutes cooldown you should be unblocked.   


Main code is in **InstaDron.ipynb** jupyter notebook file. 

Make sure, that if you want to track yours or other IG users followers list(I assume that you would track other people followers list for scientifics reasons) you have to:

1) **Setup database** - database and tables creation code is in **create_tables.sql** file. There would be tracked followers list of each user.
2) **Setup selenium** - make sure that selenium is installed and webriver is ready to use. More info you can find here: https://selenium-python.readthedocs.io/installation.html
3) **Setup credentials** - make sure that you setup credentials of database and instagram account user. Databse credentials is for storing information, IG account credentials is for scraping data of your or others users (this program is designed for running locally, so your information is safe. Personally, I'm storing creds in yml files and reading from them for additional safety)


Use at your own risk. 

If you have any questions or ideas - feel free to message me or raise an issue. 

