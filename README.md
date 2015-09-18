# iKB - Knowledge-driven Database Engine

[![Build Status](https://secure.travis-ci.org/snowyu/ikb.png?branch=master)](http://travis-ci.org/snowyu/ikb)

iΚB is based on knowledge-driven hierarchical nosql database. Its main goals are:

* The knowledge base make computers and people can understand and use it
* Provide The Common Knowledge Classification
* Inference Engine build-in to reason and "think about"
* Peer to Peer Share Knowledge(machine to machine)
* Make your computer into a real logic-based electronic brain


In some ways It is similar to:

* nosql key/value database
* Graph database
* Wordnet
* Freebase
* Wikipedia
* Wolfram


But it is still quite different with the above-mentioned.


The differencement with Wolfram:

* Open Knowledge for ervery-one
* Peer to Peer Share/exchange/create Knowledge
* More Natural Language like human mother tongue.
* Open Source

## Database Specification

First it's a hierarchical nosql key/value database and the hierarchy is inheritance releationship only.

1. Each key is a knowledge item ID(identification)
1. A knowledge item only one meaning(more than one meaning is not allowed)
1. The `"key path"` indicates inheritance relationship(ISA) of the knowledge.
1. The key's inheritor called subkey of the key.
1. The key with `"attributes"` represents meronymy relationship(HASA).
   * The `"value"` is a special `"attribute"`.
1. The key with `"actions"` means executable functions or the key issued.


## The Common Knowledge Classification Specification

This section is similar to wordnet. But the differences are:

1. Encoding the knowledge item ID(identification) with Chinese Character
1. A knowledge item only one ID(identification) and one meaning(not allow to have multiple identification or explanations)
1. The root classification is different from Wordnet.

### Why encoding Knowledge ID with Chinese characters?

Generally, we use numbers and GUID as ID (identification) System.
But this ID is meaningless and difficult to maintain.

Chinese characters have a stable architecture, as well as plenty of character,
about more than 21,000 characters, and each character has its own meaning.

This makes the Chinese coding greatly reduces the storage footprint, and can have a clear meaning.
Anyway the meaningful ID should be better than meaningless ID.

eg,

* "attrbute" is is composed of eight Engilish characters. but Chinese, only two characters: "属性".
* "type" four characters for Engilish. one character for Chinese: "型".
* "English" serven characters for English, one character for Chinese: "英".


