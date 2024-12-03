---
layout: post
title: NMR Signal Prediction (2024)
description: Nuclear Magnetic Resonance Spectroscopy Signal Prediction with Two Level GNNs 
image: /assets/images/NMR.png
---


Nuclear Magnetic Resonance Spectroscopy Signal Prediction with Two Level GNNs 
============

Background
------------
 NMR(Nuclear Magnetic Resonance) is the primary method used to estimate the properties of unknown molecules, and NMR machines are now one of the most commonly used instruments in organic chemistry laboratories. NMR spectroscopy takes advantage of the fact that the nuclear magnetic moment of each atom, which is the specific frequency of electromagnetic waves that it absorbs and emits when exposed to an external magnetic field, varies slightly depending on the environment around the atom. This information can then be used to reconstruct the environment around the atom, ultimately revealing the molecule of interest. 
![NMR image](https://soysilver.github.io/soysilvery/assets/images/NMR.png "NMR image of bipheny")

 NMR is divided into 1H NMR and 13C NMR depending on the type of target atom that is the center of the reconstruction. 1H NMR uses the chemical mobility of a hydrogen nucleus, or one lone proton, to determine the number of hydrogen atoms in a molecule, how they are bonded, and their ionization state. It is a common method for determining the structure of organic matter because the major atoms in organic compounds, such as carbon and oxygen, bond with the most common and lightest form of 1H hydrogen to form an octet of electrons. 13C NMR analyzes the chemical shifts of the carbon nucleus, which is composed of six protons and seven neutrons. Since the definition of an organic compound is a compound with a carbon atom as its backbone, 13C NMR is often used to determine the structure of complex molecules. 1H NMR has the advantage of high sensitivity and relatively quick results with a small sample volume. In contrast, 13C NMR is less sensitive and requires a large amount of sample, but it is relatively stable and accurate.

Motivation
------------
This project was conducted as part of ***Ewha Womans University's 17th Challenge Semester Program***, which allows undergraduate students to pursue projects of their choice. The project is based on ***Xing Ai's paper [Two-Level Graph Neural Network (TL-GNN)](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9714153),*** published in 2022.  They worked on enhancing the feature extraction capabilities of GNNs by focusing on counting the number of occurrences of different subgraphs within the graph structure, which we found impressive and wanted to use for NMR signal prediction. 

The approach of using partial graphs can be useful for recognizing and analyzing these specific chemical patterns within a molecule. Each functional group can be represented as a partial graph by itself, which can help predict chemical properties through structural comparisons between molecules with the same or similar functional groups.

![functional groups](https://soysilver.github.io/soysilvery/assets/images/funcGroup.gif "functional groups")
##### photo ref: James Ashenhurst, "Meet the (Most Important) Functional Groups", Master Organic Chemistry

Noting the advantages of these partial graphs in chemistry, we hypothesized that training on TL-GNNs would improve performance in using partial graphs.


Results  & feedback
------------
Experimental results showed that training with an epoch size of 10 resulted in a **Mean Absolute Error (MAE) of 46.588057388595445, which is relatively high compared to other NMR errors**. Therefore, we plan to re-experiment with the following feedback. 
  * Improve partial graph logic: Modify the current method of generating partial graphs, which only considers the number of nodes, to generate partial graphs that consider a sample of functional groups in organisms.
  * Secure learning resources: Secure resources that can be accessed continuously for longer learning time.
