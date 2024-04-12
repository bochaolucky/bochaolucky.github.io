---
layout: page
title: CAL
permalink: /datasets/cal
description: EEG database for Confusion Analysis in Learning
importance: 1
category: Datasets
---

## Abstract

**Objective:** Confusion is the primary epistemic emotion in the learning process, influencing students’ engagement and whether they become frustrated or bored. However, research on confusion in learning is still in its early stages, and there is a need to better understand how to recognize it and what EEG signals indicate its occurrence. The present work investigates confusion during reasoning learning using EEG, and aims to fill this gap with a multidisciplinary approach combining educational psychology, neuroscience and computer science.

**Approach:** First, we design an experiment to actively and accurately induce confusion in reasoning. Second, we propose a subjective and objective joint labeling technique to address the label noise issue. Third, to confirm that the confused state can be distinguished from the non-confused state, we compare and analyze the mean band power of confused and unconfused states across five typical bands. Finally, we present an EEG database for confusion analysis, together with benchmark results from conventional (Naive Bayes, SVM, Random Forest, and ANN) and end-to-end (LSTM, ResNet, and EEGNet) machine learning methods.

**Main results:** Findings revealed: 1. Significant differences in the power of delta, theta, alpha, beta and lower gamma between confused and non-confused conditions; 2. A higher attentional and cognitive load when participants were confused; and 3. The Random Forest algorithm with time-domain features achieved a high accuracy/F1 score (88.06%/0.88 for the subject-dependent approach and 84.43%/0.84 for the subject-independent approach) in the binary classification of the confused and non-confused states.

**Significance:** The study advances our understanding of confusion and provides practical insights for recognizing and analyzing it in the learning process. It extends existing theories on the differences between confused and nonconfused states during learning and contributes to the cognitive-affective model. The research enables researchers, educators, and practitioners to monitor confusion, develop adaptive systems, and test recognition approaches.

### Experiment Setup

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/fig3.jpg" title="fig3" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The experiment system comprised three parts: EEG collector, confusion inducer, and data storage, as shown in Figure 3. We employed OpenBCI as the EEG collector in this work, due to its wearable and high-quality bio-sensing hardware for brain-computer interfacing. It has eight channels (Fp1, Fp2, C3, C4, T5, T6, O1, O2) and a good sampling rate (250 Hz), providing the possibility of large-scale collection of EEG signals in learning study and application. We used one desktop to induce confused states and a laptop to connect with the EEG collector and store the data. The E-prime, a software for behavioral and psychological research, was employed to generate the stimuli and interaction. It also sent trigger signals for segmenting trials. We redeveloped the firmware and software of the OpenBCI Cyton Board, making it receive the trigger signals from DB25. When storing the data, the EEG waves were real-time sync visualized. This visualization could help testers monitor the experiment.

### Subjects and Experiment Protocol

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/cal_experiment_process.png" title="cal_experiment_process" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

A total of 25 subjects participated in this experiment. We obtained 23 subjects’ data because the unexpected equipment problem made failed collection for two persons. The ages were between 20 and 47 (Mean = 24.48, SD = 6.36); the male to female ratio is roughly half to half (12:11). The education backgrounds covered middle school, undergraduate, master, and doctoral degrees, and the major included computer science, microelectronics, bioengineering, and British and American literature. All participants were in good health and had normal vision without any history of brain injury or mental illness.

The experiment testers explained the experiment’s purpose, process, and precautions. After signed an ultimate consent form, subjects started to perform the tasks. As shown in Figure, we first presented the manipulation instruction. When subjects were ready, they watched ten scene pictures, each of which lasted 10 seconds. Next to this, they viewed and performed 48 tests, each of which lasted a maximum of 15 seconds. The participants evaluated their own level of confusion for each test item at the end of the trials.

### Dataset Summary

The Dataset consists 23 subject’ data(failed subject 1 and subject 6), and each subject has 49 files. There are five labels, confused,non-confused,guess,think-right and rest. And the data labeled undefined is wasted. The data sample rate is 250Hz. The EEG cap according to the international 10 - 20 system for 8 channels is shown below: `“Fp1”, “Fp2”, “C3”, “C4”, “T5”, “T6”, “O1”, “O2”`

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.html path="assets/img/10-20system.png" title="10-20system" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## How to use

If you are interested in using this dataset, you will have to print, sign and scan an EULA (End User License Agreement) and upload it via the dataset request form. We will then supply you with a username and password to download the data.

## Publications

Publications include not only papers, but also presentations for conferences or educational purposes.All documents and papers that report on research that uses the CAL dataset will acknowledge this by

citing the following paper:

> T. Xu, J. Wang, G. Zhang, L. Zhang, and Y. Zhou, “Confused or not: decoding brain activity and recognizing confusion in reasoning learning using EEG,” J. Neural Eng., vol. 20, no. 2, p. 026018, Mar. 2023, doi: [10.1088/1741-2552/acbfe0](https://doi.org/10.1088/1741-2552/acbfe0).

## Credits

First and foremost we’d like to thank the all(25) participants in this study for having the patience and goodwill to let us record their data. This dataset was collected by: **Intelligent Interaction Laboratory @ Northwestern Polytechnical University**

## Dataset access

To gain access to the dataset and download the files on this page, please download the license agreement below. The license agreement should be printed, signed, scanned and returned via email to <a href="mailto:xutao@nwpu.edu.cn">xutao@nwpu.edu.cn</a> with the subject of **“CAL account request”**. Upon receipt, a username, a password and a download link will be sent to download the data files below.

[The License Agreement](/assets/pdf/cal_license.pdf)

<!-- 引入不蒜子计数 -->
<script async src="//busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script>

<center>
        Views count:<span id="busuanzi_value_site_pv"><i class="fa fa-spinner fa-spin"></i></span>👀 | Number of visitors:<span id="busuanzi_value_site_uv"><i class="fa fa-spinner fa-spin"></i></span>👦
</center>
