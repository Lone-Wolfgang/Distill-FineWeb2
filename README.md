# Distill FineWeb2

Hello, everyone,

I’m working on the Japanese portion of FineWeb and noticed that the density of educational content is quite low. So far, fewer than 1% of examples have scored 3 or higher. To scale up the educational content, we’ll need a significantly larger sample.

Most web material is focused on profit or entertainment. Furthermore, isolating educational content from high-quality websites is challenging. For instance, randomly selecting a URL from a site like HuggingFace often leads to catalog pages instead of substantive content.

The FineWeb leadership has requested a list of high-quality URLs and IDs to prepare an additional sample for annotation, particularly for languages with limited educational material.

Currently living abroad, I’m working with limited compute resources: a 500 GB internal hard drive, a 2 TB external drive, and 16 GB of RAM. The Japanese segment of the dataset is quite large, totaling about 500 GB and divided into 146 shards. This repository relies on Polars to access large datasets without exhausting memory resources.

If you are working with FineWeb data with limited resources, this repository might be useful for you.

As of now, this repository has two notebooks:

- **preprocess.ipynb**: Documents the steps for grouping the FineWeb corpus by domain, which makes it easier to browse and analyze its contents. If you want to collect FineWeb IDs, please start here.  
- **collect_ids.ipynb**: Outlines a strategy for selecting websites, distilling educational content, and retrieving IDs from the FineWeb corpus.  
