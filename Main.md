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
  - [ONCE YOU HAVE DATA: quality control](#once-you-have-data-quality-control)
  - [ONCE YOU HAVE DATA: preprocessing](#once-you-have-data-preprocessing)
    - [Pipelines  (   ???   )](#pipelines--------)
    - [Artefact/Noise removal (   ???   )](#artefactnoise-removal-------)
      - [PCA  (   ???   )](#pca--------)
      - [ICA  (   ???   )](#ica--------)
      - [ART (   ???   )](#art-------)
      - [ART repair (   ???   )](#art-repair-------)
      - [Physiological noise  (   ???   )](#physiological-noise--------)
      - [Motion](#motion)
  - [ANALYSIS: general linear model](#analysis-general-linear-model)
  - [ANALYSIS: Resting state (   ???   )](#analysis-resting-state-------)
  - [Diffusion weighted imaging](#diffusion-weighted-imaging)
  - [ANALYSIS: Model selection (   ???   )](#analysis-model-selection-------)
  - [ANALYSIS: Statistical inferences and multiple comparison correction (MCP) (   ???   )](#analysis-statistical-inferences-and-multiple-comparison-correction-mcp-------)
    - [Cluster based inference (   ???   )](#cluster-based-inference-------)
    - [Family wise error (FWE) (   ???   )](#family-wise-error-fwe-------)
    - [False discovery rate (FDR) (   ???   )](#false-discovery-rate-fdr-------)
    - [Permutation tests (   ???   )](#permutation-tests-------)
      - [SnPM (   ???   )](#snpm-------)
      - [FSL PALM and Randomize(   ???   )](#fsl-palm-and-randomize------)
      - [Freesurfer PALM (   ???   )](#freesurfer-palm-------)
  - [ANALYSIS: Multivariate analysis (   ???   )](#analysis-multivariate-analysis-------)
    - [Matlab based](#matlab-based)
      - [TDT](#tdt)
      - [ProNTo](#pronto)
      - [RSA toolbox](#rsa-toolbox)
      - [PCM toolbox](#pcm-toolbox)
      - [cvMANOVA](#cvmanova)
    - [Python based](#python-based)
      - [pyMVPA](#pymvpa)
      - [nilearn](#nilearn)
    - [R based (   ???   )](#r-based-------)
  - [ANALYSIS: Encoding models (   ???   )](#analysis-encoding-models-------)
    - [Popeye](#popeye)
    - [SAMSRF](#samsrf)
  - [ANALYSIS: Robustness checks](#analysis-robustness-checks)
  - [ANALYSIS: Computational neuroscience](#analysis-computational-neuroscience)
    - [Free energy](#free-energy)
    - [Dynamic causal modelling](#dynamic-causal-modelling)
  - [ANALYSIS: Laminar and high-resolution MRI](#analysis-laminar-and-high-resolution-mri)
  - [ANALYSIS: Meta analysis (   ???   )](#analysis-meta-analysis-------)
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
  - [https://sites.google.com/site/mvlombardo/matlab-tutorials](https://sites.google.com/site/mvlombardo/matlab-tutorials)
  - [http://spm.martinpyka.de/](http://spm.martinpyka.de/)
  - [https://www.mccauslandcenter.sc.edu/crnl/tools/spm8-scripts](https://www.mccauslandcenter.sc.edu/crnl/tools/spm8-scripts)
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



## ONCE YOU HAVE DATA: quality control



* [quality control on MRI and fMRI](https://practicalfmri.blogspot.com/2014/08/qa-for-fmri-part-3-facility-qa-what-to.html)
* [COBIDacq](https://practicalfmri.blogspot.com/2017/12/cobidacq.html)
* https://en.wikibooks.org/wiki/Neuroimaging_Data_Processing/Data_Quality
* [Neuroimaging quality control task force](https://crossinvalidation.com/2018/07/31/neuroimaging-quality-control-niqc-task-force-to-develop-protocols-tools-and-manuals/)
* [References for quality control](https://www.zotero.org/groups/2221093/niqc)

* [MRIQC](https://mriqc.readthedocs.io/en/stable/) MRI quality control. A BIDS app that runs a pipeline to assess the quality of your data.
* [the PCP Quality Assessment Protocol](https://github.com/BIDS-Apps/QAP) is another BIDS app based on the protocol of [the connectome project data}(http://preprocessed-connectomes-project.org/quality-assessment-protocol/)
* [Scripts for quality control of diffusion data](http://davidroalf.com/script_download/)
* https://github.com/memobc/memolab-fmri-qa
* [Qoala-t](https://github.com/Qoala-T) for QA for freesurfer segmentations also with an online [shinyapp](https://qoala-t.shinyapps.io/qoala-t_app/)
* [Visual QC](https://github.com/raamana/visualqc) developed by [Pradeep](https://twitter.com/raamana_).

OHBM 2019 session on quality control by Pradeep

## ONCE YOU HAVE DATA: preprocessing

### Pipelines  (   ???   )
There are some ready made pipeline as [BIDS apps](http://bids-apps.neuroimaging.io/apps/) that already exist and have been tested. Using them might save you time and make your results more reproducible.
* [AFNI based](https://github.com/BIDS-Apps/afni_proc)
* [HCP Pipelines](https://github.com/BIDS-Apps/HCPPipelines): a set of tools (primarily, but not exclusively, shell scripts) for processing MRI images for the Human Connectome Project.
* [fMRIprep](https://fmriprep.readthedocs.io/en/stable/)
* [The NeuroImaging Analysis Kit](https://github.com/BIDS-Apps/niak): NIAK is a library of pipelines for the preprocessing and mining of large functional neuroimaging data.
* [Automatic Analysis](https://github.com/BIDS-Apps/aa): is a [pipeline system for neuroimaging](http://automaticanalysis.org/) written primarily in Matlab. It robustly supports recent versions of SPM, as well as selected functions from other software packages. The goal is to facilitate automatic, flexible, and replicable neuroimaging analyses through a comprehensive pipeline system.
* [nipypelines](https://github.com/BIDS-Apps/nipypelines)
* [Configurable Pipeline for the Analysis of Connectomes](https://github.com/BIDS-Apps/CPAC): C-PAC is a software for performing high-throughput preprocessing and analysis of functional connectomes data using high-performance computers.


There is also an [OPPNI](https://github.com/BIDS-Apps/oppni) for Optimization of Preprocessing Pipelines for NeuroImaging.


### Artefact/Noise removal (   ???   )

[GLM denoise](http://kendrickkay.net/GLMdenoise/)

ART repair

ART


#### PCA  (   ???   )

#### ICA  (   ???   )

#### ART (   ???   )

#### ART repair (   ???   )
https://cibsr.stanford.edu/tools/human-brain-project/artrepair-software.html

#### Physiological noise  (   ???   )

http://technicalfmri.blogspot.com/2018/02/physiological-monitoring-and-recording.html?m=1

#### Motion

http://blogs.discovermagazine.com/neuroskeptic/2014/07/06/fmri-scanning-dead/
http://blogs.discovermagazine.com/neuroskeptic/2013/11/26/head-movement-bad-news-neuroscience/
http://blogs.discovermagazine.com/neuroskeptic/2012/08/07/brains-in-motion-are-bad-for-neuroscience/


## ANALYSIS: general linear model




* a FAQ [article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3896880/) on the GLM by Cyril Pernet with [matlab code](https://www.frontiersin.org/articles/file/downloadfile/58014_supplementary-materials_datasheets_1_zip/octet-stream/Data%20Sheet%201.ZIP/2/58014) to go through
* see the section on [percent signal change](#percent-signal-change) to better understand how to report results
* orthogonalization of regressors can be a bit hard to wrap your head aroudnd at first but Jeanette Mumford (   ???   ) has great [paper](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0126255) on the topic with a [jupyter notebook](http://nbviewer.jupyter.org/github/jmumford/orthogonalizaton_ipynb/blob/master/orthogonalization.ipynb).

SPM tool box for


## ANALYSIS: Resting state (   ???   )




I know almost nothing about resting state but I have been told [this site](http://rfmri.org/) is worth having a look at.
* [Course/Tutorials](http://rfmri.org/Course)
* Tools (   ???   )

fmridenoise
neuropycon

## Diffusion weighted imaging
https://www.kaggle.com/chrisfilo/diffusion-weighted-imaging-dwi-analysis-with-dipy#



## ANALYSIS: Model selection (   ???   )




[Analytical flexibility](http://blogs.discovermagazine.com/neuroskeptic/2012/06/30/false-positive-neuroscience/) is a big [problem in neuroimaging](http://blogs.discovermagazine.com/neuroskeptic/2012/10/14/more-on-false-positive-neuroimaging/) most likely the source of a lot of false positive results.



If several analysis are attempted it can be good to have ways to decide amongst them. There is bad way to do like the one described in the [overfitting toolbox](https://www.researchgate.net/publication/319208937_The_Overfitting_Toolbox_TOT_Large-Scale_Search_in_Model_Space_for_Expected_Neuroimaging_Effects).

But there are better ways to do it:
* The [MACS](https://github.com/JoramSoch/MACS) SPM toolbox by [Joram Soch](https://twitter.com/JoramSoch)
* (   ???   )




## ANALYSIS: Statistical inferences and multiple comparison correction (MCP) (   ???   )


the salmon
http://neuroskeptic.blogspot.com/2009/09/fmri-gets-slap-in-face-with-dead-fish.html

imager's fallacy
http://blog.efpsa.org/2014/12/17/a-psychologists-guide-to-reading-a-neuroimaging-paper/

All Resolution Inference: Increasing Spatial Specificity of fMRI with Valid Circular Inference
https://www.pathlms.com/ohbm/courses/8246/sections/12541/video_presentations/115959


http://blogs.discovermagazine.com/neuroskeptic/2011/09/11/neuroscience-fails-stats-101/



### Cluster based inference (   ???   )


[Probabilistic Treshold-free Cluster Enhancement](https://spisakt.github.io/pTFCE/)
pTFCE (probabilistic TFCE) is a cluster-enahncement method to improve detectability of neuroimaging signal. It performs topology-based belief boosting by integrating cluster information into voxel-wise statistical inference.

### Family wise error (FWE) (   ???   )




In case you do not remember how random field theory works to correct for multiple comparison, [check this](http://imaging.mrc-cbu.cam.ac.uk/imaging/PrinciplesRandomFields).




### False discovery rate (FDR) (   ???   )

https://brainder.org/2011/09/05/fdr-corrected-fdr-adjusted-p-values/#comment-15388


### Permutation tests (   ???   )

[A primer on permutation testing (not only) for MVPA](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116074) by [Carsten Allefeld](https://twitter.com/c_allefeld) (36 min)


The [prevalence test](https://github.com/allefeld/prevalence-permutation)




#### SnPM (   ???   )
* [website](https://warwick.ac.uk/fac/sci/statistics/staff/academic-research/nichols/software/snpm)

#### FSL PALM and Randomize(   ???   )

#### Freesurfer PALM (   ???   )



## ANALYSIS: Multivariate analysis (   ???   )

http://blogs.discovermagazine.com/neuroskeptic/2014/06/21/fmri-mvpa-crack-neural-code/

https://distill.pub/2016/misread-tsne/

* [Jo Etzel](https://twitter.com/JosetAEtzel) has a great blog if you want to know more about multivariate analysis: [MVPA meandering](http://mvpa.blogspot.co.uk)

[Cross-validation : what, which and how?](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116075) by [Pradeep Reedy Raamana](https://twitter.com/raamana_) at OHBM 2018 (30 min)


What can we say about weight maps from linear decoding models?
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116081

Neuroimaging toolboxes for representation similarity analysis (RSA), support vector machine (SVM) and others...




### Matlab based

![Language](https://img.shields.io/badge/Language-Matlab-orange.svg)

#### TDT
TDT is the The Decoding Toolbox.
* [website](https://sites.google.com/site/tdtdecodingtoolbox/)

#### ProNTo
PRoNTo is the Pattern Recognition for Neuroimaging Toolbox developed at UCL (UK).
* [website](http://www.mlnl.cs.ucl.ac.uk/pronto/prtsoftware.html)
* [manual](http://www.mlnl.cs.ucl.ac.uk/pronto/prtdocs.html)
* [course/tutorial](http://www.mlnl.cs.ucl.ac.uk/pronto/prtcourses.html)

#### RSA toolbox
* [website](https://github.com/rsagroup/rsatoolbox)
* [manual](https://github.com/rsagroup/rsatoolbox/blob/develop/Documentation/toolbox%20documentation.pdf)

#### PCM toolbox
The pattern components modelling toolbox of the [Diedrichsen lab](https://twitter.com/diedrichsenlab)
* [website](https://github.com/jdiedrichsen/pcm_toolbox)
* [manual](https://github.com/jdiedrichsen/pcm_toolbox/blob/master/documentation/pcm_toolbox_manual.pdf)

#### cvMANOVA
From [Carsten Allefeld](https://twitter.com/c_allefeld)
* [website](https://github.com/allefeld/cvmanova)


### Python based

![Language](https://img.shields.io/badge/Language-Python-blue.svg)

#### pyMVPA
Intended to ease statistical learning analyses of large datasets.
* [website](http://www.pymvpa.org/)
* [manual](http://www.pymvpa.org/docoverview.html)
* [course/tutorial](http://www.pymvpa.org/tutorial.html)

#### nilearn
Nilearn is a Python module for fast and easy statistical learning on NeuroImaging data.
* [website](http://nilearn.github.io/)
* [manual](http://nilearn.github.io/user_guide.html)
* [course/tutorial](http://nilearn.github.io/introduction.html#python-for-neuroimaging-a-quick-start)


### R based (   ???   )



## ANALYSIS: Encoding models (   ???   )

https://nikokriegeskorte.org/tag/encoding-models/

#### Popeye
Python based pRF analysis.
* [website]https://popeye.readthedocs.io/en/latest/index.html)

#### SAMSRF
A pRF analysis toolbox called the Seriously Annoying Matlab SuRFer from [Sam Schwarzkopf](https://twitter.com/sampendu).
* [website](https://sampendu.net/seriously-annoying-matlab-surfer/)

## ANALYSIS: Robustness checks

Non neuroimaging cases
* [multiverse analysis]()
* [specification curves]() presented in a talk at SPSP [here](https://www.youtube.com/watch?v=g75jstZidX0
* vibration of effects

## ANALYSIS: Computational neuroscience



This [paper](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5230746/) comes with [some material](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005142#sec011) to apply bayesian decoding analysis to neuronal data can be of interest.



### Free energy

As someone said on twitter there is a cottage industry of blog posts trying to understand/explain this:
* https://medium.com/@solopchuk/intuitions-on-predictive-coding-and-the-free-energy-principle-3fc5bcedc754
* http://romainbrette.fr/what-is-computational-neuroscience-xxix-the-free-energy-principle/
* https://kaiu.me/2017/06/23/deep-active-inference-for-artificial-general-intelligence/
* http://slatestarcodex.com/2018/03/04/god-help-us-lets-try-to-understand-friston-on-free-energy
* http://www.aliannajmaren.com/2017/07/27/how-to-read-karl-friston-in-the-original-greek/


And a [tutorial](https://medium.com/@solopchuk/tutorial-on-active-inference-30edcf50f5dc)

### Dynamic causal modelling
[A tutorial series on DCM](https://www.youtube.com/watch?v=q-yypnHgCII&list=PLwiAO9Cs0Tb8wUGAnYY5yIMckB9tc4T3_) by [Kevin Aquino](https://twitter.com/kevin_m_aquino) [6 hrs]



## ANALYSIS: Laminar and high-resolution MRI
[Renzo Hubert](https://twitter.com/layerfmri) is keeping track of the most recent development of laminar MRI via twitter but also on his [blog](https://layerfmri.com/). He also curates laminar-fMRI related talks on his [Youtube channel](https://www.youtube.com/channel/UCMjtQ3FD41pAh1VJz-UZGJQ/videos) or papers in this [google spreahsheet](https://docs.google.com/spreadsheets/d/1DFdXA98bYPzK5Gf0M_PbNu3opvO-DIcrv7TMP5ywTMk/edit#gid=0).

* This [blog post](https://layerfmri.com/2018/01/04/layer-fmri-software-in-the-field/) has a list of most of the softwares that are related to laminar fMRI.
* A [more recent tool](https://github.com/kwagstyl/surface_tools) not listed in there for creating equivolumetric surfaces.

In terms of functional data there is high-res VASO (CBV) dataset [here](https://openneuro.org/datasets/ds001547).

For anatomical data you can have a look [here](   ???   ).

BID conference

## ANALYSIS: Meta analysis (   ???   )




* A [talk](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116072) by [Tom Nichols](https://twitter.com/ten_photos) at OHBM 2018 for an [overview](https://figshare.com/articles/Overview_of_Meta-Analysis_Approaches/6723839)
* A [practical](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116073) by [Camille Maumet](https://twitter.com/cmaumet) at OHBM 2018 on meta-analysis: [slides] (   ???   )
* A talk on ALE and brainmap
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116066


[NiMARE](https://github.com/neurostuff/NiMARE) is a Python library for coordinate- and image-based meta-analysis. [Chris Gorgolewski](https://twitter.com/ChrisFiloG) wrote a [tutorial](https://www.kaggle.com/chrisfilo/coordinate-and-image-metaanalysis-with-nimare) on how to use it.

https://github.com/NeuroVault/metanalysis_examples

For coordinate based meta-analysis:
* [brainmap](http://www.brainmap.org/) with [Sleuth](http://www.brainmap.org/software.html#Sleuth) and [GingerALE](http://www.brainmap.org/software.html#GingerALE)


For image based meta-analysis:
* [IBMA](https://github.com/NeuroimagingMetaAnalysis/ibma) is the Image-Based Meta-Analysis toolbox for SPM.




## REPORTING METHODS AND RESULTS (also useful for reviewing papers)


### A checklist: COBIDAS report
The organization from human brain mapping (OHBM) created the Committee on Best practices In Data Analysis and Sharing (COBIDAS) that published a report with a set of [guidelines](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5685169/) with an appended [checklist](https://www.biorxiv.org/content/early/2016/07/10/054262.full.pdf+html) on how to conduct and report fMRI studies. It is a very useful resource to use to make sure you are not forgetting anything when writing up your article.
See also Jeanette Mumford's [video](https://www.youtube.com/watch?v=bsM4KowO5Vc) about it.




* Journal specific requirements or checklists like those of Nature (   ???   ) or Elife (   ???   )
* [21 words solution] (   ???   )
* [Constraints on generality] (   ???   )
* Other checklists:
  - [here](http://biostat.mc.vanderbilt.edu/wiki/Main/ManuscriptChecklist)
  - http://jonathanpeelle.net/blog/2016/3/23/a-manuscript-checklist-for-improving-science





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
  - color blind friendly
  - the JET colormap is EVIL
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
