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

