# bow_nli
bag of words for natural language inference

The SNLI task poses the following problem: Given two pieces of text, a premise, and a hypothesis, you (or a model) have to choose one of the following:

1. The premise entails the hypothesis.
2. The premise contradicts the hypothesis.
3. The premise neither entails nor contradicts the hypothesis and is thus neutral to it.

For example:
1. 
Premise: A man inspects the uniform of a figure.
Hypothesis: The man is sleeping.

This is a contradiction since the man cannot be sleeping while inspecting the uniform.

2. 
Premise: A soccer game with multiple males playing. 
Hypothesis: Some men are playing a sport.

This is entailment because the hypothesis is true whenever the premise is true.

3. 
Premise: An older and younger man smiling.
Hypothesis: Two men are swimming and laughing at the cats playing on the floor. This is neutral because the premise does not contain any information about cats.

Being based on natural text, there will be some ambiguity regarding the answers. Nevertheless, the NLI-style tasks have shown to be effective for training models to capture aspects of semantic information from text. 

Refer to https://nlp.stanford.edu/projects/snli/, or the original paper (https://nlp.stanford.edu/pubs/snli_paper.pdf) for more details. You will be provided with tokenized training and validation pickle files.
