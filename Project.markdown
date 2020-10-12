---
layout: page
title: Projects
permalink: /project/
---
### [A Graph-Based Dependency Parser](https://github.com/kazzyabe/graph-parser)
This parser extended [a perceptron part-of-speech tagger](https://github.com/ftyers/conllu-perceptron-tagger.git) into dependency parser. It works on any of universal dependency corpus in a conllu format. 

The parser first scores each possible edge using perceptron, and figure out a maximum spanning tree. 

### [A Jointly Trained Part-Of-Speech (POS) tagger and Graph-Based Parser](https://github.com/kazzyabe/Joint_POS_PARSE)
This is a extension of the above project. Instead of training POS tagger and dependency parser separately, it trains them at the same time to avoid the error propagation. 

With the parser above, you have to run a POS tagger before running the parser because POS tags are a important feature that is used in the parser. Therefore, the error of the POS tagger is propagated to the parser. To avoid this propagation, a tagger and a parser is trained using the shared features.

### [A POS Tagger with handcrafted features](https://github.com/kazzyabe/POS_Handcrafted_feat_NN)
This is a slight extension of [a POS tagger](https://becominghuman.ai/part-of-speech-tagging-tutorial-with-the-keras-deep-learning-library-d7f93fa05537), implemented with tensorflow. I adopted the parser to data with conllu format.

### [A POS Tagger with Elmo Embeddings](https://github.com/kazzyabe/POS_Elmo)
This is a extension of the project above. Instead of using handcrafted features, Elmo embeddings are used for representing words. Implemented with tensorflow as well.

