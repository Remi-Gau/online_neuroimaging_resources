# Online courses

<!-- TOC -->

- [Online courses](#online-courses)
  - [Math and linear algebra courses](#math-and-linear-algebra-courses)
  - [MRI courses (   ???   )](#mri-courses-------)
  - [fMRI courses (   ???   )](#fmri-courses-------)
  - [Machine learning (   ???   )](#machine-learning-------)
  - [Resting state courses (   ???   )](#resting-state-courses-------)
  - [Neurohackademy](#neurohackademy)
  - [Software specific (   ???   )](#software-specific-------)
    - [SPM](#spm)
    - [Freesurfer](#freesurfer)
    - [FSL](#fsl)
    - [AFNI](#afni)
    - [Nipype](#nipype)
    - [MIPAV](#mipav)
    - [Others (   ???   )](#others-------)
  - [Statistics courses](#statistics-courses)
  - [Open-science and reproducibility](#open-science-and-reproducibility)

<!-- /TOC -->

## Math and linear algebra courses

Khan Academy is a great free resource for all sorts of topics.
*   Their series on [linear algebra](https://www.khanacademy.org/math/linear-algebra) is particularly useful and relevant to our needs.
*   The Fourier [series](https://www.khanacademy.org/science/electrical-engineering/ee-signals/ee-fourier-series/v/ee-fourier-series-intro) and the
*   [statistics one](https://www.khanacademy.org/math/statistics-probability) videos may also prove useful (h/t [Sam Jones] (   ???   ) ).

If you feel that your background in mathematics and signal processing is a bit weak please have a look at [these slides](https://figshare.com/s/be5a73a1e0a31fb9b6ed). This file was put together by [Joana Leitao](https://twitter.com/JoanaLeitao8) and covers several topics that are important to be familiar with in neuroimaging:
*   basic linear algebra
*   ordinary least square solution for the general linear model
*   the BOLD response and convolution: what is a linear time invariant system and why is matters when doing a fMRI study ?
*   how to do t-test and ANOVAS within a general linear model

## MRI courses (   ???   )
If you need to dust up your knowledge about MRI.
*   the [e-MRI course]([https://www.imaios.com/en/e-Courses/e-MRI)
*   [MRI fundamentals](https://www.coursera.org/learn/mri-fundamentals) on coursera
*   A [Magnetic Resonance Imaging Lab](https://cfmriweb.ucsd.edu/ecwong/BE278W14.html) from UCSD
*   [MRI question](http://mriquestions.com/how-does-fmri-work.html) is not a course but a VERY VERY comprehensive FAQ on MRI.

There are also blog posts series on [practicalfmri](http://practicalfmri.blogspot.co.uk) (and on its companion winnower account) that cover
*   [the physics of fMRI artefacts](https://practicalfmri.blogspot.com/2012/02/physics-for-understanding-fmri.html)
*   the type of [artefacts](https://practicalfmri.blogspot.com/2012/09/understanding-fmri-artifacts-contents.html) you might encounter and what to look for
*   a list of potential confounds to the [BOLD signal](https://thewinnower.com/papers/concomitant-physiologic-changes-as-potential-confounds-for-bold-based-fmri-a-checklist)
*   [quality control on MRI and fMRI](https://practicalfmri.blogspot.com/2014/08/qa-for-fmri-part-3-facility-qa-what-to.html)
*   the [Braindr web app](https://braindr.us/#/) designed by [Anisha Keshavan](https://anisha.pizza/#/projects) to expose yourself to some good, bad and ugly MRI structural images

http://the-brain-box.blogspot.com/2015/05/what-does-fmri-measure.html
http://blogs.discovermagazine.com/neuroskeptic/2014/02/03/non-bold-signal-fmri/#.UwNqBdvxBXT
Matthias Nau [???] EPI guide  https://matthiasnau.com/epi_guide.pdf

## fMRI courses (   ???   )
There are quite a few courses for fMRI analysis out there that I am aware of.
*   On coursera
A few courses on [coursera](https://www.coursera.org/courses?query=mri) with notably
 -   [Tor Wager's](https://twitter.com/torwager) and Martin Lindquist's 2 parts MOOC ([part 1](https://en.coursera.org/learn/functional-mri)
 and [part 2](https://en.coursera.org/learn/functional-mri-2))
 -   and the [Introduction to Neurohacking In R](https://www.coursera.org/learn/neurohacking)
*   Others
   -   the [fMRI Image Acquisition and Analyses course](https://www.mrn.org/education-outreach/courses-and-events) from the mind research network is an IRL course but links to useful resources too
   -   the [functional MRI methods - psych 214](https://bic-berkeley.github.io/psych-214-fall-2016/) from Berkeley


## Machine learning (   ???   )
If you are going to do some multivariate analysis, it is likely you will need to know a ~~bit~~ lot of machine learning. I did find that that [this class](https://www.coursera.org/learn/machine-learning) on coursera covered a lot of ground. It is not specific to neuroimaging but gives you a good overview of the basic concept you need to understand.

Worst case it will let you understand [why John von Neumann said](https://www.johndcook.com/blog/2011/06/21/how-to-fit-an-elephant/)
> With four parameters I can fit an elephant, and with five I can make him wiggle his trunk.

https://fmrif.nimh.nih.gov/public/other-courses/mvpa
https://dartbrains.org/intro.html


## Resting state courses (   ???   )
There is one on the rMRI [website](http://rfmri.org/Course).


## Neurohackademy
[Neurohackademy](https://neurohackademy.org/) is more than a neuroimaging course: it is broader in scope as it covers reproducibility and open science issues in neuroimaging. It is also very practical and definitely python oriented. To know more, see this [post](http://www.talyarkoni.org/blog/2018/08/16/neurohackademy-2018-a-wrap-up/) by [Tal Yarkoni](https://twitter.com/talyarkoni) about the 2018 edition of Neurohackademy.
* [videos to the edition 2017/2018](https://www.youtube.com/playlist?list=PLA6PlfxWZPLTLJ2qTN9enG0tkizpmwWaq)
* [videos to the edition 2016](https://www.youtube.com/playlist?list=PLEdFhTRBFLObkatJOX9wp3BCueH4wNSl7)
* [2018 course material](https://github.com/neurohackademy)


## Software specific (   ???   )
Most of the main analysis packages on top of the IRL courses usually have one video series that works as a course +/- tutorial.

### SPM
* [website](https://www.fil.ion.ucl.ac.uk/spm/)
* [manual](https://www.fil.ion.ucl.ac.uk/spm/doc/)
* [mailing list](https://www.fil.ion.ucl.ac.uk/spm/support/)
* [course/tutorial](http://www.fil.ion.ucl.ac.uk/spm/course/)

### Freesurfer
* [website](https://surfer.nmr.mgh.harvard.edu/)
* [manual](https://surfer.nmr.mgh.harvard.edu/fswiki)
* [mailing list](https://surfer.nmr.mgh.harvard.edu/fswiki/FreeSurferSupport)
* [course](https://www.youtube.com/channel/UCruQerP8aa-gYttXkAcyveA) and [videos](https://surfer.nmr.mgh.harvard.edu/fswiki/CourseDescription)

### FSL
* [website](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki)
* [manual](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/Support)
* [mailing list](https://www.jiscmail.ac.uk/cgi-bin/webadmin?A0=fsl)
* [course/tutorial](https://fsl.fmrib.ox.ac.uk/fslcourse/)

### AFNI
* [website](https://afni.nimh.nih.gov/)
* [manual](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/index.html)
* [mailing list](https://afni.nimh.nih.gov/afni/community/board/list.php?1)
* [course/tutorial]: Video recordings from the [AFNI bootcamp](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/educational/bootcamp_recordings.html), with slides, and [example data](https://afni.nimh.nih.gov/pub/dist/doc/htmldoc/background_install/unix_tutorial/misc/install.data.html).

### Nipype
Nipype is best viewed as a way to create and run software-agnostic preprocessing/analysis-pipeline. It becomes very powerful when you need to use different softwares in your analysis.
* [website](https://nipype.readthedocs.io/en/latest/)
* [manual](https://nipype.readthedocs.io/en/latest/documentation.html)
* [course/tutorial](https://miykael.github.io/nipype_tutorial/)

[Tim Van Mourik](https://twitter.com/tim_van_mourik) and a few other people have developed tool to facilitate building pipelines with nipype:
* [Porcupine](https://timvanmourik.github.io/Porcupine/) stands for "PORcupine Creates Ur PipelINE" which is probably *the worst recursive acronym with bad capitalisation and annoying use of slang*. This software allows researchers to build pipelines using a GUI and generates the code that is needed to run the pipeline created.
* [Giraffe](https://giraffe.tools/porcupine) is web-based "Graphical Interface for Reproducible Analysis oF workFlow Experiments" that can take advantage of Porcupine to create pipelines.

### MIPAV

### Others (   ???   )

http://www.fmri4newbies.com/


## Statistics courses
Some of those are clearly not specific to neuroimaging but are well worth going through even if you are a PI.

* If you have no idea what the distribution of p-value would look like if there were only noise in your data, then the odds are you will learn at least one thing in [Daniel Lakens](https://twitter.com/lakens) course on [how to improve your statistical inferences](https://www.coursera.org/learn/statistical-inferences). Most likely you will learn more than one thing.

Daniel also has a blog [blog](http://daniellakens.blogspot.com/) is very useful of stats related knowledge. Similarly [Guillaumme Rousselet's](https://twitter.com/robustgar) has a series of posts on his [blog](https://garstats.wordpress.com/) where you learn more about robust statistics and how to improve your data visualizations.

## Open-science and reproducibility
There is a [MOOC on open-science](https://opensciencemooc.eu/) is still under construction but on top of an insane [list of resources](https://opensciencemooc.eu/resources/) has the [module 5](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/tree/master/content_development) already up and running to teach you how to use github and zenodo to create a time stamped screenshot of your code to link to in your papers.

[Stat 159/259 - Reproducible and Collaborative Data Science](https://berkeley-stat159-f17.github.io/stat159-f17/) from Berkeley has a hands-on and integrated approach to GIT, jupyter notebooks, Python and more...
