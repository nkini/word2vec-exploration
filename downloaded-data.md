### Pre-trained word2vec vectors
- Google News data subset (about 100 billion words)
  - GoogleNews-vectors-negative300.bin.gz
  - Uses negative sampling
  - The model contains 300-dimensional vectors for 3 million words and phrases. 
  - The phrases were obtained using a simple data-driven approach described in [2]. 
  - Approx. 1.5 GB compressed

- English Wikipedia (Feb 2015)
 - Referenced at [4]. 
 - Project is "Generating Vectors for DBpedia Entities via Word2Vec and Wikipedia Dumps".
 - 1000 dimension
 - No stemming - 10skipgram
 - Approx. 8.6 GB compressed
  
### Raw training data
- Gutenberg All English (October 2014)
  - http://webapps.stackexchange.com/questions/12311
  - 42.8GB compressed
  
- Text8 corpus by Matt Mahoney
  - 100MB of cleaned English Wikipedia dump on Mar. 3, 2006
  - Part of a larger (entire en.wiki) text corpus
  - Referenced at [5]

- English Wikipedia for Nov 2015
  - /media/nikhil/Education/UCSC/290C/NLP/AllenAI/knowledge/originals/enwiki-20151102-pages-articles-multistream.xml.bz2
  - Current revisions only, no talk or user pages; 
  - 13.3GB compressed (expands to over 50 GB when uncompressed).
  - Referenced at [6]

### Other possibly helpful data
 - Freebase/Wikidata Mappings
  - Based on the Wikidata-Dump of October 28, 2013
  - Contains only those links that have at least two common Wikipedia-Links and not a single disagreeing Wikipedia-Link. 
  - Furthermore, the lines are sorted by the number of common Wikipedia-Links (although in Turtle this does not really matter).
  - Total triples: 2.1M
  - Updated: October 28, 2013
  - Data Format: N-Triples RDF
  - 21.2 MB gzip, 242.9 MB uncompressed
  - Referenced at [7]
  
- Freebase Triples
  - /media/nikhil/Education/UCSC/290C/NLP/AllenAI/knowledge/originals/freebase-rdf-latest.gz
  - This dataset contains every fact currently in Freebase. 	
  - Total triples: 1.9 billion
  - Data Format: N-Triples RDF
  - 32 GB gzip
  
- OpenCyc
  - Available, but I have no idea what it is or does. TODO: Find out
  - /media/nikhil/Education/UCSC/290C/NLP/AllenAI/knowledge/originals/opencyc-4.0-linux.tgz

#### References
    [1] Tomas Mikolov, Kai Chen, Greg Corrado, and Jeffrey Dean. Efficient Estimation of Word Representations in Vector Space. In Proceedings of Workshop at ICLR, 2013.
    [2] Tomas Mikolov, Ilya Sutskever, Kai Chen, Greg Corrado, and Jeffrey Dean. Distributed Representations of Words and Phrases and their Compositionality. In Proceedings of NIPS, 2013.
    [3] Tomas Mikolov, Wen-tau Yih, and Geoffrey Zweig. Linguistic Regularities in Continuous Space Word Representations. In Proceedings of NAACL HLT, 2013.
    [4] https://github.com/idio/wiki2vec/
    [5] http://mattmahoney.net/dc/textdata
    [6] https://en.wikipedia.org/wiki/Wikipedia:Database_download#English-language_Wikipedia
    [7] https://developers.google.com/freebase/data#citing
