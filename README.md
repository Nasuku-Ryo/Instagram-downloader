# Instaloader: Instagram Data Scraping Tool

Instaloader is a powerful tool to download Instagram posts, profiles, stories, and more directly from the command line. This guide will help you get started with installing and using Instaloader efficiently

# Tabel of Contents
- [installation](#installation)
- [Basic Usage](#Basic-Usage)
- [Downloading Profiles](#Downloading-Profiles)
  - [Downloading Profile Picture Only](#Downloading-Profile-Picture-Only)
  - [Downloading Latest Posts](#Downloading-Latest-Posts)
- [Advanced Options](#Advanced-Options)
  - [Downloading by Hashtag](#[Downloading-by-Hashtag)
  - [Downloading Specific Posts by Date](#Downloading-Specific-Posts-by-Date)
- [Downloading Stories and Highlights](#Downloading-Stories-and-Highlights)
- [Saving to Specific Directories](#Saving-to-Specific-Directories)
- [Automating Downloads](#Automating-Downloads)


# installation
To download an Instagram profile, use the following command:
```
pip install instaloader
```
Ensure Python is installed and added to your PATH.

# Basic Usage
To download an Instagram profile, use the following command:
```
instaloader profile <username>
```

# Downloading Profiles
## Downloading Profile Picture Only
```
instaloader --no-posts --profile-pic-only profile nasa
```
## Downloading Latest Posts
```
instaloader --count=5 profile nasa
```
This downloads the latest 5 posts from the profile.

# Advanced Options
## Downloading by Hashtag
```
instaloader "#nature"
```
Posts with the hashtag #nature will be downloaded.

## Downloading Specific Posts by Date
```
instaloader --post-filter="date_utc >= datetime(2023, 1, 1)" profile nasa
```
This downloads posts published after January 1, 2023.

# Downloading Stories and Highlights
To download stories and highlights, you must log in first.
```
instaloader --login your_username --stories profile nasa
```
After logging in, you can download:
```
instaloader --highlights profile nasa
```

# Saving to Specific Directories
By default, Instaloader saves files to the current directory. To change this:
```
instaloader --dirname-pattern=./instagram_data profile nasa
```
Or specify an absolute path:
```
instaloader --dirname-pattern="C:/Users/YourName/Instagram/nasa" profile nasa
```

# Automating Downloads
Automated downloads by creating script
```
instaloader profile nasa
```
Then schedule it using cron (Linux/Mac) or Task Scheduler (Windows).






















