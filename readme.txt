This project is expected to take you 15-20 hours (once you understand
the course material). The benefit in marks of exceeding this time frame
will lead to diminishing returns, so only do so if you're having fun.

This dataset is about the use of words. It is derived from the U.S.
presidents' state of the union speeches over the past 200+ years.

Psychologists have developed a measure of the intellectual complexity
of a document in terms of how much it is aware of the possibility
of more than one viewpoint, and how much it goes into depth about
the content. This model was developed by Suedfeldt at UBC and is
called integrative complexity.

Political scientists have applied this measure to the state of the union
speeches. Each is given a score between 0 and 4. Most of them are in the
range 1-2.

The problem with integrative complexity is that it requires multiple
human scorers for each documents, so it's expensive to compute.

The goal of this project is to see whether or how much integrative
complexity can be predicted just from word frequencies. Since it's
easy and algorithmic to count word frequencies, such a model would
make integrative complexity much more widely useful.

Initially, this could be treated as a prediction problem: build
a predictor for integrative complexity (notice that this is regression).

However, the integrative complexity scores came from humans and so
may be slightly inaccurate. So it might make sense to discretize them,
say into high, medium, and low.

The data itself is a document-word matrix: each row corresponds to one
speech, and each column to one word. The entries in the matrix are the
counts of each word in each document. (Only the most frequent words
are counted.) Longer documents contain more words than shorter ones,
and so their counts are higher. To remove the effect of document
length, it's usual to divide the counts in a row by the sum of the
counts in that row. This changes word counts to word rates (can you see
why?).

You might want to start by looking at the properties of the data,
using both statistics and visualisation.

The clustering might provide some insight into how difficult the
prediction problem might be. Don't forget that the attributes
can be clustered as well as the records. Perhaps you can get some
insights into which words are important.  For example, simple nouns 
probably aren't very predictive because a complex speech could be about 
any topic.

Then you can try to build good predictions, using both classification
(with well-motivated class boundaries) and regression.

Attribute selection or ranking is also useful because it lets us
see which words are signals of this kind of complexity.

Your mark is not determined by your prediction accuracy. Rather, it
depends on the quality of your design, which techniques you try, in
which order. Don't be afraid to mention dead ends, as long as they
weren't obviously dead before you tried them. You don't have to build
every possible model, but you should build the best few, so that you
know your results are not an accident.

I have included the raw text of the speeches so that you can look at
them and get a feel for what they are like.

