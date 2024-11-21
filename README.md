# GOBY: An Enterprise Benchmark for Data Integration

## Abstract
Leading large language models (LLMs) are trained on public data. However, the majority of the world’s data is dark data not pub- licly accessible, mainly in the form of private organizational data or enterprise data. We show that the performance of LLM-based methods seriously degrades when tested on real-world enterprise datasets. Current benchmarks, based on public data, overestimate the performance of LLMs. We release a benchmark of enterprise data, the Goby benchmark, to the scientific community to advance discovery in the area of enterprise data management. Based on our experience with this enterprise benchmark, we propose tech- niques to uplift the performance of LLMs on this more challenging data distribution: these are (1) hierarchical annotation (2) runtime class-learning and (3) ontology synthesis. We show that one these techniques are deployed, performance on enterprise data is on par with public data.

## Dataset Overview

The **GOBY Benchmark Dataset** is designed to aid in evaluating data integration methods on structured enterprise data. This dataset includes categories, entities, and results derived from various data sources, represented in a unified schema. Key components include:

- **Tags**: Attributes within the unified schema.
- **Results**: Records sourced from wrappers, often web scrapers targeting specific sites.
- **Entities**: Records from original data sources, represented with "tags" that correspond to unified attributes.
- **Wrappers**: Data sources, typically web scrapers generating structured output.

---

## Contents of Goby

The primary data archive, `goby.tar.gz`, contains the following key directories:

- `dump/`: PostgreSQL dump files that include:
  - `doit_categories`: Data categories with record counts.
  - `doit_data`: Triple-based data representing (category_id, source_id, entity_id, name, value).
  - Additional mapping and result files.

---

## Download Instructions

To access the GOBY dataset:

1. Download the `goby.zip` file from the repository (link forthcoming).
2. Extract it using a tool like:
   ```bash
   unzip -P your_password goby.zip -d /path/to/extract/


## Download the Goby Benchmark
The benchmark mentioned in the abstract can be downloaded [here](https://fabian-ai.github.io/goby/) using the download button with the passcode:
```
GOBY2025
```

## Acknowledgments
Parts of this project page were adopted from the [Nerfies](https://nerfies.github.io/) page.

## Website License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
