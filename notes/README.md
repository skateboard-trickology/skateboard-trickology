# notes/ — knowledge log for Skateboard Trickology

One Markdown file per trick or trick concept. The frontmatter is plain YAML (no RDF
here — the semantics live in the TTL file). Point Obsidian at this
folder.

## Rules
1. **Filename = the IRI's local name in kebab-case**, set once, never
   changed. `:MuteGrab` → `mute-grab.md`. Name changes are handled via
   `label` + `aliases`, not a new filename.
2. **The `iri` field in the frontmatter must be quoted** (`":MuteGrab"`)
   — values starting with a colon are otherwise invalid YAML.
3. **`tags` use the ontology classes' local names** (e.g. `grabTrick`),
   so the tag set can be compared against `rdf:type` later.
4. **`status` flow:** research → draft → mature → in-ontology.
   When knowledge is lifted into the TTL (e.g. as `skos:changeNote`),
   set status to `in-ontology`. Keep the note as raw material.
5. New note: copy `_template.md`.

## Workflow
```
cp notes/_template.md notes/new-concept.md
# ...write...
git add . && git commit -m "notes: new-concept" && git push origin main
```
