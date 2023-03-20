# Establishing best practice guidelines for imaging-based spatially resolved transcriptomics data

> The German Network for Bioinformatics Infrastructure (deNBI) organised a week-long biohackathon consisting of many subgroups and according major projects. I registered for the SpatialHackaton project which was lead by Naveed Ishaque.
The project I personally lead was about exploring the new Stereo-seq spatial technology and evaluating it's suitability for the integration into the TXsim pipeline.

1. Nuaveed Ishaque ([]Naveed.ishaque@bih-charite.de), Berlin Institute of Health at the Charité, Germany
2. Co-lead: Brian Long ([]brianl@alleninstitute.org), Allen Institute for Brain Science, USA
3. Co-lead: Louis Kuemmerle, ([]louis.kuemmerle@helmholtz-muenchen.de Helmholtz Center Munich, Germany

[Hackathon github](https://spatialhackathon.github.io)

# Subproject: Exploring Stereo-seq for TXsim integration

> Aim of the project was to analyse the Stereo-seq technology for integratino into the `TXsim` pipeline.
> In short, we were able to load in the data, format it to AnnData, apply watershed segmentation and do a typical single-cell downstream analysis of the measured spots.

Team members:
- Ian (Leader)
- Shashwat Sahay
- Lotte Polaris

### Dataset information
||  |
| ----------------- | ---------------------------------------                              |
| Sample ID         | SS200000135TL_D1.cellbin.gem                                         |
| Source            | [Stereopy Github](https://github.com/BGIResearch/stereopy)          |
| Files             | [BGIResearch_Pan-Genomics](https://pan.genomics.cn/ucdisk/s/BvIrye) |
| Technology        | Stereo-seq                                                          |
| Organism           | Mus musculus                                                        |
| Organ             | Brain, hemibrain - coronal section                                                              |
| Added by          | Ian Dirk Fichtner                                                   |
| Added on          | 2022.12.14                                                          |

- Assumption: dataset comes from Chen-2022 paper
- Officially available data in raw sequence read format
- Lotte Polaris provided with a link to preprocessed data

### Conclusions:

- Stereo-seq is suitable for integration into the TXsim pipeline
  - It promises transcriptome-wide coverage and sub-cellular resolution
  - Further evaluation is needed
    - Compare with other sub-cellular spatial technologies
    - Segmentation comparisons
- Challenges: only DAPI channel availability limits the segmentation options
