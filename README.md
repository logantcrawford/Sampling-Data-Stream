# sampling-data-stream
For real-world data mining applications, streamed data can come in fast, sampling can minimize the overwhelming data.

![Data Mining: Sampling and Counting ft. Twitter Data](assets/sampling.jpg)

For real-world data mining applications, streamed data can come in fast. It's estimated that every single day around 500 million tweets are posted. If we imagine that the data stored for each tweet is on average 1 kilobyte, that is 500 gigabytes daily.  For a large corporation like Twitter, this might be reasonable, but for researchers, data scientists, hobbyists, and smaller companies collecting data, this is exceptionally challenging. This isn't even including the processing and transformations made, which could slow the process down. But suppose we are prepared to collect specific information that is important to us. In that case, we can sample the incoming data to manage the vital information and drastically reduce storage space and processing time. We will be working with two types of sampling, random sampling and reservoir sampling, for this analysis. 

Random sampling is used to generate a subset of individuals chosen from a more extensive set in which a subset of individuals is chosen randomly. Though this method is excellent, it can suffer by missing out on a particular group. There are other ways to handle random sampling, but we will be working with a general lottery system for this analysis. 

Reservoir sampling is used to generate randomized algorithms for choosing a simple random sample, without replacement, of k items from a population of unknown size n in a single pass over the items.

Starting this analysis, we will begin the Tweepy API using my private Twitter API credentials. These can be updated through the `assets/` folder and creating an access.txt in the format:

`consumer_key = 'string'

consumer_secret = 'string'

access_token = 'string'

access_token_secret = 'string'

bearer_token = 'string'`
