---
layout: relation
title: 'obl'
shortdef: 'oblique argument or adjunct'
udver: '2'
---

The `obl` relation is used for oblique nominal arguments and adjuncts of verbs, adjectives or adverbs.

`obl` is a [noun](NOUN) (or noun phrase) functioning as a
non-core (oblique) argument or adjunct.
This means that it functionally corresponds to an adverbial when it attaches to a verb, adjective or other adverb.

~~~ sdparse
Ես հանդիպեցի նրան անցյալ չորեքշաբթի ։ \n I-have-met him last Thursday .
obl(հանդիպեցի, չորեքշաբթի)
obl(I-have-met, Thursday)
~~~

The obl relation can be further specified by the case. In conjunction with the case relation, it provides a uniform analysis for:

*	variant forms with case, a preposition or a postposition, 

~~~ sdparse
Դուրս_եկավ տնից ։ \n He-went-out from-the-house.`Abl` .
obl(Դուրս_եկավ, տնից)
obl(He-went-out, from-the-house.`Abl`)
~~~

~~~ sdparse
Նա նստած էր ծառի տակ ։ \n He-was sitting under the-tree.`Dat` .
obl(նստած, ծառի)
case(ծառի, տակ)
obl(sitting, the-tree.`Dat`)
case(the-tree.`Dat`, under)
~~~

*	obl is also used for temporal and locational nominal modifiers:

~~~ sdparse
Երեկոյան հանդիպեցի նրան սրճարանում ։ \n I-met him in-the-evening in-the-cafe .
obl(հանդիպեցի, Երեկոյան)
obl(հանդիպեցի, սրճարանում)
obl(I-met, in-the-evening)
obl(I-met, in-the-cafe)
~~~
