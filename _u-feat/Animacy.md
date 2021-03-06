---
layout: feature
title: 'Animacy'
shortdef: 'animacy'
udver: '2'
---

<table class="typeindex" border="1">
<tr>
  <td style="background-color:cornflowerblue;color:white"><strong>Values:</strong> </td>
  <td><a href="#Anim">Anim</a></td>
  <td><a href="#Hum">Hum</a></td>
  <td><a href="#Inan">Inan</a></td>
  <td><a href="#Nhum">Nhum</a></td>
</tr>
</table>

Similarly to [Gender]() (and to the African noun classes), animacy is
usually a lexical feature of [nouns](u-pos/NOUN) and inflectional feature
of other parts of speech ([pronouns](u-pos/PRON),
[adjectives](u-pos/ADJ), [determiners](u-pos/DET), [numerals](u-pos/NUM),
[verbs](u-pos/VERB)) that mark agreement with
nouns. It is
independent of gender, therefore it is encoded separately in some
tagsets (e.g. all the Multext-East tagsets). On the other hand, in
Czech the (almost) only grammatical implications occur within the
masculine gender, which is why the PDT tagset does not have
animateness as separate feature and instead defines four genders:
masculine animate, masculine inanimate, feminine and neuter.  We
follow the two-feature approach used in Multext-East (many languages)
because it is safer.

Polish is special in that it also distinguishes grammatically human
vs. non-human animates. It can be demonstrated by inflection of words with
adjectival inflection, for example, the word _który_ "which" (boldface forms differ from the middle
row):

|------------------------------------------------------------------------------------------------------------------------------------------------|
| gender            | sg-nom | sg-gen  | sg-dat  | sg-acc    | sg-ins | sg-loc | pl-nom     | pl-gen  | pl-dat | pl-acc      | pl-ins  | pl-loc  | 
|------------------------------------------------------------------------------------------------------------------------------------------------|
| animate human     | który  | którego | któremu | którego   | którym | którym | **którzy** | których | którym | **których** | którymi | których | 
| animate non-human | który  | którego | któremu | którego   | którym | którym | które      | których | którym | które       | którymi | których | 
| in-animate        | który  | którego | któremu | **który** | którym | którym | które      | których | którym | które       | którymi | których | 
|------------------------------------------------------------------------------------------------------------------------------------------------|
{: cellpadding="2" cellspacing="0" }

More generally: Some languages distinguish animate vs. inanimate (e.g. Czech
masculines), some languages distinguish human vs. non-human (e.g. Yuwan, a
Ryukyuan language), and others distinguish three values, human vs. non-human
animate vs. inanimate (e.g. Polish masculines).

### <a name="Anim">`Anim`</a>: animate

Human beings, animals, fictional characters, names of professions
etc. are all animate. Even nouns that are normally inanimate can be
inflected as animate if they are personified. For instance, consider a
children's story about cars where cars live and talk as people; then
the cars may become and be inflected as animates.

### <a name="Inan">`Inan`</a>: inanimate

Nouns that are not animate are inanimate.

### <a name="Hum">`Hum`</a>: human

A subset of animates that only includes human beings (and personified characters)
but not animals.

### <a name="Nhum">`Nhum`</a>: non-human

In languages that only distinguish human from non-human, this value includes
inanimates. In languages that distinguish human animates, non-human animates
and inanimates, this value is used only for non-human animates, while `Inan`
is used for inanimates.
