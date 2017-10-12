# iKB - Knowledge-driven Database Engine

[![Build Status](https://secure.travis-ci.org/snowyu/ikb.png?branch=master)](http://travis-ci.org/snowyu/ikb)

iΚB is based on knowledge-driven hierarchical nosql database. Its main goals are:

* `One BIG` P2P knowledge database only
* The knowledge base make computers and people can understand and use it
* Provide The Common Knowledge Classification
* Inference Engine build-in to reason and "think about"
* Peer to Peer Share Knowledge(machine to machine)
* Make your computer into a real logic-based electronic brain


In some ways it is similar to:

* nosql key/value database
* Graph database
* Wordnet
* Freebase
* Wikipedia


But it is still quite different with the above-mentioned.


## Database Specification

First it's a hierarchical nosql key/value database and the hierarchy is inheritance releationship only.

1. Each key is a knowledge item ID(identification)
1. A knowledge item only one explanation(not allow to have multiple explanations)
1. The `"key path"` indicates inheritance relationship(ISA) of the knowledge.
  * use the posix path separator("/") to separate each key.
  * eg, `/creature/animal/deuterostomia/chordata/vertebrata/fish`
1. The key's inheritor called subkey of the key.
  * eg, `fish` is the subkey of the key `/creature/animal/deuterostomia/chordata/vertebrata`
1. The key with `"attributes"` represents meronymy relationship(HASA).
  * use the `'.'` dot prefix to express the attribute of a key. eg `/system/a.com/user/jack/.value`
  * The `"value"`, `"type"` is the special `"attributes"`.
1. The key with `"actions"` means executable functions or the key issued.
  * use the `'!'` exclamation mark prefix to express the action of a key. eg `/book/!open`

## The Common Knowledge Classification Specification

This section is similar to wordnet. But the differences are:

1. Encoding the knowledge item ID(identification) with Chinese Character
1. A knowledge item only one ID(identification) and one explanation(not allow to have multiple identification or explanations)
1. The root classification is different from Wordnet.



### Why encoding Knowledge ID with Chinese characters?

Generally, we use numbers and GUID as ID (identification) System.
But this ID is unmeaning and difficult to maintain. I wish it could be self-explanatory.

Chinese characters have a stable architecture, as well as plenty of character,
about more than 21,000 characters, and each character has its own meaning.

This makes the Chinese coding greatly reduces the storage footprint, and can have a clear meaning.

eg,

* "attrbute" is is composed of eight Engilish characters. but Chinese, only two characters: "属性".
* "type" four characters for Engilish. one character only for Chinese: "型".
* "English" serven characters for English, one character for Chinese: "英".
* "/creature/animal/deuterostomia/chordata/vertebrata/fish" for Chinese: "/生/动/后口/脊索/脊椎/鱼"

