# PRV
PRV - Parallel Routing Vector  
this project is an extension of my  
oneAPI contest entry "PRT"  

here's the concept:  
whereas my my actual contest entry  
implements simple CAM (Content Addressable Memory) functionality,  
which returns a result index (into the actual result table),  
based upon a direct match of a parallel searched for index key;  

this project attempts to generalize the concept, 
to provide a result vector,  
indicating a best statistical probabilty. 




modules:

	PRV-SC  Spelling Correction

		analyzes individual input words, 
		and considers possible spelling corrections; 
		
	PRV-RV	Rating Vector

		implements a: context aware, sequential classification, of input sentences;
		producing a multi-dimensional output vector based upon statistical probability rating.



Spelling  -  Theoretical Basis:

based upon the research of the:
Natural Language Processing Group at Stanford University 
https://nlp.stanford.edu/
https://nlp.stanford.edu/IR-book/html/htmledition/spelling-correction-1.html
https://nlp.stanford.edu/IR-book/html/htmledition/implementing-spelling-correction-1.html

they developed algorithms to determine "Edit Distance",  
which expresses "various alternative correct spellings" 
in terms of:  
  "the minimum number of edit operations required to transform" String1 into String2
https://nlp.stanford.edu/IR-book/html/htmledition/edit-distance-1.html

k-gram indexes can improve upon isolate word corrections
(K-grams are k-length subsequences of a string)
https://nlp.stanford.edu/IR-book/html/htmledition/k-gram-indexes-for-spelling-correction-1.html

although general purpose (sugestive) spelling correction can be implemented,
common spelling errors relevant to particular knowlege domains might yield better results.




NLP (natural language processing)  -  Theoretical Basis:

Google developed: BERT (Bidirectional Encoder Representations from Transformers) 
which "is a Transformer-based machine learning technique for natural language processing (NLP) pre-training"
https://en.wikipedia.org/wiki/BERT_(language_model)




in my project developmental efforts, 
I would like to evaluate: 

Word2vec, which represents distinct words as numbers in a vector
https://en.wikipedia.org/wiki/Word2vec

semantic similarity between the words represented by those vectors, 
is expressed mathematicaly as a scaler value of cosine similarity between the vectors;
which if it works, indicates the level of semantic similarity between the words represented by those vectors.

https://en.wikipedia.org/wiki/Inner_product_space
https://en.wikipedia.org/wiki/Cosine_similarity




I would like to experiment with (Google) TensorFlow 
to try to implement deep NLU (Natural Language Understanding) networks 
via "Tensors", which are multidimensional arrays (matrices).

RNN (Recurrent Neural Networks) 
https://en.wikipedia.org/wiki/Recurrent_neural_network

express sequences of words (sentences) as "chain structures",
with internal links between processing nodes 
expressing the "recurrent" functionality


LSTM (Long Short-Term Memory)
https://en.wikipedia.org/wiki/Long_short-term_memory




this extension project is in conceptual research and development stage.

