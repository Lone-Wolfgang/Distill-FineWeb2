# Distill-FineWeb2

Hello, everyone. I'm working on the Japanese portion of FineWeb. During annotation, I noticed that the density of educational content is quite low. So far, fewer than 1% of examples have scored 3 or higher. To scale up the educational content, we’ll need a significantly larger sample.

Educational content is sparse. Most web material is geared toward entertainment or profit. Furthermore, isolating educational content from high-quality websites is not trivial. For instance, if you were to randomly select a URL from a site like HuggingFace, it’s highly likely that you’d end up with a catalog page.

For languages with a low density of educational material, the leadership of FineWeb has requested a list of high-quality URLs and IDs to prepare an additional sample for annotation.

My primary challenge is limited compute resources. Currently, I’m living abroad with a constrained setup: a 500 GB internal hard drive, a 2 TB external hard drive, and 16 GB of RAM. The Japanese segment of the dataset is quite large, totaling about 500 GB and divided into 146 shards.

In the notebook, I’ll share how I extracted a sample of IDs that are potentially high quality.

In the folder, 'IDs', you will find IDs from the FineWeb corpus that I have identified as potentially high quality. Right now, there are IDs from only a single website, but I am working on getting more.
