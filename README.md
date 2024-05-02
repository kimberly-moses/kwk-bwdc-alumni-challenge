# kwk-bwdc-alumni-challenge
Analyze BWDC and Yelp API data to understand Black business trends and their impact on communities in Baltimore City, MD to contribute insights to BWDC and empower decision-makers to support Black-owned businesses.

# Dependencies
* Python3/pip3
* Packages listed in requirements.txt

# Installing Dependencies
```bash
$ pip install -r requirements.txt
```

# Configuration Management
Configuration information such as the database url/port, credentials, API keys etc are to be supplied to the application. However, it is bad practice to stage production information in publicly visible repositories.
Instead, all config is provided by a config file or via [environment variables](https://linuxize.com/post/how-to-set-and-list-environment-variables-in-linux/).

config.py
```python
SQLALCHEMY_DATABASE_URI = "sqlite:///yelp.db"
YELP_API_KEY = "<my_api_key>"
```

# Run Order
If running notebooks in this repo, you may want to run scraper.ipynb before the rest as data from this notebook is used for the others.