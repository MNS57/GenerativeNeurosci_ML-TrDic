# GenerativeNeurosci_ML-TrDic

This repository provides code and supporting files for reproducing the analyses in:

Shimono, M. (2026). In Vitro to In Vivo: Bidirectional and High-Precision Generation of In Vitro and In Vivo Neuronal Spike Data. Algorithms, 19(4), 305. https://doi.org/10.3390/a19040305

## Overview

This project implements a Transformer-based framework with Dice loss for bidirectional generation between unpaired in vitro and in vivo multineuronal spike-train data. The framework is designed to evaluate whether sparse population spike dynamics can be transferred across different experimental preparations, including in vitro slice recordings and in vivo recordings.

The main analysis script is:

test_a2b_binary_step4_double_loop_v11_dictloss_invitromix2invivo_share.py

## How to run

1. Download all files in this repository.
2. Place all downloaded files in the same project folder.
3. Move into the `spike_tnb_200428` directory.
4. Run the main script:

   python test_a2b_binary_step4_double_loop_v11_dictloss_invitromix2invivo_share.py

5. Depending on your local environment, please modify the data paths in the script before execution.

## Notes

The code was developed for sparse binary spike-train data and may require adjustment of file paths, dataset locations, and environment-specific settings before running on a different machine.

For detailed questions about the code, data structure, or reproduction procedure, please contact:

shimonomlab@gmail.com

## Citation

If you use this code, dataset structure, evaluation procedure, or benchmark concept, please cite:

Shimono, M. (2026). In Vitro to In Vivo: Bidirectional and High-Precision Generation of In Vitro and In Vivo Neuronal Spike Data. Algorithms, 19(4), 305. https://doi.org/10.3390/a19040305
