# Curated datasets for TEA

This repository contains curation data and the target articles for Pathogen Identifier and Strain Tagger datasets.

The curation data is stored in JSON format under curation_data and divided into two subfolders: pathogens for Pathogen Identifier dataset and strains for Strain Tagger dataset.

The JSON files contain curated article hash as a key followed by IOB-format compatible tag/location key-value pairs. The tag locations are indicated inside an array on word-level as a start index, followed by a plus sign and another number that indicates the length of the tag: e.g. strains/purple: [42+2, 153+1] means that there are two strains/purple tags starting from word number 43 and 154, and spanning for two words and one word (i.e. that word only).

See [TEA](https://github.com/tznurmin/TEA) repository for usage example.

## Entity categories

### Pathogen Identifier

| **Entity**     | **Number of tags** |
| -------------- | ------------------ |
| commensals     | 25                 |
| negatives      | 9322               |
| opportunistics | 37                 |
| pathogens      | 859                |
| probiotics     | 20                 |
| strains        | 123                |

### Strain Tagger

| **Entity** | **Number of tags** |
| ---------- | ------------------ |
| negatives  | 13181              |
| species    | 837                |
| strains    | 1788               |

The curated data is provided under MIT licence.

# Third-party licences

The target articles texts are found under source_articles. The article texts are licenced under various Creative Commons licences (i.e. BY/NC/SA).

See attribution.txt for article-level details and general attribution.
