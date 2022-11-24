Docker image for Pavian GxIT
============================

# Pavian

Pavian is a interactive browser application for analyzing and visualization metagenomics classification results from classifiers such as
Kraken, KrakenUniq, Kraken 2, Centrifuge and MetaPhlAn. Pavian also provides an alignment viewer for validation of matches to a particular genome.

For more information look at the publication at https://doi.org/10.1093/bioinformatics/btz715

Pavian: interactive analysis of metagenomics data for microbiome studies and pathogen identification. FP Breitwieser, SL Salzberg - Bioinformatics, 2020

Thank you for citing the publication if Pavian helps in your research :).

## Supported formats

pavian natively supports the Kraken and MetaPhlAn-style report formats. In extension, you can use Centrifuge results by running `centrifuge-kreport` on Centrifuge output files, and Kaiju results by running `kraken-report` on Kaiju output files.

# Docker image for GxIT

Based on:

- https://github.com/65MO/Galaxy-E/tree/master/GIE
- https://github.com/fbreitwieser/pavian/tree/master/inst/docker