# iKB - Knowledge-driven Database Engine

iΚB is based on knowledge-driven hierarchical nosql database. Its main goals are:

* The knowledge base make computers and people can understand and use it
* Provide The Common Knowledge Classification
* Inference Engine build-in to reason and "think about"
* Peer to Peer Share Knowledge
* Make your computer into a real logic-based electronic brain


In some ways It is similar to:

* nosql key/value database
* Graph database
* Wordnet
* Freebase
* Wikipedia


But it is still quite different with the above-mentioned.


## Database Specification

First it's a hierarchical nosql key/value database and the hierarchy is inheritance releationship only.

1. Each key is a knowledge item
1. A knowledge item only one explanation(not allow to have multiple explanations)
1. the `"key path"` indicates inheritance relationship(ISA) of the knowledge.
1. The key with `"attributes"` represents meronymy relationship(HASA).
   * The `"value"` is a special `"attribute"`.
1. The key with `"actions"` means executable functions or the key issued.


## The Common Knowledge Classification Specification

This section is similar to wordnet. But

1. Encoding the knowledge item with Chinese Character
1. A knowledge item only one explanation(not allow to have multiple explanations)
1. The root classification is different from Wordnet.

### Why encoding with Chinese characters?

Chinese characters have a stable architecture, as well as plenty of character,
about more than 21,000 characters, and each character has its own meaning.

This makes the Chinese coding greatly reduces the storage footprint, and can have a clear meaning.

eg, "attrbute" is is composed of eight Engilish characters. but Chinese, only two characters: "属性".




