# Establishing best practice guidelines for imaging-based spatially resolved transcriptomics data

The German Network for Bioinformatics Infrastructure (deNBI) organised a week-long biohackathon consisting of many subgroups and according major projects. I registered for the SpatialHackaton project whih was lead by Naveed Ishaque.
The project I personally lead was about <mark style="background: #FFF3A3A6;">exploring the new Stereo-seq spatial technology and evaluating it's suitability for the integration into the `TXsim` pipeline.</mark>

[Main website](https://spatialhackathon.github.io/)

Team members:
1. Ian (Leader)
2. Shashwat Sahay
3. Lotte Polaris (only gave some indications)

In short, we were able to read in the data, format it to `AnnData`, apply watershed segmentation and do a typical single-cell downstream analysis on the measured spots.
 
Full disclosure, Shashwat did the sc-analysis part and I don't know why he did it on the spot-level since I would have grouped the spots and their expression by the segmentation mast, achieving-pseudo cell profiles, and then would have applied the single-cell analysis.

Conclusions:
 - Stereo-seq is suitable for integration into the `TXsim` pipeline
 	- It promises transcriptome-wide coverage and sub-cellular resolution
 	- Further evaluation is needed
 		- Compare with other sub-cellular spatial technologies
 		- Segmentation comparisons
 - Challenges: only DAPI channel availability limits the segmentation options
