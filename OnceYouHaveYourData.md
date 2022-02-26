# ONCE YOU HAVE DATA

<!-- TOC -->

- [ONCE YOU HAVE DATA](#once-you-have-data)
  - [quality control](#quality-control)
  - [preprocessing](#preprocessing)
    - [Pipelines ( ??? )](#pipelines---)
    - [Artefact/Noise removal ( ??? )](#artefactnoise-removal---)
      - [PCA ( ??? )](#pca---)
      - [ICA ( ??? )](#ica---)
      - [ART ( ??? )](#art---)
      - [ART repair ( ??? )](#art-repair---)
      - [Physiological noise ( ??? )](#physiological-noise---)
      - [Motion](#motion)
  - [Analysis](#analysis)
    - [general linear model](#general-linear-model)
    - [Model selection ( ??? )](#model-selection---)
    - [Multivariate analysis ( ??? )](#multivariate-analysis---)
      - [R based ( ??? )](#r-based---)
    - [Resting state ( ??? )](#resting-state---)
    - [Diffusion weighted imaging](#diffusion-weighted-imaging)
    - [Statistical inferences and multiple comparison correction (MCP) ( ??? )](#statistical-inferences-and-multiple-comparison-correction-mcp---)
      - [Cluster based inference ( ??? )](#cluster-based-inference---)
      - [Family wise error (FWE) ( ??? )](#family-wise-error-fwe---)
      - [False discovery rate (FDR) ( ??? )](#false-discovery-rate-fdr---)
      - [Permutation tests ( ??? )](#permutation-tests---)
      - [SnPM ( ??? )](#snpm---)
      - [FSL PALM and Randomize( ??? )](#fsl-palm-and-randomize--)
      - [Freesurfer PALM ( ??? )](#freesurfer-palm---)
    - [Encoding models ( ??? )](#encoding-models---)
      - [Popeye](#popeye)
      - [SAMSRF](#samsrf)
  - [Robustness checks](#robustness-checks)
  - [Computational neuroscience](#computational-neuroscience)
    - [Free energy](#free-energy)
    - [Dynamic causal modelling](#dynamic-causal-modelling)
  - [Laminar and high-resolution MRI](#laminar-and-high-resolution-mri)
  - [Meta analysis ( ??? )](#meta-analysis---)

<!-- /TOC -->

## quality control

- [quality control on MRI and fMRI](https://practicalfmri.blogspot.com/2014/08/qa-for-fmri-part-3-facility-qa-what-to.html)
- [COBIDacq](https://practicalfmri.blogspot.com/2017/12/cobidacq.html)
- https://en.wikibooks.org/wiki/Neuroimaging_Data_Processing/Data_Quality
- [Neuroimaging quality control task force](https://crossinvalidation.com/2018/07/31/neuroimaging-quality-control-niqc-task-force-to-develop-protocols-tools-and-manuals/)
- [References for quality control](https://www.zotero.org/groups/2221093/niqc)

- [MRIQC](https://mriqc.readthedocs.io/en/stable/) MRI quality control. A BIDS
  app that runs a pipeline to assess the quality of your data.
- [the PCP Quality Assessment Protocol](https://github.com/BIDS-Apps/QAP) is
  another BIDS app based on the protocol of [the connectome project
  data}(http://preprocessed-connectomes-project.org/quality-assessment-protocol/)
- [Scripts for quality control of diffusion data](http://davidroalf.com/script_download/)
- https://github.com/memobc/memolab-fmri-qa
- [Qoala-t](https://github.com/Qoala-T) for QA for freesurfer segmentations also
  with an online [shinyapp](https://qoala-t.shinyapps.io/qoala-t_app/)
- [Visual QC](https://github.com/raamana/visualqc) developed by
  [Pradeep](https://twitter.com/raamana_).

OHBM 2019 session on quality control by Pradeep

## preprocessing

### Pipelines ( ??? )

There are some ready made pipeline as
[BIDS apps](http://bids-apps.neuroimaging.io/apps/) that already exist and have
been tested. Using them might save you time and make your results more
reproducible.

- [AFNI based](https://github.com/BIDS-Apps/afni_proc)
- [HCP Pipelines](https://github.com/BIDS-Apps/HCPPipelines): a set of tools
  (primarily, but not exclusively, shell scripts) for processing MRI images for
  the Human Connectome Project.
- [fMRIprep](https://fmriprep.readthedocs.io/en/stable/)
- [The NeuroImaging Analysis Kit](https://github.com/BIDS-Apps/niak): NIAK is a
  library of pipelines for the preprocessing and mining of large functional
  neuroimaging data.
- [Automatic Analysis](https://github.com/BIDS-Apps/aa): is a
  [pipeline system for neuroimaging](http://automaticanalysis.org/) written
  primarily in Matlab. It robustly supports recent versions of SPM, as well as
  selected functions from other software packages. The goal is to facilitate
  automatic, flexible, and replicable neuroimaging analyses through a
  comprehensive pipeline system.
- [nipypelines](https://github.com/BIDS-Apps/nipypelines)
- [Configurable Pipeline for the Analysis of Connectomes](https://github.com/BIDS-Apps/CPAC):
  C-PAC is a software for performing high-throughput preprocessing and analysis
  of functional connectomes data using high-performance computers.

There is also an [OPPNI](https://github.com/BIDS-Apps/oppni) for Optimization of
Preprocessing Pipelines for NeuroImaging.

### Artefact/Noise removal ( ??? )

[GLM denoise](http://kendrickkay.net/GLMdenoise/)

ART repair

ART

fmridenoise

#### PCA ( ??? )

#### ICA ( ??? )

#### ART ( ??? )

#### ART repair ( ??? )

https://cibsr.stanford.edu/tools/human-brain-project/artrepair-software.html

#### Physiological noise ( ??? )

http://technicalfmri.blogspot.com/2018/02/physiological-monitoring-and-recording.html?m=1

#### Motion

http://blogs.discovermagazine.com/neuroskeptic/2014/07/06/fmri-scanning-dead/
http://blogs.discovermagazine.com/neuroskeptic/2013/11/26/head-movement-bad-news-neuroscience/
http://blogs.discovermagazine.com/neuroskeptic/2012/08/07/brains-in-motion-are-bad-for-neuroscience/

## Analysis

### general linear model

- a FAQ [article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3896880/) on the
  GLM by Cyril Pernet with
  [matlab code](https://www.frontiersin.org/articles/file/downloadfile/58014_supplementary-materials_datasheets_1_zip/octet-stream/Data%20Sheet%201.ZIP/2/58014)
  to go through
- see the section on [percent signal change](#percent-signal-change) to better
  understand how to report results
- orthogonalization of regressors can be a bit hard to wrap your head aroudnd at
  first but Jeanette Mumford ( ??? ) has great
  [paper](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0126255)
  on the topic with a
  [jupyter notebook](http://nbviewer.jupyter.org/github/jmumford/orthogonalizaton_ipynb/blob/master/orthogonalization.ipynb).

SPM tool box for

### Model selection ( ??? )

[Analytical flexibility](http://blogs.discovermagazine.com/neuroskeptic/2012/06/30/false-positive-neuroscience/)
is a big
[problem in neuroimaging](http://blogs.discovermagazine.com/neuroskeptic/2012/10/14/more-on-false-positive-neuroimaging/)
most likely the source of a lot of false positive results.

If several analysis are attempted it can be good to have ways to decide amongst
them. There is bad way to do like the one described in the
[overfitting toolbox](https://www.researchgate.net/publication/319208937_The_Overfitting_Toolbox_TOT_Large-Scale_Search_in_Model_Space_for_Expected_Neuroimaging_Effects).

But there are better ways to do it:

- The [MACS](https://github.com/JoramSoch/MACS) SPM toolbox by
  [Joram Soch](https://twitter.com/JoramSoch)
- ( ??? )

### Multivariate analysis ( ??? )

http://blogs.discovermagazine.com/neuroskeptic/2014/06/21/fmri-mvpa-crack-neural-code/

https://distill.pub/2016/misread-tsne/

- [Jo Etzel](https://twitter.com/JosetAEtzel) has a great blog if you want to
  know more about multivariate analysis:
  [MVPA meandering](http://mvpa.blogspot.co.uk)

[Cross-validation : what, which and how?](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116075)
by [Pradeep Reedy Raamana](https://twitter.com/raamana_) at OHBM 2018 (30 min)

What can we say about weight maps from linear decoding models?
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116081

Neuroimaging toolboxes for representation similarity analysis (RSA), support
vector machine (SVM) and others...

#### R based ( ??? )

### Resting state ( ??? )

I know almost nothing about resting state but I have been told
[this site](http://rfmri.org/) is worth having a look at.

- [Course/Tutorials](http://rfmri.org/Course)
- Tools ( ??? )

fmridenoise neuropycon

### Diffusion weighted imaging

https://www.kaggle.com/chrisfilo/diffusion-weighted-imaging-dwi-analysis-with-dipy#

https://www.mrtrix.org/

### Statistical inferences and multiple comparison correction (MCP) ( ??? )

the salmon
http://neuroskeptic.blogspot.com/2009/09/fmri-gets-slap-in-face-with-dead-fish.html

imager's fallacy
http://blog.efpsa.org/2014/12/17/a-psychologists-guide-to-reading-a-neuroimaging-paper/

All Resolution Inference: Increasing Spatial Specificity of fMRI with Valid
Circular Inference
https://www.pathlms.com/ohbm/courses/8246/sections/12541/video_presentations/115959

http://blogs.discovermagazine.com/neuroskeptic/2011/09/11/neuroscience-fails-stats-101/

#### Cluster based inference ( ??? )

[Probabilistic Treshold-free Cluster Enhancement](https://spisakt.github.io/pTFCE/)
pTFCE (probabilistic TFCE) is a cluster-enahncement method to improve
detectability of neuroimaging signal. It performs topology-based belief boosting
by integrating cluster information into voxel-wise statistical inference.

#### Family wise error (FWE) ( ??? )

In case you do not remember how random field theory works to correct for
multiple comparison,
[check this](http://imaging.mrc-cbu.cam.ac.uk/imaging/PrinciplesRandomFields).

#### False discovery rate (FDR) ( ??? )

https://brainder.org/2011/09/05/fdr-corrected-fdr-adjusted-p-values/#comment-15388

#### Permutation tests ( ??? )

[A primer on permutation testing (not only) for MVPA](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116074)
by [Carsten Allefeld](https://twitter.com/c_allefeld) (36 min)

The [prevalence test](https://github.com/allefeld/prevalence-permutation)

#### SnPM ( ??? )

- [website](https://warwick.ac.uk/fac/sci/statistics/staff/academic-research/nichols/software/snpm)

#### FSL PALM and Randomize( ??? )

#### Freesurfer PALM ( ??? )

### Encoding models ( ??? )

https://nikokriegeskorte.org/tag/encoding-models/

#### Popeye

Python based pRF analysis.

- [website]https://popeye.readthedocs.io/en/latest/index.html)

#### SAMSRF

A pRF analysis toolbox called the Seriously Annoying Matlab SuRFer from
[Sam Schwarzkopf](https://twitter.com/sampendu).

- [website](https://sampendu.net/seriously-annoying-matlab-surfer/)

## Robustness checks

Non neuroimaging cases

- [multiverse analysis]()
- [specification curves]() presented in a talk at SPSP
  [here](https://www.youtube.com/watch?v=g75jstZidX0
- vibration of effects

## Computational neuroscience

This [paper](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5230746/) comes with
[some material](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005142#sec011)
to apply bayesian decoding analysis to neuronal data can be of interest.

### Free energy

As someone said on twitter there is a cottage industry of blog posts trying to
understand/explain this:

- https://medium.com/@solopchuk/intuitions-on-predictive-coding-and-the-free-energy-principle-3fc5bcedc754
- http://romainbrette.fr/what-is-computational-neuroscience-xxix-the-free-energy-principle/
- https://kaiu.me/2017/06/23/deep-active-inference-for-artificial-general-intelligence/
- http://slatestarcodex.com/2018/03/04/god-help-us-lets-try-to-understand-friston-on-free-energy
- http://www.aliannajmaren.com/2017/07/27/how-to-read-karl-friston-in-the-original-greek/

And a
[tutorial](https://medium.com/@solopchuk/tutorial-on-active-inference-30edcf50f5dc)

### Dynamic causal modelling

[A tutorial series on DCM](https://www.youtube.com/watch?v=q-yypnHgCII&list=PLwiAO9Cs0Tb8wUGAnYY5yIMckB9tc4T3_)
by [Kevin Aquino](https://twitter.com/kevin_m_aquino) [6 hrs]

## Laminar and high-resolution MRI

[Renzo Hubert](https://twitter.com/layerfmri) is keeping track of the most
recent development of laminar MRI via twitter but also on his
[blog](https://layerfmri.com/). He also curates laminar-fMRI related talks on
his
[Youtube channel](https://www.youtube.com/channel/UCMjtQ3FD41pAh1VJz-UZGJQ/videos)
or papers in this
[google spreahsheet](https://docs.google.com/spreadsheets/d/1DFdXA98bYPzK5Gf0M_PbNu3opvO-DIcrv7TMP5ywTMk/edit#gid=0).

- This
  [blog post](https://layerfmri.com/2018/01/04/layer-fmri-software-in-the-field/)
  has a list of most of the softwares that are related to laminar fMRI.
- A [more recent tool](https://github.com/kwagstyl/surface_tools) not listed in
  there for creating equivolumetric surfaces.

In terms of functional data there is high-res VASO (CBV) dataset
[here](https://openneuro.org/datasets/ds001547).

For anatomical data you can have a look [here](???).

BID conference

## Meta analysis ( ??? )

- A
  [talk](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116072)
  by [Tom Nichols](https://twitter.com/ten_photos) at OHBM 2018 for an
  [overview](https://figshare.com/articles/Overview_of_Meta-Analysis_Approaches/6723839)
- A
  [practical](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116073)
  by [Camille Maumet](https://twitter.com/cmaumet) at OHBM 2018 on
  meta-analysis: [slides] ( ??? )
- A talk on ALE and brainmap
  https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116066

[NiMARE](https://github.com/neurostuff/NiMARE) is a Python library for
coordinate- and image-based meta-analysis.
[Chris Gorgolewski](https://twitter.com/ChrisFiloG) wrote a
[tutorial](https://www.kaggle.com/chrisfilo/coordinate-and-image-metaanalysis-with-nimare)
on how to use it.

https://github.com/NeuroVault/metanalysis_examples

For coordinate based meta-analysis:

- [brainmap](http://www.brainmap.org/) with
  [Sleuth](http://www.brainmap.org/software.html#Sleuth) and
  [GingerALE](http://www.brainmap.org/software.html#GingerALE)

For image based meta-analysis:

- [IBMA](https://github.com/NeuroimagingMetaAnalysis/ibma) is the Image-Based
  Meta-Analysis toolbox for SPM.
