# Distill FineWeb2

Hello, everyone,

I’m working on the Japanese portion of FineWeb and noticed that the density of educational content is quite low. So far, fewer than 1% of examples have scored 3 or higher. To scale up the educational content, we’ll need a significantly larger sample.

This scarcity is due to the web’s focus on entertainment or profit-oriented material. Isolating educational content from high-quality websites is challenging. For instance, randomly selecting a URL from a site like HuggingFace often leads to catalog pages instead of substantive content.

To address this, FineWeb leadership has requested a list of high-quality URLs and IDs to prepare an additional sample for annotation, particularly for languages with limited educational material.

I face some constraints in this task. Living abroad, I’m working with limited compute resources: a 500 GB internal hard drive, a 2 TB external drive, and 16 GB of RAM. The Japanese segment of the dataset is quite large, totaling about 500 GB and divided into 146 shards.

As of now, this repsository has two notebooks:

- **preprocess.ipynb**: documents the steps for grouping the FineWeb corpus by domain, which makes it easier to browse and analyze its contents.
- **webscraping.ipynb**: outlines a couple of stratgies for compiling promising links by webscraping and exctracing the appropriate IDs fomr the FineWebCorpus.

In the folder labeled "IDs," you’ll find IDs from the FineWeb corpus that I’ve identified as potentially high quality. Currently, these IDs are from a two websites, but I am working on adding more.