# Learning Graph Generator Session Log

- **Skill:** learning-graph-generator v1.07
- **Date:** 2026-11-02
- **Book:** Transmission Lines, Fields, and Waves (EE3601)

## Python programs used

| Program | Version | Notes |
|---|---|---|
| csv-to-json.py | 1.05 | Generated `learning-graph.json`, including Concept Impact Scores (CIS) |
| analyze-graph.py | not versioned | Wrote `quality-metrics.md` |
| taxonomy-distribution.py | not versioned | Wrote `taxonomy-distribution.md` |
| validate-learning-graph.py | not versioned | Schema validation, run with the `jsonschema` package |
| add-taxonomy.py | not used | TaxonomyIDs were written directly into the CSV |

The scripts were run with the system Python 3.9. The JSON schema check and the
MkDocs build used a temporary virtual environment with MkDocs 1.6.1,
mkdocs-material and jsonschema.

## Steps

1. **Course description check — skipped.** `docs/course-description.md` already
   had `quality_score: 100`, which is above 85.
2. **Concept list.** Drafted 416 concepts. The author cut the list after
   concept 392 (Friis Transmission Equation). That removed Wireless Link, the
   tools and measurement concepts (Python, TDR, VNA, simulation), and the
   engineering design concepts, including the capstone project.
3. **Dependency graph.** Wrote the prerequisites for each concept, then
   converted the labels to ConceptIDs, checking that every label matched and
   that no concept depended on itself.
4. **Quality validation.** Valid DAG with 0 cycles, 0 orphaned nodes and 1
   connected component. There are 8 foundational concepts and 74 terminal nodes
   (18.9%), the average is 1.89 dependencies per concept, and the longest chain
   has 29 concepts.
5. **Taxonomy.** 14 categories. The largest is Electrostatics at 12.2% and the
   smallest is Antennas at 4.3%.
6. **JSON.** `learning-graph.json` has 392 nodes, 726 edges and 14 groups, and it
   passes schema validation. The top concepts by CIS are Cartesian Coordinates,
   Unit Vector, Scalar Field, Vector Field, Electric Charge and Sinusoidal
   Signal. All are foundational, which confirms the edges point the right way.
7. **Reports and navigation.** Wrote `concept-taxonomy.md`,
   `taxonomy-distribution.md` and `index.md`, and added every page to the
   `nav:` block in `mkdocs.yml`. `mkdocs build --strict` exits clean.

## Files created

- `docs/learning-graph/concept-list.md`
- `docs/learning-graph/learning-graph.csv`
- `docs/learning-graph/learning-graph.json`
- `docs/learning-graph/taxonomy-names.json`
- `docs/learning-graph/color-config.json`
- `docs/learning-graph/metadata.json`
- `docs/learning-graph/concept-taxonomy.md`
- `docs/learning-graph/quality-metrics.md`
- `docs/learning-graph/taxonomy-distribution.md`
- `docs/learning-graph/index.md` (rewritten from `index-template.md`)
- Copies of the skill's Python scripts and `learning-graph-schema.json`
