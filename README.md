[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.nm000119-blue)](https://doi.org/10.82901/nemar.nm000119)

# SSVEP MAMEM 1 dataset

SSVEP MAMEM 1 dataset.

## Dataset Overview

- **Code**: MAMEM1
- **Paradigm**: ssvep
- **DOI**: 10.48550/arXiv.1602.00904
- **Subjects**: 11
- **Sessions per subject**: 1
- **Events**: 6.66=1, 7.50=2, 8.57=3, 10.00=4, 12.00=5
- **Trial interval**: [1, 4] s
- **File format**: MATLAB .mat

## Acquisition

- **Sampling rate**: 250.0 Hz
- **Number of channels**: 256
- **Channel types**: eeg=256
- **Channel names**: E1, E10, E100, E101, E102, E103, E104, E105, E106, E107, E108, E109, E11, E110, E111, E112, E113, E114, E115, E116, E117, E118, E119, E12, E120, E121, E122, E123, E124, E125, E126, E127, E128, E129, E13, E130, E131, E132, E133, E134, E135, E136, E137, E138, E139, E14, E140, E141, E142, E143, E144, E145, E146, E147, E148, E149, E15, E150, E151, E152, E153, E154, E155, E156, E157, E158, E159, E16, E160, E161, E162, E163, E164, E165, E166, E167, E168, E169, E17, E170, E171, E172, E173, E174, E175, E176, E177, E178, E179, E18, E180, E181, E182, E183, E184, E185, E186, E187, E188, E189, E19, E190, E191, E192, E193, E194, E195, E196, E197, E198, E199, E2, E20, E200, E201, E202, E203, E204, E205, E206, E207, E208, E209, E21, E210, E211, E212, E213, E214, E215, E216, E217, E218, E219, E22, E220, E221, E222, E223, E224, E225, E226, E227, E228, E229, E23, E230, E231, E232, E233, E234, E235, E236, E237, E238, E239, E24, E240, E241, E242, E243, E244, E245, E246, E247, E248, E249, E25, E250, E251, E252, E253, E254, E255, E256, E26, E27, E28, E29, E3, E30, E31, E32, E33, E34, E35, E36, E37, E38, E39, E4, E40, E41, E42, E43, E44, E45, E46, E47, E48, E49, E5, E50, E51, E52, E53, E54, E55, E56, E57, E58, E59, E6, E60, E61, E62, E63, E64, E65, E66, E67, E68, E69, E7, E70, E71, E72, E73, E74, E75, E76, E77, E78, E79, E8, E80, E81, E82, E83, E84, E85, E86, E87, E88, E89, E9, E90, E91, E92, E93, E94, E95, E96, E97, E98, E99
- **Montage**: GSN-HydroCel-256
- **Hardware**: EGI 300 Geodesic EEG System (GES 300)
- **Line frequency**: 50.0 Hz
- **Impedance threshold**: 80.0 kOhm
- **Cap manufacturer**: EGI
- **Cap model**: HydroCel Geodesic Sensor Net (HCGSN)

## Participants

- **Number of subjects**: 11
- **Health status**: healthy
- **Clinical population**: able-bodied subjects without any known neuro-muscular or mental disorders
- **Age**: min=24, max=39
- **Gender distribution**: male=8, female=3
- **Handedness**: {'right': 10, 'left': 1}
- **Species**: human

## Experimental Protocol

- **Paradigm**: ssvep
- **Number of classes**: 5
- **Class labels**: 6.66, 7.50, 8.57, 10.00, 12.00
- **Trial duration**: 5.0 s
- **Study design**: Subjects focus attention on a single violet box flickering at different frequencies (6.66, 7.50, 8.57, 10.00, 12.00 Hz) presented sequentially. Each frequency is presented for 5 seconds (trial) followed by 5 seconds rest, repeated 3 times per frequency, with 30 seconds rest between different frequencies.
- **Feedback type**: none
- **Stimulus type**: flickering box
- **Stimulus modalities**: visual
- **Primary modality**: visual
- **Synchronicity**: synchronous
- **Mode**: offline
- **Instructions**: Subjects were instructed to focus attention on the flickering box, limit movements, and avoid swallowing or blinking during visual stimulation
- **Stimulus presentation**: SoftwareName=Microsoft Visual Studio 2010 with OpenGL, monitor=22 inch LCD monitor, refresh_rate=60 Hz, resolution=1680x1080 pixels

## HED Event Annotations

Schema: HED 8.4.0 | Browse: https://www.hedtags.org/hed-schema-browser

```
  6.66
    ├─ Sensory-event
    ├─ Experimental-stimulus
    ├─ Visual-presentation
    └─ Label/6_66

  7.50
    ├─ Sensory-event
    ├─ Experimental-stimulus
    ├─ Visual-presentation
    └─ Label/7_50

  8.57
    ├─ Sensory-event
    ├─ Experimental-stimulus
    ├─ Visual-presentation
    └─ Label/8_57

  10.00
    ├─ Sensory-event
    ├─ Experimental-stimulus
    ├─ Visual-presentation
    └─ Label/10_00

  12.00
    ├─ Sensory-event
    ├─ Experimental-stimulus
    ├─ Visual-presentation
    └─ Label/12_00

```
## Paradigm-Specific Parameters

- **Detected paradigm**: ssvep
- **Stimulus frequencies**: [6.66, 7.5, 8.57, 10.0, 12.0] Hz
- **Number of targets**: 5
- **Number of repetitions**: 3

## Data Structure

- **Trials**: 1104
- **Trials context**: Total 1104 trials across all subjects. Each session includes 23 trials (8 adaptation + 15 main). S001: 3 sessions, S003 and S004: 4 sessions, others: 5 sessions. Some sessions excluded due to technical issues.

## Preprocessing

- **Data state**: raw
- **Preprocessing applied**: False

## Signal Processing

- **Classifiers**: LDA, SVM, Random Forest, kNN, Naive Bayes, CCA, AdaBoost, Decision Trees
- **Feature extraction**: Periodogram, Welch Spectrum, Goertzel algorithm, Yule-AR Spectrum, FFT, PSD, Discrete Wavelet Transform
- **Frequency bands**: analyzed=[5.0, 48.0] Hz
- **Spatial filters**: CAR, CSP, Minimum Energy

## Cross-Validation

- **Method**: leave-one-subject-out
- **Evaluation type**: cross_subject

## Performance (Original Study)

- **Default Accuracy**: 72.47
- **Optimal Accuracy**: 79.47

## BCI Application

- **Applications**: communication
- **Environment**: laboratory
- **Online feedback**: False

## Tags

- **Pathology**: Healthy
- **Modality**: Visual
- **Type**: Perception

## Documentation

- **Description**: Comparative evaluation of state-of-the-art algorithms for SSVEP-based BCIs
- **DOI**: 10.6084/m9.figshare.2068677.v1
- **Associated paper DOI**: 10.48550/arXiv.1602.00904
- **License**: ODC-By-1.0
- **Investigators**: Vangelis P. Oikonomou, Georgios Liaros, Kostantinos Georgiadis, Elisavet Chatzilari, Katerina Adam, Spiros Nikolopoulos, Ioannis Kompatsiaris
- **Senior author**: Ioannis Kompatsiaris
- **Institution**: Centre for Research and Technology Hellas (CERTH)
- **Country**: GR
- **Repository**: Figshare
- **Data URL**: https://dx.doi.org/10.6084/m9.figshare.2068677.v1
- **Publication year**: 2016
- **Funding**: H2020-ICT-2014-644780
- **Ethics approval**: Centre for Research and Technology Hellas ethics committee, dated 3/7/2015, grant H2020-ICT-2014-644780
- **Keywords**: SSVEP, BCI, EEG, brain-computer interface, comparative evaluation, state-of-the-art algorithms

## Abstract

Brain-computer interfaces (BCIs) have been gaining momentum in making human-computer interaction more natural, especially for people with neuro-muscular disabilities. This report focuses on SSVEP-based BCIs and performs a comparative evaluation of the most promising algorithms. A dataset of 256-channel EEG signals from 11 subjects is provided, along with a processing toolbox for reproducing results and supporting further experimentation.

## Methodology

Empirical approach where each signal processing parameter (filtering, artifact removal, feature extraction, feature selection, classification) is studied independently by keeping all other parameters fixed. Leave-one-subject-out cross-validation used to evaluate system without subject-specific training. Multiple algorithms compared for each processing stage to obtain state-of-the-art baseline.

## References

Oikonomou, V. P., Liaros, G., Georgiadis, K., Chatzilari, E., Adam, K., Nikolopoulos, S., & Kompatsiaris, I. (2016). Comparative evaluation of state-of-the-art algorithms for SSVEP-based BCIs. arXiv preprint arXiv:1602.00904.

MAMEM Steady State Visually Evoked Potential EEG Database `<https://archive.physionet.org/physiobank/database/mssvepdb/>`_

S. Nikolopoulos, 2016, DataAcquisitionDetails.pdf `<https://figshare.com/articles/dataset/MAMEM_EEG_SSVEP_Dataset_I_256_channels_11_subjects_5_frequencies_/2068677?file=3793738>`_
Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R., Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Hochenberger, R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A. and Jas, M. (2019). MNE-BIDS: Organizing electrophysiological data into the BIDS format and facilitating their analysis. Journal of Open Source Software 4: (1896). https://doi.org/10.21105/joss.01896

Pernet, C. R., Appelhoff, S., Gorgolewski, K. J., Flandin, G., Phillips, C., Delorme, A., Oostenveld, R. (2019). EEG-BIDS, an extension to the brain imaging data structure for electroencephalography. Scientific Data, 6, 103. https://doi.org/10.1038/s41597-019-0104-8

---
Generated by MOABB 1.4.3 (Mother of All BCI Benchmarks)
https://github.com/NeuroTechX/moabb
