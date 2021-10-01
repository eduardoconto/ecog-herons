# Project Proposal
## Distinguishing motor execution from motor imagery

**Keywords:** motor execution, motor imagery, ECoG, ECoG decoding, event related
potential, power spectrum density, hand control, tongue control, motor cortex,
Miller 2019, efficient real-time decoding.

We propose to understand the neurological differences between actual movement
and motor imagery. Furthermore, we would like to decode signals from the motor
cortex to predict movement onset. To achieve this, we will leverage the ECoG
dataset from Miller 2019 on motor imagery.

Our research will focus in two questions:
1. How is motor execution different from motor imagery?
2. Can we decode hand movement and tongue movement?

More precisely, for (1), we ask whether there exists a model that can
differentiate between motor execution and motor imagery? Does it generalize
across the two studied movement tasks (tongue and hand)? Our initial hypothesis
is that motor execution should active a larger number of areas in the brain,
since it has to (a) decide on precise movement to execute and (b) execute it by
recruiting the spinal cord. Is this hypothesis backed by the data? In general,
what are the brain mechanisms in play here?

For (2), our goal is to decode the hand movement and tongue movement with an
efficient model. Can we achieve a high decoding accuracy (above 90%)? What is
the minimum number of parameters required for such decoding (best trade-off
number of parameters vs efficiency)? Can we build an efficient decoding
algorithm suitable for a real-time usage? Can we predict the motor task prior to
its onset and, if so, by how much time?

We will attempt to tackle these questions by analysis the dataset:
preprocessing, extracting features (Power Spectrum Density, ERP, electrode
position) and building suitable models.

# Abstract
## Cross-session decoding accuracy: motor imagery vs. motor execution

Brain Computer Interfaces (BCI) aim to restore or augment human skills via efficient neuroprosthetic solutions. One common BCI paradigm is motor imagery decoding: a subject is instructed to imagine making a movement without actually executing it. However, few studies so far focused on motor execution. Hence, it is unknown whether decoding algorithms for motor imagery would have a similar accuracy on motor execution. On the other hand, prior research has shown that both motor imagery and execution have similar brain activation patterns. Therefore, we hypothesize that a model trained on motor imagery data would have similar performance on motor execution data. Here we evaluate a traditional BCI pipeline composed of filtering on the high-frequency band (76-100Hz), Principal Component Analysis (PCA) for dimensionality reduction and Support Vector Machine (SVM) for classification. We then evaluate the cross-section accuracy for each subject. We perform such analysis on the data from Miller, 2019, composed of electrocorticography (ECoG) recordings collected from eight patients. We aim to show that, if we train a decoding model on motor imagery data, then we can use it to decode motor execution data and obtain similar accuracy across these two experiments. This would allow us to conclude that, since accuracy is preserved, we can decode ECoG data for both motor execution and imagery tasks using the same model. This would also further validate previous studies showing that the brain activation for motor execution and imagery are similar. Future research should attempt to replicate these findings on other datasets and, in particular, on electroencephalogram (EEG) data.

# Presentation
[pdf](ecog-herons-presentation.pdf)

# Credits
Project members: [Anjali Agarwal](mailto:anjaliagrl8@gmail.com), [Eduardo de Conto](mailto:eduardoconto@gmail.com), [Gilbert Temgoua](mailto:gilbertemgoua@gmail.com), [Yigit Yargili](mailto:yigityargili99@gmail.com)

Mentor: Sarah Schoch

Project Teaching Assistant: Jonathan Coutinho

Teaching Assistant: Tuan-Duy Nguyen
