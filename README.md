# Distill-FineWeb2

Hello, everyone,

I’m working on the Japanese portion of FineWeb and noticed that the density of educational content is quite low. So far, fewer than 1% of examples have scored 3 or higher. To scale up the educational content, we’ll need a significantly larger sample.

This scarcity is due to the web’s focus on entertainment or profit-oriented material. Isolating educational content from high-quality websites is challenging. For instance, randomly selecting a URL from a site like HuggingFace often leads to catalog pages instead of substantive content.

To address this, FineWeb leadership has requested a list of high-quality URLs and IDs to prepare an additional sample for annotation, particularly for languages with limited educational material.

I face some constraints in this task. Living abroad, I’m working with limited compute resources: a 500 GB internal hard drive, a 2 TB external drive, and 16 GB of RAM. The Japanese segment of the dataset is quite large, totaling about 500 GB and divided into 146 shards.

In my notebook, I’ll demonstrate how I extracted a sample of potentially high-quality IDs. To do this, I analyzed the websites contributing to the FineWeb corpus. The data has been preprocessed, allowing me to quickly query the number of pages and URLs contributed by each site. I’ve focused on the largest contributors, identifying domains with some educational content and scraping promising links. Using this list of links, I query the preprocessed data and compile the corresponding IDs if the links are present.

The notebook explains how I preprocessed the data, and how to scrape using BeautifulSoup.

In the folder labeled "IDs," you’ll find IDs from the FineWeb corpus that I’ve identified as potentially high quality. Currently, these IDs are from a single website, but I am working on adding more.
