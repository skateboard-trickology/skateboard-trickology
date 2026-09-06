---
iri: ":LocalName"          # frozen at creation, never changes. PascalCase for
                           # tricks and skaters, lowerCamelCase for enum values
label: ""                  # current name -> rdfs:label / skos:prefLabel
aliases: []                # former/alternative names -> skos:altLabel
type: trick                # trick | compositeTrick | skater | enumValue | class | property | concept
tags: []                   # ontology class local names, e.g. Grabtrick
inventedYear: ""           # a single year, e.g. 1978. Anything vaguer goes in History
inventedBy: ""             # the skater that invented the trick
firstMakeBy: ""            # the skater that landed it first, like the 1260 by Mitchie Brusco
namedAfter: ""             # who or what the name points at, e.g. Monty grind -> Monty Nolder
popularizedBy: []          # who made the trick popular
origin: ""                 # origin place or scene
difficulty: ""             # basic | intermediate | advanced | pro
noteStatus: research       # research | draft | mature | in-ontology, about this note
reviewStatus: unreviewed   # unreviewed | inReview | verified | disputed
reviewedBy: []             # person who has reviewed the text and given a thumbs up
reviewedDate: ""           # date of that review, YYYY-MM-DD
confidence: low            # low | medium | high, strength of the sources
sources: []                # URLs, articles, interviews
---

# Title (current name)

## Description
Briefly, what the trick/concept is.

## History
Origin, name changes, evolution over time. With sources.

## Curated text 
The public-facing text — what a reader gets beyond the bare definition.
Written from Description and History, but as prose someone would actually
want to read. Becomes dcterms:description.

## Open questions
- [ ]

## Ontology notes
What this means for the model: class membership, enum values,
candidates for skos:changeNote/historyNote, known collisions.