### Instruction
The `data.zip` file is the exact data partitioning for each aspect of the original work. It has `IMDb_id` as the unique key of referring to the corresponding movies on `imdb.com`. The `severity_rating` column has links to the severity rating items under `Parent Guide`. We do not release the rating digits directly due to regulation concerns, but it is very easy to use the ids and links we provide to collect the up-to-date ratings by the users. If the user would like to use the rating digits exactly the same as the paper is based on, please contact the author.

The movies script text is hosted at our research group website: https://ritual.uh.edu/1493-2/. It contains the movie corpus, a collection of movie subtitles, and metadata for about 15k movies. One should simply match the movie scripts and the ratings on `IMDb_id`, then the dataset is ready to use.

The `Sample_data.csv` provides a sample dataset with dummy data entries. The code can be applied to the data in the same format as the sample data.

Research purposes only.
