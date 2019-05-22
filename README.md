# NaverBlog-Twitter-Youtube-crawling

## 0. Installing
- How to install

```
git clone https://github.com/phillip0726/NaverBlog-Twitter-Youtube-crawling.git
cd NaverBlog-Twitter-Youtube-crawling/
pip install -r requestments.txt
```

## 1. Functions
### Crawling
### Data Filtering, extraction
### Youtube video extraction, convert to mp3 files.

## 2. Crawling
* 2.1 Naver Blog Crawling
  - You have to enter the keyword.
  - After enter the keywork, you have to enter the number of page to crawl.
  - This program only crawls blog preview content.
  - The data is stored in a csv file named '/data/naver_comment.csv'
* 2.2 Youtube Comment Crawling
  - You have to enter the keyword.
  - First step, crawls the URL of all videos for that keyword.
  - The data is stored in a csv file named 'youtube_url_collection.csv'.
  - Second step, read 'youtube_url_collection.csv' file.
  - Third step, access all URLs and crawl all comments, stored in a csv file named '/data/youtube_comment.csv'.
* Twitter Posts Crawling
  - You have to enter the keyword.
  - Search for that keyword on Twitter, and crawl all posts.
  - The data is stored in a csv file named '/data/twitter_comment.csv'.

## 3. Data Filtering, extraction
* 3.1 Filtering
  - The words to be filtered are stored in '/data/except_spam/spam.txt'.
  - When A is executed, refined data is stored in '/data/except_spam/'.
* 3.2 Extraction
  - '/data/filtering_keyword_or.py' perform an OR operation on the input keywords.
  - '/data/filtering_keyword_and.py' perform an AND operation on the input keywords.
  - When these files are executed, extracted dataes are stored in '/data/include_keyword/'.
## 4. Youtube video extraction, convert to mp3 files.
* a
