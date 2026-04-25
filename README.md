# GenerativeNeurosci_ML-TrDic

## Transformer + Dice Loss Framework for Bidirectional In Vitro–In Vivo Neural Spike-Train Generation

This repository provides code and supporting files for reproducing and extending the analyses reported in:

**Shimono, M. (2026). _In Vitro to In Vivo: Bidirectional and High-Precision Generation of In Vitro and In Vivo Neuronal Spike Data_. Algorithms, 19(4), 305. https://doi.org/10.3390/a19040305**

## Overview

This repository implements a Transformer-based generative framework for sparse multineuronal spike-train data.

The main goal is to evaluate whether spontaneous population activity recorded **in vitro** can be transformed into **in vivo-like** neural activity, and whether **in vivo** neural activity can likewise be transformed into **in vitro-like** activity.

This problem is important because in vitro and in vivo recordings are obtained under very different experimental conditions, and there is usually no one-to-one correspondence between neurons across independent experiments. Instead of assuming matched neurons, this project formulates the problem as a **time-resolved, bidirectional neural-domain transfer task between unpaired population spike trains**.

The method uses an autoregressive Transformer model together with Dice loss to improve learning from extremely sparse binary spike events. The evaluation includes ROC-AUC, Precision–Recall curves, and PR-AUC / average precision, which are especially important for sparse neural event prediction.

## Key Concepts

- Generative neuroscience
- Computational neuroscience
- NeuroAI
- Neural spike-train generation
- Spike-train prediction
- Sparse binary time-series modeling
- Multineuronal population activity
- In vitro to in vivo neural-domain transfer
- In vivo to in vitro neural-domain transfer
- Bidirectional neural-domain transfer
- Autoregressive Transformer
- Dice loss for sparse spike events
- ROC-AUC and PR-AUC evaluation
- Benchmarking neural dynamics across experimental preparations
- Translational neuroscience
- 3Rs-oriented computational modeling

## What This Repository Is For

This repository is intended for researchers who want to:

1. Reproduce the Transformer + Dice loss analyses described in the paper.
2. Study bidirectional generation between in vitro and in vivo multineuronal spike-train data.
3. Evaluate cross-domain transfer of spontaneous neural population activity.
4. Use this framework as a benchmark for neural-domain transfer.
5. Adapt or modify the code for other sparse neural event datasets.
6. Compare other models against this Transformer + Dice loss framework.
7. Extend the analysis toward generative neuroscience, neural foundation models, translational neuroscience, or computational replacement-oriented approaches.

## Main Script

The main analysis script is:

`test_a2b_binary_step4_double_loop_v11_dictloss_invitromix2invivo_share.py`

This script performs the main bidirectional generation analysis using sparse binary spike-train data.

## How to Run

1. Download all files in this repository.

2. Save all downloaded files in the same project folder.

3. Move into the following directory:

   `spike_tnb_200428`

4. Run the main script:

   `python test_a2b_binary_step4_double_loop_v11_dictloss_invitromix2invivo_share.py`

5. Before running the script, please check and modify the data paths according to your local environment.

Because the original analyses were performed with specific local directory structures, path adjustment is usually necessary when reproducing the analysis on another machine.

## Data and Path Notes

The code assumes sparse binary multineuronal spike-train data arranged in the expected project directory structure.

If the script cannot find the input files, please first check:

- the root data directory
- the location of the `spike_tnb_200428` folder
- the paths to in vitro datasets
- the paths to in vivo datasets
- the output directory for generated results
- operating-system-specific path separators on Windows, macOS, or Linux

If you adapt this code to a different dataset, please make sure that the input data format is consistent with the binary spike-train representation expected by the script.

## Expected Analysis Outputs

Depending on the local configuration, the analysis may generate outputs related to:

- generated / predicted spike-train data
- ground-truth spike-train data
- ROC curves
- Precision–Recall curves
- ROC-AUC values
- PR-AUC / average precision values
- training and validation performance summaries
- cross-domain generation results for in vitro-to-in vivo conditions
- cross-domain generation results for in vivo-to-in vitro conditions

## Citation Policy

If you use this repository in any way that contributes to a publication, preprint, thesis, presentation, software tool, benchmark comparison, dataset analysis, or derivative codebase, please cite the paper below.

Please cite the paper if you:

- use the original code
- modify or extend the code
- reuse part of the code in another project
- use this repository as a benchmark
- compare another model against this framework
- use the dataset structure or preprocessing procedure
- use the evaluation procedure, including ROC-AUC, PR-AUC, or average precision analysis
- build upon the Transformer + Dice loss framework
- build upon the idea of bidirectional in vitro–in vivo neural-domain transfer
- use this work as a reference for sparse spike-train generation, neural-domain transfer, or generative neuroscience

Recommended citation:

**Shimono, M. (2026). _In Vitro to In Vivo: Bidirectional and High-Precision Generation of In Vitro and In Vivo Neuronal Spike Data_. Algorithms, 19(4), 305. https://doi.org/10.3390/a19040305**

Preprint version:

**Shimono, M. (2025). _In vitro 2 In vivo: Bidirectional and High-Precision Generation of In Vitro and In Vivo Neuronal Spike Data_. bioRxiv. https://doi.org/10.1101/2025.03.26.645366**

## Short Citation Request

If you use this code, benchmark, dataset structure, evaluation procedure, or any modified version of this repository, please cite:

**Shimono, M. (2026). _In Vitro to In Vivo: Bidirectional and High-Precision Generation of In Vitro and In Vivo Neuronal Spike Data_. Algorithms, 19(4), 305. https://doi.org/10.3390/a19040305**

## Suggested Citation Sentence

This repository implements a Transformer + Dice loss framework for bidirectional neural-domain transfer between unpaired in vitro and in vivo multineuronal spike trains.

## Contact

For detailed questions about the code, data format, reproduction procedure, or possible extensions, please contact:

**shimonomlab@gmail.com**
