We know that transformer networks, unlike recurrent networks, are non-sequential, which
makes them somewhat weaker in time series problems. Various methods exist to address
this challenge through modifications in positional encoding, the attention module, and at
the architecture level. In this task, you will become familiar with one of the most recent
proposals, called the iTransformer network, and implement it yourself. The related paper
is indexed in ICLR 2024, and the corresponding model code is available on their GitHub.
Since the model is new and there aren't many resources available about it, it is essential
to read both the paper and the GitHub repository to understand the concept of the
iTransformer. You are required to implement the predictive model using both the
transformer and iTransformer networks, so you can compare their performance. The
training data is related to the exchange rates of 8 countries over time, and since there are
8 variables to predict, it is considered a multivariate problem.
The strength of the iTransformer will particularly show in problems with high-dimensional
variables over time. Note that both the transformer and iTransformer models must be
written by you without using predefined functions such as nn.transformer (you must write
the attention and FeedForward blocks yourself, but you may use nn.layernorm for layer
normalization). After implementing both models, you will notice the differences between
them
