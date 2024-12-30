# Instaloader: Instagram Data Scraping Tool

Instaloader is a powerful tool to download Instagram posts, profiles, stories, and more directly from the command line. This guide will help you get started with installing and using Instaloader efficiently

# Tabel of Contents
- [installation](#installation)
- [Basic Usage](#Basic-Usage)
- Downloading Profiles
  - Downloading Profile Picture Only
  - Downloading Latest Posts
- Advanced Options
  - Downloading by Hashtag
  - Downloading Specific Posts by Date
- Downloading Stories and Highlights
- Saving to Specific Directories
- Automating Downloads
- Notes

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










