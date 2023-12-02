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
    - Turn on GitHub Actions
    - Set up your .yml file
        - BE SURE TO MAKE SURE YOUR NOTEBOOK NAME MATCHES!!!!
3. Make a website!!!
    - Create an index.html
    - Add it to your repo and push it up to GitHub
    - Turn on GitHub Pages by clicking many buttons
    - Make sure your index.html works by visiting your page
4. Make a visualization for our webpage
    - We're going to use DataWrapper!!!
    - Make sure we're linking to our data, not uploading it
    - Use the 'responsive iframe' version of embedding
5. Update our website
    - Add the embed code to our index.html
    - Push it on up to GitHub Pages
    - Wait for GitHub actions to finish deploying our web page
6. Party!!!!