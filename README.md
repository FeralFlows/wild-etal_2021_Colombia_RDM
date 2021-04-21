# wild-etal_2021_Colombia_RDM
Discovering Robust Deep Decarbonization Pathways for Colombia

## Contents
- [Abstract](#abstract)
- [RDM Computational Infrustructure](#robust-decision-making-computational-infrustructure)
- [Code Reference](#code-reference)
- [Journal Reference](#journal-reference)
- [Contributing Models](#contributing-models)
- [Data Reference](#data-reference)
- [Reproduce My Experiement](#reproduce-my-experiement)

<br />

## Abstract


[Back to Contents](#contents)

<br />

## Robust Decision Making Computational Infrustructure

<a name="figure1"></a>

<p align="center"> <img src="Figures/RDM Infrastructure v2.png", width = '700'></p>

**Figure 1.** Robust Decision Making (RDM) computational infrustructure.

[Back to Contents](#contents)

<br />

## Code Reference
<!-- for each minted software release for all code involved.  If you have modified a codebase that is outside of a formal release, and the modifications are not planned on being merged back into a version, fork the parent repository and add a `.<shortname>` to the version number of the parent and conduct your own name.  For example, `v1.2.5.hydro`.-->
[1] **GCAM**. authors.  GCAM-LAC v5.3. repository DOI.

<!--
#### Example:

Wild, T.B. (2020). Colorado Nexus Repository. Github. https://github.com/FeralFlows/wild-etal_2020_ColoradoNexus.git
-->

[Back to Contents](#contents)

<br />


## Journal Reference
Journal reference will be updated after acceptance.

[Back to Contents](#contents)

<br />

## Contributing Models

<a name="table1"></a>
**Table 1:** Model repository and DOI links.

| Model | Version | Repository Link/DOI |
|-------|---------|---------------------|
| GCAM-LAC | v5.3 | <DOI>|

[Back to Contents](#contents)

<br />

## Data reference

### Input Data

<a name="table2"></a>
**Table 2:** Input data for each model and DOI links.

| Input Data Category | Model | DOI | Description |
|---|---|---|---|
| Climate Impacts | GCAM-LAC v5.3 | <http://doi.org/10.5281/zenodo.4708046> | [XML files] Climate impacts on ag, hydro, and runoff. |


### Output Data
GCAM output queries are located wild-etal_2021_Colombia_RDM/runs/query_proj/.


<!--
#### Example:
Human, I.M. (2020). My dataset name [Data set]. DataHub. https://doi.org/some-doi-number
-->

[Back to Contents](#contents)

<br />




## Reproduce My Experiement

### Install Metis

1. Clone and install metis to your desired location from www.github.com/JGCRI/metis. This Metis GitHub repository has detailed installation instructions.

```
git clone https://github.com/JGCRI/metis.git
```

2. Checkout the metis model version used to run this publication's experiments. The git "tag" that points to the version/commit of metis used to run this publication's experiments is "wild_et_al_2020_ColoradoNexus". Nevigate into the cloned metis folder and run the following command to checkout the 'tagged' metis version.

```
git checkout tags/wild-etal_2021_Colombia_RDM
```

3. To use the 'tagged' metis version associated with this paper, go to cloned metis folder, open metis.Rproj, select Build -> Document. Then select Build -> Install and Restart. If you previously installed metis, reload metis.

```
devtools::unload("metis")
library(metis)
```

### Reproduce Results

1. Clone reproducible repository into your desired location.

```
git clone https://github.com/FeralFlows/wild-etal_2021_Colombia_RDM.git
```

2. To process GCAM output queries (.proj files) and produce figures, run metrics_paper.R script within metrics folder.

3. To determine the percentage of scenarios below/above 10th/90th percentile, as described in the paper, run metrics_post_processing.R.


</details>

[Back to Contents](#contents)
