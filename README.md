# 1. Conduct a scan of the ODIS graph targetting any schema.org type that mentions microbes using SILVA taxonomy

## Repository Structure

- `documentation/`: Documentation files.
- `scripts/`: Scripts for SPARQL queries, Python data processing, etc.

When attempting to extract all the child clauses of bacterial and archaeal taxa from the SILVA database, we curated the headers of all the microbial genomes as follows:
- The species name's epithet was removed, and any duplicate generic names were eliminated. 
- We also removed non-alphabetic characters from the list and referenced species by their corresponding numbers. 
- Additionally, we excluded names shorter than four characters and those containing more than two consecutive identical letters.


Some names still seemed unfamiliar, and there were still some acronyms for specific categories and some environmental descriptions like "blood" or "stool". Reviewing this entire list would require more time and manually checking for these unusual names.
Instead, we relied on the different taxonomic levels from the most common marine microbes, as documented in the literature:

/Users/gaetanemagali/OIH_rotation/documentation/Most_common_microbes.png 

Overmann, J., Lepleux, C. (2016). Marine Bacteria and Archaea: Diversity, Adaptations, and Culturability. In: Stal, L., Cretoiu, M. (eds) The Marine Microbiome. Springer, Cham. [https://doi.org/10.1007/978-3-319-33000-6_2](https://doi.org/10.1007/978-3-319-33000-6_2)


Both lists can be found on the following Zenodo upload: 
- [Zenodo Record](https://zenodo.org/records/12571310?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6Ijk2MjhkYzAwLTMyNmYtNGU1OC1iZTFlLWI5M2FlMDFlNWU2OSIsImRhdGEiOnt9LCJyYW5kb20iOiJjY2E0OGU4ODNiMzVlZjBjOWNjYWY0OWQ3ODkyODkwOSJ9.d4HYua3NmaACGy1TJ0WkzdkwgbZ0reyqmcX3UpfhDVmtKcTL7CYBKpFZI1lVyXe79pnq4qJHN16DGp_QEz6dvw)

