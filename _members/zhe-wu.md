---
name: Zhe (Tim) Wu
image: images/zhe.jpg
role: postdoc
affiliation: Siemens Healthineers
description: MRI Collaboration Scientist
group: alum
links: 
  google-scholar: NR-5WkIAAAAJ&hl=en
aliases:
  - Zhe Wu
  - Tim Wu
  - Z. Wu
  - T. Wu
  - Z Wu
  - T Wu
---

Zhe Wu (Tim) is an MRI Collaboration Scientist at Siemens Healthineers, working closely with BRAIN-TO group.

Before joining Siemens Healthineers, Tim was a Postdoctoral Fellow at Krembil Research Institute of the University Health Network (UHN). His Ph.D. project was on fast MR quantitative myelin water imaging. In 2018, after obtaining his Ph.D. degree of Biomedical Engineering from Zhejiang University in China, he worked as a Postdoctoral Researcher at the Montreal Neurological Institute and Hospital (MNI, or the Neuro) of McGill University in Montréal, Canada. In June 2019, he moved to the UHN and joined Dr. Kâmil Uludağ’s group. Dr. Wu is a specialist in MR sequence programming and image reconstruction, with experience on both GE EPIC system and Siemens IDEA platform. Dr. Wu has published three journal peer-reviewed paper as the first or second author and more than ten conference papers, and acted as a reviewer for top MR imaging journals.

**Motion estimation and correction for fast MR imaging methods.**
MRI scanning is sensitive to subject motion due to lengthy data acquisition, which is longer than most types of physiological movement cycles. In order to reduce scanning time and impact from motion, parallel imaging methods have been introduced and applied in clinical applications. For example, the recently introduced wave-CAIPI achieves significantly lower g-factor penalty to image signal-to-noise ratio (SNR) than the traditional SENSE and GRAPPA methods. This method is capable to achieve a high acceleration factor and reduce the scan time of the whole-brain anatomical scan with a sub-millimeter resolution within 1 minute. Even though the scan time has been significantly shortened, significant motion-related image degradation using wave-CAIPI acquisition can persist, for example due to short sudden movement, in particular in the readout direction. This research is focusing on investigating the possibility of using joint optimization to estimate and correct motion for accelerated 3D wave-CAIPI acquisition.

**Gradient imperfection estimation and its application on high-resolution spiral diffusion imaging**
In MRI scanning, the actual k-space trajectory applied during the MRI experiment can differ from the nominal trajectory due to hardware imperfections, resulting in image artifacts such as ghosting, blurring or geometric distortion. This problem is exacerbated in many non-Cartesian trajectories, such as spirals, because these fast imaging protocols place high demands on the gradient hardware of the MRI system. Accurate characterization of the system hardware is necessary and can be used for k-space trajectory correction, for example via a gradient impulse response function (GIRF). We developed the open-source [GIRFReco.jl](https://github.com/BRAIN-TO/GIRFReco.jl) reconstruction pipeline, which provides a single ecosystem implementation of this state-of-the-art approach to non-Cartesian MRI in the programming language Julia. It integrates system characterization information via GIRF correction for accurate representation of the encoding fields, relevant calibration data (coil sensitivity and static off-resonance maps) and iterative parallel imaging reconstruction for non-Cartesian k-space sampling patterns, including spiral trajectories.

