# Introduction
We employed a machine learning framework called EcoTyper to identify the fundamental cell states and cellular ecosystems (ecotypes) that make up soft tissue sarcomas and validated their relevance using single-cell RNA sequencing and spatial transcriptomics. We have shown that these cell states and ecotypes are prognostic of patient outcomes and predict response to immune checkpoint inhibition. The files and directories in this repository and the instructions below will allow users to use the EcoTyper framework to recover these sarcoma cell states and ecotypes from bulk gene expression, single-cell RNA sequencing, and spatial transcriptomics data.

# Setup
Users should start by downloading the latest version of the EcoTyper source code from the [EcoTyper GitHub repository](https://github.com/digitalcytometry/ecotyper):

```
git clone https://github.com/digitalcytometry/ecotyper
cd ecotyper
```

Next, download the "SoftTissueSarcoma" folder from this repository into the "EcoTyper" folder within the "ecotyper" directory:

```
cd EcoTyper
git init
git remote add -f origin https://github.com/ejmoding/sarcomaecotyper
git config core.sparseCheckout true
echo 'SoftTissueSarcoma' >> .git/info/sparse-checkout
git pull origin master
cd ..
```

Finally, follow the instructions for recovery of cell states and ecotypes in bulk expression, single cell RNA sequencing, or spatial transcriptomics data within the [EcoTyper GitHub repository](https://github.com/digitalcytometry/ecotyper).
