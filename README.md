# Anchore Security CVE 5 Enriched Dataset

> [!WARNING]  
> Although it is intended that this repo will become the place for community CVE 5 data curation contributions in future, currently contributions should be directed to https://github.com/anchore/vulnerability-index-spec-files
>

The data in this repo is a fork of https://github.com/anchore/dataset-security-cve5-control (which contains only the elements from the upstream CVE5 snapshot currently targeted for enrichment) with Anchore and community contributions added.  The general idea is that git will manage conflicts as upstream data changes and these can be resolved by curators as part of the merge process.  

Additional post-processing will take this enriched dataset, calculate the difference between this and the control set as a json patch, and then apply that to the last merged snapshot from https://github.com/anchore/dataset-security-cve5-upstream-snapshot (noted in the index.json file at the root of the repo).  This will render full CVE 5 json files for the full dataset.  These will be published to some yet to be determined publicly-accessible location for all downstream processing to utilise.