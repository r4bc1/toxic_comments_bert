# toxic_comments_bert
Toxic comments classification using BERT

At the end of 2017 the platform shut down and made their ~2m comments from their platform available in
a lasting open archive so that researchers could understand and improve civility in online conversations for
years to come. Then this effort was sponsored and its annotation was extended by human raters for various
toxic conversational attributes.

In the data supplied for this challenge, the text of the individual comment is found in
the commenttext column. Each comment in Train (toxtrain.csv) has a toxicity label (target), and models
should predict the target toxicity for the Test data (tox_test.csv). For evaluation, test set examples
with target >= 0.5 will be considered to be in the positive class (toxic).

The data also has several additional toxicity subtype attributes. Subtype attributes are:

    severe_toxicity
    obscene
    threat
    insult
    identity_attack

The goal of this challenge is to develop a model to predict target column, i.e. the level of toxicity of a
given comment, while 0 is non-toxic, and 1 is maximum level of toxicity.
Secondary goal is to detect additional subtypes of toxicity.
