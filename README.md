
# CMML_FAIR
**Roll number**: 2135  
This repository contains the code used for drafting my CMML report.

## Attempts to Set Up Docker from Ersilia's Repository
- [Ersilia Repository 1](https://github.com/ersilia-os/eos9f6t)
- [Ersilia Repository 2](https://github.com/ersilia-os/eos8fth)

To build the Docker container locally:
```
docker build -t model .
```

## Original Authors' Repository (Kc et al., 2021)
- [Redial-2020 Repository](https://github.com/sirimullalab/redial-2020)

### Setup Instructions
To set up the environment using Docker, run the following commands:

```
docker pull sirimullalab/redial-2020:latest
docker run -p 6000:5000 sirimullalab/redial-2020:latest
```

### Example Data: Remdesivir

SMILES notation for Remdesivir:

```
CCC(COC(=O)[C@@H](N[P@@](=O)(Oc1ccccc1)OC[C@H]1O[C@@]([C@@H]([C@@H]1O)O)(C#N)c1ccc2n1ncnc2N)C)CC
```

### Prediction Using Remdesivir as an Example
To predict using Remdesivir, use the following `curl` command:
```
curl -F smiles='CCC(COC(=O)[C@@H](N[P@@](=O)(Oc1ccccc1)OC[C@H]1O[C@@]([C@@H]([C@@H]1O)O)(C#N)c1ccc2n1ncnc2N)C)CC' 
```

