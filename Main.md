# On-line neuroimaging resources

I try to list here links to softwares, databases, tutorials, blogs and other resources list that I or others have found relevant to learn about neuroimaging or to help us perform neuroimaging analysis. Most of the things listed here are for fMRI but feel free to point towards EEG, MEG, TMS things too. Feel free to add things: see the **How to contribute** section below.

This document is mostly meant for me to be able to quickly find things without having to google them or browse through my bookmarks, pocket, github stars and repos. But if it can help others, that's great.

Also I am by no means an expert or even have used or done all the things I list... But I wish I had and I wish someone had told me some of those things 5 years ago.

I am also working on a companion [reading list] (  ???  ).

<!-- TOC -->

- [On-line neuroimaging resources](#on-line-neuroimaging-resources)
  - [Metalist](#metalist)
    - [Neuroimaging Informatics Tools and Resources Clearinghouse](#neuroimaging-informatics-tools-and-resources-clearinghouse)
    - [Lab guides and lab wikis](#lab-guides-and-lab-wikis)
    - [Others](#others)
  - [Online courses](#online-courses)
  - [Video series](#video-series)
    - [Mumford brainstats](#mumford-brainstats)
    - [Andrew Jahn](#andrew-jahn)
    - [Center for Brains, Minds and Machines](#center-for-brains-minds-and-machines)
    - [Organization from human brain mapping (OHBM)](#organization-from-human-brain-mapping-ohbm)
    - [fMRIf summer courses from the NIH](#fmrif-summer-courses-from-the-nih)
    - [Conference on Cognitive Computational Neuroscience (CCN)](#conference-on-cognitive-computational-neuroscience-ccn)
  - [Blogs](#blogs)
  - [Where to ask for help](#where-to-ask-for-help)
  - [Image formats](#image-formats)
    - [s and q matrices](#s-and-q-matrices)
    - [NIFTI](#nifti)
  - [UNIX command line](#unix-command-line)
  - [Matlab and SPM specific resources](#matlab-and-spm-specific-resources)
    - [Matlab (   ???   )](#matlab-------)
    - [SPM](#spm)
  - [The python ecosystem (   ???   )](#the-python-ecosystem-------)
  - [R](#r)
  - [Web apps (   ???   )](#web-apps-------)
    - [R based apps](#r-based-apps)
    - [Vizualizaton](#vizualizaton)
    - [Anatomy atlases (   ???   )](#anatomy-atlases-------)
  - [EEG and MEG Softwares](#eeg-and-meg-softwares)
  - [[BEFORE YOU START](BeforeYouStart.md)](#before-you-startbeforeyoustartmd)
    - [[Reproducibility (   ???   )](BeforeYouStart.md/#reproducibility-------)](#reproducibility-------beforeyoustartmdreproducibility-------)
    - [[Ethics and consent forms](BeforeYouStart.md/#ethics-and-consent-forms)](#ethics-and-consent-formsbeforeyoustartmdethics-and-consent-forms)
    - [[Code and data management (   ???   )](BeforeYouStart.md/#code-and-data-management-------)](#code-and-data-management-------beforeyoustartmdcode-and-data-management-------)
      - [[Code management](BeforeYouStart.md/#code-management)](#code-managementbeforeyoustartmdcode-management)
        - [[Version control](BeforeYouStart.md/#version-control)](#version-controlbeforeyoustartmdversion-control)
        - [[Coding style](BeforeYouStart.md/#coding-style)](#coding-stylebeforeyoustartmdcoding-style)
        - [[Avoid selective debugging: unit tests, positive and negative control](#avoid-selective-debugging-unit-tests-positive-and-negative-control)](#avoid-selective-debugging-unit-tests-positive-and-negative-controlavoid-selective-debugging-unit-tests-positive-and-negative-control)
      - [[Data: BIDS, Datalad and YODA](BeforeYouStart.md/#data-bids-datalad-and-yoda)](#data-bids-datalad-and-yodabeforeyoustartmddata-bids-datalad-and-yoda)
        - [[BIDS](BeforeYouStart.md/#bids)](#bidsbeforeyoustartmdbids)
        - [[Datalad](BeforeYouStart.md/#datalad)](#dataladbeforeyoustartmddatalad)
        - [[YODA](BeforeYouStart.md/#yoda)](#yodabeforeyoustartmdyoda)
      - [[Documentation (   ???   )](BeforeYouStart.md/#documentation-------)](#documentation-------beforeyoustartmddocumentation-------)
  - [[PLANNING YOUR STUDY](PlanningYourStudy.md/#planning-your-study)](#planning-your-studyplanningyourstudymdplanning-your-study)
    - [[Reusing data](PlanningYourStudy.md/#reusing-data)](#reusing-dataplanningyourstudymdreusing-data)
    - [[Defining your terms and your task](PlanningYourStudy.md/#defining-your-terms-and-your-task)](#defining-your-terms-and-your-taskplanningyourstudymddefining-your-terms-and-your-task)
    - [[Ontologies](PlanningYourStudy.md/#ontologies)](#ontologiesplanningyourstudymdontologies)
    - [[Piloting (   ???   )](PlanningYourStudy.md/#piloting-------)](#piloting-------planningyourstudymdpiloting-------)
    - [[Pre-registration](PlanningYourStudy.md/#pre-registration)](#pre-registrationplanningyourstudymdpre-registration)
    - [[Optimizing your design](PlanningYourStudy.md/#optimizing-your-design)](#optimizing-your-designplanningyourstudymdoptimizing-your-design)
    - [[Design efficiency (   ???   )](PlanningYourStudy.md/#design-efficiency-------)](#design-efficiency-------planningyourstudymddesign-efficiency-------)
    - [[Power](PlanningYourStudy.md/#power)](#powerplanningyourstudymdpower)
    - [[For MVPA: same analysis approach](PlanningYourStudy.md/#for-mvpa-same-analysis-approach)](#for-mvpa-same-analysis-approachplanningyourstudymdfor-mvpa-same-analysis-approach)
    - [[Defining your region of interest (   ???   )](PlanningYourStudy.md/#defining-your-region-of-interest-------)](#defining-your-region-of-interest-------planningyourstudymddefining-your-region-of-interest-------)
    - [[Using previous results (   ???   )](PlanningYourStudy.md/#using-previous-results-------)](#using-previous-results-------planningyourstudymdusing-previous-results-------)
    - [[Localizers (   ???   )](PlanningYourStudy.md/#localizers-------)](#localizers-------planningyourstudymdlocalizers-------)
    - [[Atlases](PlanningYourStudy.md/#atlases)](#atlasesplanningyourstudymdatlases)
    - [[Non-standard templates (   ???   )](PlanningYourStudy.md/#non-standard-templates-------)](#non-standard-templates-------planningyourstudymdnon-standard-templates-------)
  - [Getting data](#getting-data)
    - [Stimuli presentation softwares](#stimuli-presentation-softwares)
      - [psychopy](#psychopy)
      - [expyriment](#expyriment)
      - [psychtoolbox](#psychtoolbox)
    - [Existing protocols](#existing-protocols)
  - [[ONCE YOU HAVE DATA](OnceYouHaveYourData.md/#once-you-have-data)](#once-you-have-dataonceyouhaveyourdatamdonce-you-have-data)
    - [[quality control](OnceYouHaveYourData.md/#quality-control)](#quality-controlonceyouhaveyourdatamdquality-control)
    - [[preprocessing](OnceYouHaveYourData.md/#preprocessing)](#preprocessingonceyouhaveyourdatamdpreprocessing)
      - [[Pipelines  (   ???   )](OnceYouHaveYourData.md/#pipelines--------)](#pipelines--------onceyouhaveyourdatamdpipelines--------)
      - [[Artefact/Noise removal (   ???   )](OnceYouHaveYourData.md/#artefactnoise-removal-------)](#artefactnoise-removal-------onceyouhaveyourdatamdartefactnoise-removal-------)
        - [[PCA  (   ???   )](OnceYouHaveYourData.md/#pca--------)](#pca--------onceyouhaveyourdatamdpca--------)
        - [[ICA  (   ???   )](OnceYouHaveYourData.md/#ica--------)](#ica--------onceyouhaveyourdatamdica--------)
        - [[ART (   ???   )](OnceYouHaveYourData.md/#art-------)](#art-------onceyouhaveyourdatamdart-------)
        - [[ART repair (   ???   )](OnceYouHaveYourData.md/#art-repair-------)](#art-repair-------onceyouhaveyourdatamdart-repair-------)
        - [[Physiological noise  (   ???   )](OnceYouHaveYourData.md/#physiological-noise--------)](#physiological-noise--------onceyouhaveyourdatamdphysiological-noise--------)
        - [[Motion](OnceYouHaveYourData.md/#motion)](#motiononceyouhaveyourdatamdmotion)
    - [[Analysis](OnceYouHaveYourData.md/#analysis)](#analysisonceyouhaveyourdatamdanalysis)
      - [[general linear model](OnceYouHaveYourData.md/#general-linear-model)](#general-linear-modelonceyouhaveyourdatamdgeneral-linear-model)
      - [[Model selection (   ???   )](OnceYouHaveYourData.md/#model-selection-------)](#model-selection-------onceyouhaveyourdatamdmodel-selection-------)
      - [[Multivariate analysis (   ???   )](OnceYouHaveYourData.md/#multivariate-analysis-------)](#multivariate-analysis-------onceyouhaveyourdatamdmultivariate-analysis-------)
        - [[Matlab based](OnceYouHaveYourData.md/#matlab-based)](#matlab-basedonceyouhaveyourdatamdmatlab-based)
          - [[TDT](OnceYouHaveYourData.md/#tdt)](#tdtonceyouhaveyourdatamdtdt)
          - [[ProNTo](#pronto)](#prontopronto)
          - [[RSA toolbox](OnceYouHaveYourData.md/#rsa-toolbox)](#rsa-toolboxonceyouhaveyourdatamdrsa-toolbox)
          - [[PCM toolbox](OnceYouHaveYourData.md/#pcm-toolbox)](#pcm-toolboxonceyouhaveyourdatamdpcm-toolbox)
          - [[cvMANOVA](OnceYouHaveYourData.md/#cvmanova)](#cvmanovaonceyouhaveyourdatamdcvmanova)
        - [[Python based](OnceYouHaveYourData.md/#python-based)](#python-basedonceyouhaveyourdatamdpython-based)
          - [[pyMVPA](OnceYouHaveYourData.md/#pymvpa)](#pymvpaonceyouhaveyourdatamdpymvpa)
          - [[nilearn](OnceYouHaveYourData.md/#nilearn)](#nilearnonceyouhaveyourdatamdnilearn)
        - [[R based (   ???   )](OnceYouHaveYourData.md/#r-based-------)](#r-based-------onceyouhaveyourdatamdr-based-------)
      - [[Resting state (   ???   )](OnceYouHaveYourData.md/#resting-state-------)](#resting-state-------onceyouhaveyourdatamdresting-state-------)
      - [[Diffusion weighted imaging](OnceYouHaveYourData.md/#diffusion-weighted-imaging)](#diffusion-weighted-imagingonceyouhaveyourdatamddiffusion-weighted-imaging)
      - [[Statistical inferences and multiple comparison correction (MCP) (   ???   )](OnceYouHaveYourData.md/#statistical-inferences-and-multiple-comparison-correction-mcp-------)](#statistical-inferences-and-multiple-comparison-correction-mcp-------onceyouhaveyourdatamdstatistical-inferences-and-multiple-comparison-correction-mcp-------)
        - [[Cluster based inference (   ???   )](OnceYouHaveYourData.md/#cluster-based-inference-------)](#cluster-based-inference-------onceyouhaveyourdatamdcluster-based-inference-------)
        - [[Family wise error (FWE) (   ???   )](OnceYouHaveYourData.md/#family-wise-error-fwe-------)](#family-wise-error-fwe-------onceyouhaveyourdatamdfamily-wise-error-fwe-------)
        - [[False discovery rate (FDR) (   ???   )](OnceYouHaveYourData.md/#false-discovery-rate-fdr-------)](#false-discovery-rate-fdr-------onceyouhaveyourdatamdfalse-discovery-rate-fdr-------)
        - [[Permutation tests (   ???   )](OnceYouHaveYourData.md/#permutation-tests-------)](#permutation-tests-------onceyouhaveyourdatamdpermutation-tests-------)
        - [[SnPM (   ???   )](OnceYouHaveYourData.md/#snpm-------)](#snpm-------onceyouhaveyourdatamdsnpm-------)
        - [[FSL PALM and Randomize(   ???   )](OnceYouHaveYourData.md/#fsl-palm-and-randomize------)](#fsl-palm-and-randomize------onceyouhaveyourdatamdfsl-palm-and-randomize------)
        - [[Freesurfer PALM (   ???   )](OnceYouHaveYourData.md/#freesurfer-palm-------)](#freesurfer-palm-------onceyouhaveyourdatamdfreesurfer-palm-------)
      - [[Encoding models (   ???   )](OnceYouHaveYourData.md/#encoding-models-------)](#encoding-models-------onceyouhaveyourdatamdencoding-models-------)
        - [[Popeye](OnceYouHaveYourData.md/#popeye)](#popeyeonceyouhaveyourdatamdpopeye)
        - [[SAMSRF](OnceYouHaveYourData.md/#samsrf)](#samsrfonceyouhaveyourdatamdsamsrf)
    - [[Robustness checks](OnceYouHaveYourData.md/#robustness-checks)](#robustness-checksonceyouhaveyourdatamdrobustness-checks)
    - [[Computational neuroscience](OnceYouHaveYourData.md/#computational-neuroscience)](#computational-neuroscienceonceyouhaveyourdatamdcomputational-neuroscience)
      - [[Free energy](OnceYouHaveYourData.md/#free-energy)](#free-energyonceyouhaveyourdatamdfree-energy)
      - [[Dynamic causal modelling](OnceYouHaveYourData.md/#dynamic-causal-modelling)](#dynamic-causal-modellingonceyouhaveyourdatamddynamic-causal-modelling)
    - [[Laminar and high-resolution MRI](OnceYouHaveYourData.md/#laminar-and-high-resolution-mri)](#laminar-and-high-resolution-mrionceyouhaveyourdatamdlaminar-and-high-resolution-mri)
    - [[Meta analysis (   ???   )](OnceYouHaveYourData.md/#meta-analysis-------)](#meta-analysis-------onceyouhaveyourdatamdmeta-analysis-------)
  - [REPORTING METHODS AND RESULTS (also useful for reviewing papers)](#reporting-methods-and-results-also-useful-for-reviewing-papers)
    - [A checklist: COBIDAS report](#a-checklist-cobidas-report)
    - [Percent signal change (   ???   )](#percent-signal-change-------)
    - [Making figures (   ???   )](#making-figures-------)
    - [Tools to check results/statistics (   ???   )](#tools-to-check-resultsstatistics-------)
    - [Peer review (   ???   )](#peer-review-------)
  - [YOU ARE NOT DONE YET: sharing your code, data and your results](#you-are-not-done-yet-sharing-your-code-data-and-your-results)
    - [Sharing code](#sharing-code)
    - [NeuroImaging Data Model (NIDM)](#neuroimaging-data-model-nidm)
    - [Sharing your data](#sharing-your-data)
    - [Meta-analysis databases](#meta-analysis-databases)

<!-- /TOC -->


---

**How to use this document**
Most people don't use a map by starting in the upper left corner, scanning horizontally till they end up in the bottom right corner (or however it is that people read in the region of the world you are in at the moment). Similarly this document is obviously not meant to be read from top to bottom. The best is to browse the **Table of content** below and jump to section that interests you. For that reason there is some redundancy in the content. This also means that this document is not a cookbook: I just try to list things that could apply a to wide variety of topics and context, but in many cases only a handful of those will be relevant to you.

Note also that some of the sectioning is bit arbitrary: I try to put cross-links where useful.



**To add in the list**

http://cbs.fas.harvard.edu/science/core-facilities/neuroimaging/information-investigators/MRphysicsfaq
https://emmarobinson01.com/2016/10/07/forget-weak-statistics-fmri-studies-suffer-from-oversimplified-assumptions-made-during-pre-processing/

specific talks from
mumfordbrainstats
OHBM conference
other video series
Meehl philosophy lectures

stats blogs (Gelman, Mayo )

study swap

replication award

BOOKS
http://www.neuroimagingprimers.org/

HUMOR
`#MRIvalentines`
http://www.fmri4newbies.com/humor/
https://collectivelyunconscious.wordpress.com/2012/11/02/brain-region-found-that-does-absolutely-nothing/
https://www.theguardian.com/science/head-quarters/2014/apr/01/fmri-brain-imaging-spoof-april-fools
"- Designing an fMRI experiment is like building a miniature ship in a glass bottle. Every direction you want to move in you find some new unanticipated constraints.
- That's on a good day. Most days it is more like building a miniature ship in a glass bottle in the dark while drunk and with one hand tied behind your back."

---

## Metalist
There are tons of on-line resources for neuroimaging data analysis so the following list is not meant to be exhaustive. There are also similar lists here and there that might partly overlap with this one, so here is a list of lists.


### Neuroimaging Informatics Tools and Resources Clearinghouse
The most obvious place where everything is centralized is the [Neuroimaging Informatics Tools and Resources Clearinghouse](https://www.nitrc.org/). Many tools, atlases, courses are there but if your favorite isn't make sure to add it.


### Lab guides and lab wikis
If your lab does not have a lab guide/wiki, it is well worth the time to make one. Lab wikis can save a lot of time for newcomers to get set up and started (rather than reinvent the wheel or take time from other lab members), while lab guides will also help PIs, PhD students and post-docs know what to expect from each others and to promote a [healthier lab culture](https://www.nature.com/articles/d41586-018-05142-9). [Mariam Aly](https://twitter.com/mariam_s_aly) explains that well [here](https://www.nature.com/articles/d41586-018-06167-w).

If you lab does not have a guide and/or wiki here is a [list](https://docs.google.com/spreadsheets/d/1kn4A0nR4loUOSDn9Qysd3MqFJ9cGU91dCDM6x9aga-8/edit#gid=0) you can use to create your own. But I suggest that you go beyond a copy-paste as the ones you find in there might not be tailored to your lab's needs.

And here are some neuroimaging oriented lab wikis:
* [Mariam Aly's](https://twitter.com/mariam_s_aly) lab wiki is [there](https://osf.io/kgd9b/wiki/home/).
* [Jonathan Peelle](@jpeelle) has a great [list of resources](http://jonathanpeelle.net/mri-resources-for-beginners) for beginners.
* Check the [wiki](http://imaging.mrc-cbu.cam.ac.uk/imaging/CbuImaging) from the CBU in Cambridge.
* The one from [Tor Wager's](https://twitter.com/torwager) [lab](https://canlabweb.colorado.edu/wiki/doku.php/help/fmri_tools_documentation)
* Michael Beauchamp's lab [wiki](https://openwetware.org/wiki/Beauchamp:Lab_Notebook)
* Chris Rorden's Neuropsychology Lab [wiki](https://www.mccauslandcenter.sc.edu/crnl/tools)
* The [Kording](https://twitter.com/KordingLab) lab and Kendrick Kay's labs are more computational oriented and so check [them](http://kordinglab.com/resources/) [out](http://cvnlab.net/resources.html) if this is what you do.


### Others
* [Stephan Heunis](https://twitter.com/fmrwhy) has a [list](https://www.fmrwhy.com/2018/06/28/spm12-matlab-scripting-tutorial-4/) to many SPM and matlab material.
* [https://github.com/brainhack101](https://github.com/brainhack101) also has a [collections or links](https://brainhack101.github.io/neurolinks/) to courses, data...
* ReproNim is a good [site](http://www.reproducibleimaging.org/index.html) to get up to date on doing reproducible neuroimaging research.
* [Open neuroscience](https://openeuroscience.com/) points to a lot of open things related to neuroscience.
* There [MOOC on open-science](https://opensciencemooc.eu/) is still under construction but already has an insane [list of resources](https://opensciencemooc.eu/resources/).
* A [list](https://docs.google.com/document/d/1Wt6sZUavq4oQf4t3tpQARcajf-6i4TtHlx_lw-WJD1U/edit#heading=h.rgwbys315r9s) of Scientific Coding Resource put together by [neuroconscience] (   ???   )
* [Aya Ben-Yakov](@aya_ben_yakov) compiled a great list of [open-science resources](http://www.mrc-cbu.cam.ac.uk/openscience/resources/) for the CBU in Cambridge.
* [LabHacks](https://github.com/pbeukema/LabHacks) is a list of resources for data driven neuroscientists put together by Patrick Beukema
* a list of [open computational neuroscience resources](‏ https://github.com/asoplata/open-computational-neuroscience-resources/blob/master/README.md) put together by [Austin Soplata](https://twitter.com/austinsoplata)
* a list of [Computational resources](https://github.com/martinagvilas/lists/blob/master/computational_resources.md) put together by [Martina Vilas](https://twitter.com/martinagvilas)
* a [list of resources for machine learning](https://sgfin.github.io/learning-resources/) put together by Sam Finlayson
* [Matthew Brett](http://matthew.dynevor.org/) has some great tutorials on [neuroimaing](http://matthew.dynevor.org/research/publications.html#pubs-methodology) as well as some [math or IT skills that you should know about](http://matthew-brett.github.io/teaching/)


https://anisha.pizza/#/projects
https://brainlife.io/


## Online courses
See the [online courses page](.OnlinesCourses.md).

## Video series
If you run out of things to binge on Netflix, Youtube has some useful channels if you want to learn more about fMRI data analysis. I also list here other repository of MRI related videos.


### Mumford brainstats
Jeanette Mumford has a fantastic series of videos on neuroimaging analysis on [youtube](https://www.youtube.com/channel/UCZ7gF0zm35FwrFpDND6DWeA). The channel also has [Facebook group](https://www.facebook.com/groups/mumfordbrainstats/) (as well as a [tumblr](http://mumfordbrainstats.tumblr.com/) and [twitter account](https://twitter.com/mumbrainstats)) if you have questions.


### Andrew Jahn
[Here](https://www.youtube.com/user/Shala5ha5ka) for the videos but he also as a [blog](https://www.andysbrainblog.com/) (see the old version [here](http://andysbrainblog.blogspot.com)). He has some very good follow along 'tutorials' for FSL, SPM, Freesurfer and AFNI amongst other things.


### Center for Brains, Minds and Machines
[Here](https://www.youtube.com/channel/UCGoxKRfTs0jQP52cfHCyyRQ)


### Organization from human brain mapping (OHBM)
The videos of the lectures and workshops from the previous HBM conferences are available online [here](https://www.pathlms.com/ohbm/courses).


### fMRIf summer courses from the NIH
[Here](https://fmrif.nimh.nih.gov/public/fmri-course/)


### Conference on Cognitive Computational Neuroscience (CCN)
This new [conference](https://ccneuro.org/) has the videos from its first edition [here](https://ccneuro.org/2017/index.html@p=602.html)


CBU openscience workshop 2016 http://www.mrc-cbu.cam.ac.uk/openscience2016/

Justin O'Brien
https://www.youtube.com/playlist?list=PLxItDNjOWyDVMOerTs-ZRwtQQSE76ULm5


## Blogs
There are many excellent blogs run by neuroscientists where you can find interesting and more or less technical information on neuroimaging analysis. I list a few below but you can find a subsample of my neuroscience blogroll in the file [blogroll_a_sample.opml](.blogroll_a_sample.opml) that you can import into your favorite news reader (e.g [feedly](https://feedly.com)).

* [Jo Etzel](https://twitter.com/JosetAEtzel) has a great blog if you want to know more about multivariate analysis: [MVPA meandering](http://mvpa.blogspot.co.uk)
* [practiCal fMRI](https://twitter.com/practiCalfMRI) has good [blog](http://practicalfmri.blogspot.co.uk) posts that cover the basics of fMRI, MRI artefacts, as well as a all the things that can affect the BOLD signal
* [techniCal fMRI](http://technicalfmri.blogspot.com/) companion to practiCal fMRI that covers topics related to ancillary equipment for fMRI scanning.
* [Chris Chambers](https://twitter.com/chrisdc77) blog is [Neurochambers](http://neurochambers.blogspot.co.uk)s
* [Neuroskeptic](https://twitter.com/Neuro_Skeptic) blogs at [Neuroskeptic](http://blogs.discovermagazine.com/neuroskeptic/)
* [Dorothy Bishop](https://twitter.com/deevybee) is [there](http://deevybee.blogspot.com/).
* [Russel Poldracks](https://twitter.com/russpoldrack) posts can be found [here](http://www.russpoldrack.org)
* [Peter Bandettini](https://twitter.com/fMRI_today) blogs at [the brain blog](http://www.thebrainblog.org)
* [Peter Molfese](https://twitter.com/commander_crash) blogs at [Crash Log](http://blog.cogneurostats.com/), somewhat AFNI focused.



## Where to ask for help
If you have question linked to a specific software, check the documentation/FAQ/manual/wiki/tutorial for that software first. Then you can turn to [the mailing list](https://kirstiewhitaker.com/2014/12/16/how-to-use-the-fsl-and-freesurfer-mailing-lists-for-success-in-your-phd/) related to that software: but always start by looking through the archives of those mailing lists first before sending a question that has already been answered.

But if you have more general questions you can also try :
* the [neurostars](https://neurostars.org/) forum
* social medias: there are some specialised Facebook groups or good hashtags on twitter that will succeed when your google fu fails you.
* the slack channel of [brainhack](https://www.brainhack.org/)



## Image formats

### s and q matrices

https://nifti.nimh.nih.gov/nifti-1/documentation/nifti1fields/nifti1fields_pages/qsform_brief_usage/document_view
https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/Orientation%20Explained
http://gru.stanford.edu/doku.php/mrTools/coordinateTransforms

more on nibabel

### NIFTI

https://brainder.org/2012/09/23/the-nifti-file-format/#comment-16430
https://brainder.org/2015/04/03/the-nifti-2-file-format/




## UNIX command line
Even if you have only used Windows in your life, the odds are that you will at some point have to use a UNIX command line (like the one you can find on a linux computer or a Mac) to do some of your MRI analysis. Best case scenario you might only need it to explore some folder structure on some server, worst case you might have to write some scripts to automate some tasks. Either way, having some basics ideas about how to interact with a UNIX is a good idea.

* from the FSL [website](https://fsl.fmrib.ox.ac.uk/fslcourse/lectures/scripting/all.htm)
* on the MRC-CBU [wiki](http://imaging.mrc-cbu.cam.ac.uk/methods/unixsurvivalguide)
* from software carpentry for [beginners](http://swcarpentry.github.io/shell-novice/) and more [advanced users](http://swcarpentry.github.io/shell-extras/)
* also for [beginners](http://www.ee.surrey.ac.uk/Teaching/Unix/)
* for [more advanced scripting](https://wilsonericn.wordpress.com/2011/08/25/find-grep-sed-and-awk) (h/t [Tom Nichols](https://twitter.com/ten_photos))



https://bash.cyberciti.biz/guide/Main_Page



## Matlab and SPM specific resources

### Matlab (   ???   )
* tutorials
I learnt matlab with a book and by reading other's scripts and with a lot of coffee, patience, sweat, tears and, trial and errors. I am sure there are better ways to do it than that but I don't really know what the best tutorials are these days.

### SPM
* The first place to look is the [SPM wiki book](https://en.wikibooks.org/wiki/SPM) that could become a even better resource if users contributed even more to it.
* Then you can check the [add-ons for SPM](https://www.fil.ion.ucl.ac.uk/spm/ext/).
* https://www.youtube.com/playlist?list=PLxItDNjOWyDVMOerTs-ZRwtQQSE76ULm5
* Justin O'Brien has a [good tutorial video series](https://www.youtube.com/playlist?list=PLxItDNjOWyDVMOerTs-ZRwtQQSE76ULm5) on how to analyze data with SPM from beginning to the end.
* The spm.mat is the file where SPM stores all the information about your analysis. This [page](http://people.duke.edu/~njs28/spmdatastructure.htm) explains its organization.
* If you want to write scripts and use batches efficiently using SPM see what I wrote [here](./How2Script.md)
* [The clever machine](https://theclevermachine.wordpress.com/category/fmri/) blog has some very useful matlab codes for fMRI analysis
* [Tom Nichols](https://twitter.com/ten_photos) has tagged SPM related posts on his [website](http://blogs.warwick.ac.uk/nichols/) if you are looking for some good code snippets: see for example some of John Ashburner's [gems](http://blogs.warwick.ac.uk/nichols/tag/johns-gems/).
* Check out [Cyril Pernet](https://twitter.com/cyrilrpernet) website for SPM/matlab code: [here](http://www.sbirc.ed.ac.uk/cyril/teaching.html) or [there](http://www.sbirc.ed.ac.uk/cyril/Stats.html)
* Some good tutorials on the CBU if you want to understand [design efficiency](http://imaging.mrc-cbu.cam.ac.uk/imaging/DesignEfficiency), [smoothing](http://imaging.mrc-cbu.cam.ac.uk/imaging/PrinciplesSmoothing), [SPM GLM stats](http://imaging.mrc-cbu.cam.ac.uk/imaging/PrinciplesStatistics) or [how random field theory works to correct for multiple comparison](http://imaging.mrc-cbu.cam.ac.uk/imaging/PrinciplesRandomFields)
* Quite a few others on the web
 # [https://sites.google.com/site/mvlombardo/matlab-tutorials](https://sites.google.com/site/mvlombardo/matlab-tutorials)
 # [http://spm.martinpyka.de/](http://spm.martinpyka.de/)
 # [https://www.mccauslandcenter.sc.edu/crnl/tools/spm8-scripts](https://www.mccauslandcenter.sc.edu/crnl/tools/spm8-scripts)
* But also [too many repos on Github to list them all](https://github.com/search?q=matlab+fmri) but here are some you might come across: [Rik Henson's](https://github.com/MRC-CBU/riksneurotools), the [canlab](https://github.com/canlab)



## The python ecosystem (   ???   )
Matlab must still be the most used "language" in neuroimaging (citation needed) but there is huge neuroscience-oriented python ecosystem out there taking advantage of the scientific python community. On top of the financial aspect (those matlab licenses can be quite expensive), there are many good reasons why you might wanna switch if only because [matlab breeds](http://neuroplausible.com/matlab) [bad coding habits](http://www.rath.org/matlab-is-a-terrible-programming-language.html).

https://metarabbit.wordpress.com/2013/10/18/why-python-is-better-than-matlab-for-scientific-software/
https://www.stat.washington.edu/~hoytak/blog/whypython.html

Here too there are plenty of generic python courses on [datacamp](https://www.datacamp.com/tracks/python-programmer), [code academy](https://www.codecademy.com/learn/learn-python) or [kaggle](https://www.kaggle.com/learn/python). You can also check things that are more scientific python oriented like the [scipy lectures](http://www.scipy-lectures.org/) or Jake Vanderplas's jupyter notebooks [Whirlwind Tour Of Python](https://github.com/jakevdp/WhirlwindTourOfPython) and [Python Data Science Handbook](https://github.com/jakevdp/PythonDataScienceHandbook).

We might also want to check [An introduction to Python!](https://cogs18.github.io/intro/), the course made by [Thomas Donoghue](   ???   )

There are also a [handbook](https://www.enthought.com/white-paper-matlab-to-python) and a [course](https://www.fz-juelich.de/ias/jsc/EN/Expertise/Services/Documentation/presentations/presentation-matlab2python_table.html?nn=362392) that might ease the transition from matlab to python.

https://docs.scipy.org/doc/numpy-1.14.0/user/numpy-for-matlab-users.html

If you turn to neuroimaging in python I guess you will first want to go to check the [nipy website](http://nipy.org/) and then turn to [nibabel](http://nipy.org/nibabel/), [nipype](#Nipype), [nilearn](#nilearn), [pyMVPA](#pyMVPA), …


## R
http://compcogscisydney.org/psyr/
https://rweekly.org/
http://compcogscisydney.org/psyr/


## Web apps (   ???   )

p values are hard to understand but can be seen as a surprise factor: s-values express that by saying that your results no more surprising than getting all heads in X fair coin tosses. See this [blog post and web app](https://www.lesslikely.com/statistics/s-values/) to know more.


### R based apps
Even if they are not specific to neuroimaging many of the R based web based apps from [shiny apps](http://shinyapps.org/) and [R psychologist](http://rpsychologist.com/) can be very useful to help better understand:

*   [p-values](https://www.shinyapps.org/apps/vs-mpr/)
*   [confidence intervals](http://rpsychologist.com/d3/CI/)
*   [p curves](https://shinyapps.org/apps/p-checker/) and [why with a decent power and a large effect size, it is relatively unlikely to find a value between p<.01 and p<.05](http://rpsychologist.com/d3/pdist/)
*   [null hypothesis significance testing](http://rpsychologist.com/d3/NHST/)
*   [p hacking](https://www.shinyapps.org/apps/p-hacker/)
*   [positive predictive values](http://shinyapps.org/showapp.php?app=https://tellmi.psy.lmu.de/felix/PPV&by=Michael%20Zehetleitner%20and%20Felix%20Sch%C3%B6nbrodt&title=When%20does%20a%20significant%20p-value%20indicate%20a%20true%20effect?&shorttitle=When%20does%20a%20significant%20p-value%20indicate%20a%20true%20effect?)


### Vizualizaton
* the [bioimagesuite](https://bioimagesuiteweb.github.io/webapp/index.html) seems like a convenient way to visualize and do some processing of you images on the fly via a web-browser. (h/t [Renzo](https://twitter.com/layerfmri))

papaya and mango

http://gallantlab.org/pycortex/retinotopy_demo/



### Anatomy atlases (   ???   )
Some of those might help you learn or revise your neuroanatomy:
* http://www.med.harvard.edu/AANLIB/cases/caseNA/pb9.htm
* http://ghiasi.org/2009/05/10-great-sites-for-reviewing-brain-anatomy/
* http://atlas.brain-map.org/

http://gallantlab.org/pycortex/retinotopy_demo/


## EEG and MEG Softwares
See the [EEG and MEG Softwares page](MEEGsoftwares.md).


## [BEFORE YOU START](BeforeYouStart.md)

### [Reproducibility (   ???   )](BeforeYouStart.md/#reproducibility-------)
### [Ethics and consent forms](BeforeYouStart.md/#ethics-and-consent-forms)
### [Code and data management (   ???   )](BeforeYouStart.md/#code-and-data-management-------)
#### [Code management](BeforeYouStart.md/#code-management)
##### [Version control](BeforeYouStart.md/#version-control)
##### [Coding style](BeforeYouStart.md/#coding-style)
##### [Avoid selective debugging: unit tests, positive and negative control](#avoid-selective-debugging-unit-tests-positive-and-negative-control)
#### [Data: BIDS, Datalad and YODA](BeforeYouStart.md/#data-bids-datalad-and-yoda)
##### [BIDS](BeforeYouStart.md/#bids)
##### [Datalad](BeforeYouStart.md/#datalad)
##### [YODA](BeforeYouStart.md/#yoda)
#### [Documentation (   ???   )](BeforeYouStart.md/#documentation-------)


## [PLANNING YOUR STUDY](PlanningYourStudy.md/#planning-your-study)

### [Reusing data](PlanningYourStudy.md/#reusing-data)
### [Defining your terms and your task](PlanningYourStudy.md/#defining-your-terms-and-your-task)
### [Ontologies](PlanningYourStudy.md/#ontologies)
### [Piloting (   ???   )](PlanningYourStudy.md/#piloting-------)
### [Pre-registration](PlanningYourStudy.md/#pre-registration)
### [Optimizing your design](PlanningYourStudy.md/#optimizing-your-design)
### [Design efficiency (   ???   )](PlanningYourStudy.md/#design-efficiency-------)
### [Power](PlanningYourStudy.md/#power)
### [For MVPA: same analysis approach](PlanningYourStudy.md/#for-mvpa-same-analysis-approach)
### [Defining your region of interest (   ???   )](PlanningYourStudy.md/#defining-your-region-of-interest-------)
### [Using previous results (   ???   )](PlanningYourStudy.md/#using-previous-results-------)
### [Localizers (   ???   )](PlanningYourStudy.md/#localizers-------)
### [Atlases](PlanningYourStudy.md/#atlases)
### [Non-standard templates (   ???   )](PlanningYourStudy.md/#non-standard-templates-------)


## Getting data

### Stimuli presentation softwares

![Language](https://img.shields.io/badge/Language-Python-blue.svg)
#### psychopy
#### expyriment

![Language](https://img.shields.io/badge/Language-Matlab-orange.svg)
#### psychtoolbox



### Existing protocols

HBP public protocols

for pRF?

Other site centralizing existing protocols?


## [ONCE YOU HAVE DATA](OnceYouHaveYourData.md/#once-you-have-data)
### [quality control](OnceYouHaveYourData.md/#quality-control)
### [preprocessing](OnceYouHaveYourData.md/#preprocessing)
#### [Pipelines  (   ???   )](OnceYouHaveYourData.md/#pipelines--------)
#### [Artefact/Noise removal (   ???   )](OnceYouHaveYourData.md/#artefactnoise-removal-------)
##### [PCA  (   ???   )](OnceYouHaveYourData.md/#pca--------)
##### [ICA  (   ???   )](OnceYouHaveYourData.md/#ica--------)
##### [ART (   ???   )](OnceYouHaveYourData.md/#art-------)
##### [ART repair (   ???   )](OnceYouHaveYourData.md/#art-repair-------)
##### [Physiological noise  (   ???   )](OnceYouHaveYourData.md/#physiological-noise--------)
##### [Motion](OnceYouHaveYourData.md/#motion)
### [Analysis](OnceYouHaveYourData.md/#analysis)
#### [general linear model](OnceYouHaveYourData.md/#general-linear-model)
#### [Model selection (   ???   )](OnceYouHaveYourData.md/#model-selection-------)
#### [Multivariate analysis (   ???   )](OnceYouHaveYourData.md/#multivariate-analysis-------)
##### [Matlab based](OnceYouHaveYourData.md/#matlab-based)
###### [TDT](OnceYouHaveYourData.md/#tdt)
###### [ProNTo](#pronto)
###### [RSA toolbox](OnceYouHaveYourData.md/#rsa-toolbox)
###### [PCM toolbox](OnceYouHaveYourData.md/#pcm-toolbox)
###### [cvMANOVA](OnceYouHaveYourData.md/#cvmanova)
##### [Python based](OnceYouHaveYourData.md/#python-based)
###### [pyMVPA](OnceYouHaveYourData.md/#pymvpa)
###### [nilearn](OnceYouHaveYourData.md/#nilearn)
##### [R based (   ???   )](OnceYouHaveYourData.md/#r-based-------)
#### [Resting state (   ???   )](OnceYouHaveYourData.md/#resting-state-------)
#### [Diffusion weighted imaging](OnceYouHaveYourData.md/#diffusion-weighted-imaging)
#### [Statistical inferences and multiple comparison correction (MCP) (   ???   )](OnceYouHaveYourData.md/#statistical-inferences-and-multiple-comparison-correction-mcp-------)
##### [Cluster based inference (   ???   )](OnceYouHaveYourData.md/#cluster-based-inference-------)
##### [Family wise error (FWE) (   ???   )](OnceYouHaveYourData.md/#family-wise-error-fwe-------)
##### [False discovery rate (FDR) (   ???   )](OnceYouHaveYourData.md/#false-discovery-rate-fdr-------)
##### [Permutation tests (   ???   )](OnceYouHaveYourData.md/#permutation-tests-------)
##### [SnPM (   ???   )](OnceYouHaveYourData.md/#snpm-------)
##### [FSL PALM and Randomize(   ???   )](OnceYouHaveYourData.md/#fsl-palm-and-randomize------)
##### [Freesurfer PALM (   ???   )](OnceYouHaveYourData.md/#freesurfer-palm-------)
#### [Encoding models (   ???   )](OnceYouHaveYourData.md/#encoding-models-------)
##### [Popeye](OnceYouHaveYourData.md/#popeye)
##### [SAMSRF](OnceYouHaveYourData.md/#samsrf)
### [Robustness checks](OnceYouHaveYourData.md/#robustness-checks)
### [Computational neuroscience](OnceYouHaveYourData.md/#computational-neuroscience)
#### [Free energy](OnceYouHaveYourData.md/#free-energy)
#### [Dynamic causal modelling](OnceYouHaveYourData.md/#dynamic-causal-modelling)
### [Laminar and high-resolution MRI](OnceYouHaveYourData.md/#laminar-and-high-resolution-mri)
### [Meta analysis (   ???   )](OnceYouHaveYourData.md/#meta-analysis-------)


## REPORTING METHODS AND RESULTS (also useful for reviewing papers)


### A checklist: COBIDAS report
The organization from human brain mapping (OHBM) created the Committee on Best practices In Data Analysis and Sharing (COBIDAS) that published a report with a set of [guidelines](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5685169/) with an appended [checklist](https://www.biorxiv.org/content/early/2016/07/10/054262.full.pdf+html) on how to conduct and report fMRI studies. It is a very useful resource to use to make sure you are not forgetting anything when writing up your article.
See also Jeanette Mumford's [video](https://www.youtube.com/watch?v=bsM4KowO5Vc) about it.




* Journal specific requirements or checklists like those of Nature (   ???   ) or Elife (   ???   )
* [21 words solution] (   ???   )
* [Constraints on generality] (   ???   )
* Other checklists:
 # [here](http://biostat.mc.vanderbilt.edu/wiki/Main/ManuscriptChecklist)
 # http://jonathanpeelle.net/blog/2016/3/23/a-manuscript-checklist-for-improving-science





### Percent signal change (   ???   )




* a FAQ [article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3896880/) on the GLM by Cyril Pernet with [matlab code](https://www.frontiersin.org/articles/file/downloadfile/58014_supplementary-materials_datasheets_1_zip/octet-stream/Data%20Sheet%201.ZIP/2/58014) to go through has some mention on reporting PSC.
* See also this FSL [guide](http://mumford.bol.ucla.edu/perchange_guide.pdf) by Jeanette Mumford (   ???   ) for reporting results in PSC.
* This [post](http://blogs.warwick.ac.uk/nichols/entry/spm_plot_units/) by [Tom Nichols](https://twitter.com/ten_photos) can be helpful to understand what are the units that SPM paranter estimates are reported in.
* The [MarsBAR](http://marsbar.sourceforge.net/) SPM toolbox can also help you deal with PSC.
* From the [ArtRepair webiste](https://cibsr.stanford.edu/content/dam/sm/cibsr/documents/tools/methods/artrepair-software/FMRIPercentSignalChange.pdf)



### Making figures (   ???   )




I keep hearing that the books by Edward R. Tufte are great
https://www.amazon.com/dp/0961392118/?tag=codihorr-20
https://www.amazon.com/dp/0961392126/?tag=codihorr-20

http://mkweb.bcgsc.ca/essentials.of.data.visualization/
https://www.jisc.ac.uk/full-guide/data-visualisation
https://jimgrange.wordpress.com/2016/06/15/solution-to-barbarplots-in-r/
https://f1000research.com/articles/4-466/v1

blog and paper guillaume Rousselet
http://eelkespaak.nl/blog/customizing-common-m-eeg-plots-part-2-the-time-frequency-representation-tfr/

* Color maps
* http://colorbrewer2.org/#type=sequential&scheme=BuGn&n=3
 # color blind friendly
 # the JET colormap is EVIL
* https://davidmathlogic.com/colorblind/#%23D81B60-%231E88E5-%23FFC107-%23004D40

* Dual coded statistical maps
[Code](http://mialab.mrn.org/datavis/) to display beta values and t values on the same map. From the *Data visualization in the neurosciences: overcoming the curse of dimensionality* [paper](https://www.ncbi.nlm.nih.gov/pubmed/22632718).




### Tools to check results/statistics (   ???   )
Those recent tools cannot be applied to statistical maps but they can be useful for any behavioural results. Many of them can be used on a paper you are about to publish to check for errors or on a paper you are reviewing / reading.

* [Statcheck](http://statcheck.io/) developed by automatically checks for errors in statistical reporting making sure that your p values match with your t/F values and degrees of freedom.
* [GRIM test](http://www.prepubmed.org/grim_test/) checks for Granularity-Related Inconsistency of Means. Developed by [Nick Brown](https://twitter.com/sTeamTraen) and [James Heathers](https://twitter.com/jamesheathers) makes sure that the mean reported are plausible given a measurement scale (liek a Likert scale or a visual analog scale) and a sample size. There are [GRIMMER](http://www.prepubmed.org/grimmer/, GRIMMEST extension to standard deviations and F values.
* [SPRITE](https://peerj.com/preprints/26968v1/) stands for Sample Parameter Reconstruction via Iterative TEchniques and allows to generate the possible data distribution given a scale, a mean and variability measure [web app](http://www.prepubmed.org/sprite/), [shiny app](https://steamtraen.shinyapps.io/rsprite/), [code](https://osf.io/pwjad/).
* There is also the [p-checker shinyapp](https://shinyapps.org/apps/p-checker/) that lets you inspect/diagnose a group of results by doing a p-curve analysis, a test of insufficient variance, z-curve analysis, …



### Peer review (   ???   )




* [Peer review openness (PRO) initiative](https://opennessinitiative.org/) to ask for data






## YOU ARE NOT DONE YET: sharing your code, data and your results
There should be at least 3 boxes on your to do list once your study is completed.
* sharing the code
* sharing the data
* sharing the statistical map
* updating meta-analysis databases
If the 3 first points are done before an article submission it can be useful for reviewers to check what you have done. But all of those points are important also for future researchers that would like to base new research on your results or to run a meta-analysis of similar studies.


### Sharing code
You might be tempted to not [share your code](https://sinews.siam.org/Details-Page/top-ten-reasons-to-not-share-your-code-and-why-you-should-anyway). If your code and/or your jupyter notebooks are on a [github repository](#version-control), you can make snapshot of it to publish on zenodo as explained [here](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/tree/master/content_development).


### NeuroImaging Data Model (NIDM)
If you want to share your results I suggest you export your final results using the NIDM format that is supported natively by [SPM12](https://github.com/incf-nidash/nidmresults-spm). There are also tools for exporting [FSL](https://github.com/incf-nidash/nidmresults-fsl) results and things are under development for [AFNI](https://github.com/incf-nidash/nidmresults-afni). The NIDM format makes your results easily viewable by other softwares (check the [INCF-NIDASH](https://github.com/incf-nidash) repo for more information). There are extension in development for the NIDM to cover not only non-parametric statistical maps but also to export in very compact way [many of the details of about your experiment and analysis](http://nidm.nidash.org/specs/nidm-experiment_dev.html).

Another good reason to use the NIDM model is that it facilitates uploading them to a site like [neurovault](https://neurovault.org/) where you can store them and share them with others.


### Sharing your data
Some of the main databases where you can put your data are:
* [OpenNeuro](https://openneuro.org/) for rawdata
* [INDI](http://fcon_1000.projects.nitrc.org/) for rawdata
* [neurovault](https://neurovault.org/) for statistical maps
* [BALSA](https://balsa.wustl.edu/)
* [LORIS](https://github.com/aces/Loris/wiki/Open-LORIS)
* [XNAT](https://www.nitrc.org/ir/)
* [Pain repository](https://www.painrepository.org/])

But there are [many](https://brainhack101.github.io/neurolinks/) other [possibilities](https://en.wikipedia.org/wiki/List_of_neuroscience_databases) to share your raw and/or pre-processed data. Maybe your university or your institute has ways to help you share your data (e.g the [Donders institute](https://data.donders.ru.nl/?0).


FAIR data

https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/115883


### Meta-analysis databases
Another thing you can do to share your published results is to add them to meta-analytical databases like [ANIMA](http://anima.modelgui.org), [brainmap](http://www.brainmap.org/) or [neurosynth](http://neurosynth.org/): for this you could use [brainspell](http://brainspell.org/) and [Scribe](http://www.brainmap.org/software.html#Scribe).

Practical Intensity Based Meta-Analysis
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116073
Foundations and potential of meta-analyses
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116068
ALE and BrainMap
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116066
How to Plan and Prepare a Meta-Analysis
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116069
Neuroinformatics resources for coordinate and image-based meta-analysis
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116071
