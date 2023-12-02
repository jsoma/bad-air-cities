# Auto-updating air quality website

A (series of??) tutorials on auto-updating charts using GitHub Actions, GitHub Pages, and DataWrapper. One day this will include a link to the YouTube video!

## The problem

There's a website with some data! The data is great, the display is... not.

## The steps

We need to abduct the data and make our own visualization of it.

1. Turn the website's data into a CSV of our own (in this case, we're going to scrape it!)
    - Used `pd.read_html` to find all of the `<table>` elements
    - Grabbed the first table as our data 
    - Cleaned it up a bit
    - Saved it as `air-quality.csv`
2. Make that update automatically!
    - Make it a GitHub repository
    