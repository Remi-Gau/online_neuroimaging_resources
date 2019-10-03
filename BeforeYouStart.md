# BEFORE YOU START

<!-- TOC -->

- [BEFORE YOU START](#before-you-start)
  - [Reproducibility (   ???   )](#reproducibility-------)
  - [Ethics and consent forms](#ethics-and-consent-forms)
  - [Code and data management (   ???   )](#code-and-data-management-------)
    - [Code management](#code-management)
      - [Version control](#version-control)
      - [Coding style](#coding-style)
      - [Avoid selective debugging: unit tests, positive and negative control](#avoid-selective-debugging-unit-tests-positive-and-negative-control)
    - [Data: BIDS, Datalad and YODA](#data-bids-datalad-and-yoda)
      - [BIDS](#bids)
      - [Datalad](#datalad)
      - [YODA](#yoda)
  - [Documentation (   ???   )](#documentation-------)

<!-- /TOC -->

## Reproducibility (   ???   )

* [Neuroimaging Workflows & Statistics for reproducibility](https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/115885) by Dorota Jarecka, Satrajit Ghosh, Celia Greenwood and Jean-Baptiste Poline at OHBM (3 hr 45 min)

http://blogs.discovermagazine.com/neuroskeptic/2012/06/14/brains-are-different-on-macs/

Same Data - Different Software - Different Results? Analytic Variability of Group fMRI Results.
https://www.pathlms.com/ohbm/courses/8246/sections/12541/video_presentations/116000


There are a few options you can investigate to make your analysis more replicable and reproducible. On top of [sharing your data and your code](#Sharing-your-code, data-and-your-results) you can use containers like [docker](https://www.docker.com/) or singularity that allows you to run your analysis in contained environment that has an operating system, the software you need and all their dependencies.

In practice this means that by using this container:
* other researchers can reproduce your analysis **now** on their computer (e.g you can run a linux container with freesurfer on your windows computer),
* you can reproduce your own analysis **in 5 years** from now without facing the problem of knowing which version of the software you used.

If you want a brief conceptual introduction to containers and to the difference between containers and virtual machine, I recommend you start with these 2 posts:
https://towardsdatascience.com/learn-enough-docker-to-be-useful-b7ba70caeb4b
https://medium.freecodecamp.org/a-beginner-friendly-introduction-to-containers-vms-and-docker-79a9e3e119b

[Neurodocker](https://github.com/kaczmarj/neurodocker) allows you to easily create a docker container suited to your needs in terms of neuroimaging analysis. There is nice [tutorial](https://miykael.github.io/nipype_tutorial/notebooks/introduction_neurodocker.html) here on how to use it.

[Code-ocean](https://codeocean.com/) is web based service that relies on docker containers to let you run your analysis online. There is [post](https://www.fmrwhy.com/2018/10/31/reproducible-fmri-codeocean/) by [Stephan Heunis](https://twitter.com/fmrwhy) describing how he did that with an SPM pipeline.

Another thing you can implement is using notebooks like [jupyter](http://jupyter.org/), [jupyter lab](https://jupyterlab.readthedocs.io/en/stable/) or [binder](https://mybinder.org/) (   ???   ). Here is fascinating [talk](https://www.youtube.com/watch?v=zC-3sdPtb0w&list=PLO3l0PnUGHYEqA7rFQT2jM6jxsaC2XiHh&t=384s&index=19) by [Fernando Perez](https://twitter.com/fperez_org), one the person behind the jupyter project.


Neuroimaging Workflows & Statistics for reproducibility
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/115885
Neuroinformatics and Replication: beyond BASH scripts and winner’s curses
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116085
Introduction to reproducible neuroimaging
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/115884
Reproducibility and replicability: a practical approach
https://www.pathlms.com/ohbm/courses/8246/sections/12538/video_presentations/116214


## Ethics and consent forms
The [open brain consent form](https://open-brain-consent.readthedocs.io/en/stable/) tries to facilitate neuroimaging data sharing by providing an “out of the box” solution addressing human subjects concerns and consisting of
* widely acceptable consent form allowing deposition of anonymized data to public data archives
* collection of tools/pipelines to help anonymization of neuroimaging data making it ready for sharing



LICENSES : to help you which license to choose start [here](https://choosealicense.com/)

Lincenses don't apply to data

https://gist.github.com/lukas-h/2a5d00690736b4c3a7ba


## Code and data management (   ???   )
In general I suggest you have a look at some of the courses and material offered by the Carpentries for [data](https://datacarpentry.org/) and [code](https://software-carpentry.org/).


http://nikola.me/folder_structure.html
https://drivendata.github.io/cookiecutter-data-science/

### Code management

#### Version control
For managing your code, if you don't already, I suggest you make version control with [GIT](https://git-scm.com/) part of every day your every day workflow. GIT might seem scary and confusing at first but it is well worth the effort: the good news is that there are plenty of tutorials available (for example: [here](http://swcarpentry.github.io/git-novice/), [there](https://www.codecademy.com/learn/learn-git) or [there](https://www.youtube.com/playlist?list=PL0lo9MOBetEHhfG9vJzVCTiDYcbhAiEqL)). Another advantage of using GIT is that it allows you to collaborate on many projects on [github](https://github.com) but which already makes a lot of sense even simply [at the scale of a lab](https://ourcodingclub.github.io/2017/05/15/git-for-labs.html).

Even though GIT is most powerful when using the command line, there are also many [graphic interfaces](https://git-scm.com/downloads/guis/) that might just be enough for what you need. Plus the graphic interface can help you get started to then you move on to use the command line only. There is no shame in using a GUI: just don't tell the GIT purists this is what you do otherwise you will never hear the end of it.

https://medium.freecodecamp.org/how-to-use-badges-to-stop-feeling-like-a-noob-d4e6600d37d2

https://lgatto.github.io/github-intro/

#### Coding style
Another good coding practice to have is a consistent coding style. For python you have the [PEP8 standard](https://www.python.org/dev/peps/pep-0008/) and some tools like [pylint](https://www.pylint.org/), [pycodestyle](https://pypi.org/project/pycodestyle/2.2.0/), or [pep8online](http://pep8online.com/) that help you make sure that your code complies with this standard.

https://github.com/ambv/black

You can also have a look at the code style used by [google for many languages](https://github.com/google/styleguide) (h/t [Kelly Garner](@garner_theory)). You will notice that matlab is not in the list so you might want to check this [here](https://fr.mathworks.com/matlabcentral/fileexchange/46056-matlab-style-guidelines-2-0?s_tid=mwa_osa_a).
http://sci-hub.tw/https://www.cambridge.org/core/books/elements-of-matlab-style/8825411CE69013434DB0939780CFD907

mlint and checkcode
https://fr.mathworks.com/help/matlab/ref/mlint.html
https://fr.mathworks.com/help/matlab/ref/checkcode.html
https://blogs.mathworks.com/community/2008/09/08/let-m-lint-help-simplify-your-code/

https://arstechnica.com/information-technology/2012/08/ive-inherited-200k-lines-of-spaghetti-codewhat-now/

https://refactoring.com/

#### Avoid selective debugging: unit tests, positive and negative control

https://www.software.ac.uk/

Having a bug is annoying. Having your code run but give you an obviously wrong answer is more annoying. Having your code run and give you a plausible but wrong answer is scary (and potentially expensive when it [crashes a spaceship onto a planet](https://en.wikipedia.org/wiki/Mars_Climate_Orbiter#Cause_of_failure)). Having your code run and give you the answer you want but not the true answer is the worst and keeps me up at night.

Selective debugging happens when we don't check the code that gives us the answer we want but we do check it when it gives us an answer that goes against our expectation. In a way it is a quite insidious form of p-hacking.

There are some [recent](http://blogs.discovermagazine.com/neuroskeptic/2016/08/21/software-errors-in-fmri/#.V8B1vZ7TU-i) [examples](http://www.russpoldrack.org/2013/02/anatomy-of-coding-error.html) in [neuroimaging](http://the-brain-box.blogspot.com/2013/02/biased-debugging.html).

Some things that can be done about it:
- organize code reviews in your lab: basically make sure that the code has been checked by another person. Pairing a beginner with a more senior member of the lab can also be a way to improve learning and skill transfer in the lab.
- [test your code](http://www.reproducibleimaging.org/module-dataprocessing/06-testing/). These tests can be implemented automatically to your project by continuous integration services like [Travis](https://travis-ci.org/).
- test your pipeline with positive negative control. A negative control is testing your analysis by running on random noise or on data that should have no signal in it. The latter was the approach used by [Anders Eklund](https://twitter.com/wandedob) and [Tom Nichols](https://twitter.com/ten_photos) in their [cluster failure paper series](http://blogs.discovermagazine.com/neuroskeptic/2018/07/22/cluster-failure-revisited/). A positive control is making sure that your analysis can detect VERY obvious things it should detect (e.g motor cortex activation following button presses, classify responses to auditory versus visual stimuli in V1, …). [Jo Etzel](https://twitter.com/JosetAEtzel) has post about [this](https://mvpa.blogspot.com/2015/11/positive-control-analyses-and-checking.html).



https://jupyter4edu.github.io/jupyter-edu-book/


### Data: BIDS, Datalad and YODA

#### BIDS
If you are going to do some fMRI analysis you will quickly drown in data if you are not a bit organized, so I highly recommend you use the brain imaging data structure standard ([BIDS](http://bids.neuroimaging.io/)) to organize your data. The current version of BIDS only talks about raw data but it should soon cover derivatives (e.g preprocessed data). In general BIDS also allows you to more easily share your data and use plenty of analytical [tools](bids-apps.neuroimaging.io/apps/).

If you would like to use BIDS but you have no idea what a JSON file or the length of the specification document scares you, head over to the [BIDS starter kit](https://github.com/bids-standard/bids-starter-kit) to find tutorials and scripts to help you rearrange your data.

#### Datalad
[Datalad](https://www.datalad.org/for/data-consumers) is to data what git is to code. It allows curation of data and version controlling of but also lets you crawl databases to explore and download data from them and it facilitates data sharing. Several of these features are described [here](https://www.datalad.org/features.html) with scripts that act as tutorial. There are videos presentation of it [there](https://www.youtube.com/watch?v=59CE6iOr45k).

#### YODA
Having a standard way to organize not only your data but also your code, the results, the documentation... from the beginning of a project can go a long way to save you a lot of time down the line (when communicating within or outside your lab, or when you have to wrap things up when moving to a new project/job). The [YODA template](https://github.com/myyoda/template) is folder structure recommended by [ReproNim](http://www.reproducibleimaging.org/index.html) that you can use.

https://eglerean.wordpress.com/2017/05/24/project-management-data-management/

Other good habits:
* a simple, transparent and systematic filenaming is a good [start](https://www.google.fr/search?q=good+file+naming+conventions&rlz=1C1CHBD_en-GBGB758GB758&oq=good+filenaming+&aqs=chrome.1.69i57j0l3j69i64.6421j0j7&sourceid=chrome&ie=UTF-8)
* if you have to deal with data in spreadsheet I think you will enjoy [this paper](https://www.tandfonline.com/doi/full/10.1080/00031305.2017.1375989) and this [cookbook](https://www.polydesmida.info/cookbook/)

BIDS equivalent for psych data in general
https://medium.freecodecamp.org/10-common-data-structures-explained-with-videos-exercises-aaff6c06fb2b

## Documentation (   ???   )
It is often said to:
> Always code as if the person who ends up maintaining your code is a violent psychopath who knows where you live.

Proper documentation of a project and good commenting of your code will help others to use it or pick it up later. But there are good selfish reasons to document your project and comment your code: it will most likely help future you when you have to respond to reviewers or when you want to check something in that data set or in that function you used 6 months ago.

>- Most likely, you will have to re-run your analysis more than once.
>- In the future, you or a collaborator may have to re-visit part of the project.
>- Your most likely collaborator is your future self, and your past self doesn’t answer emails.

See [here](http://bioconnector.github.io/bims8382/r-repres.html) for more.

There are plenty of recommendations out there about writing documentation. I did find [this one](https://www.divio.com/blog/documentation/) useful and this [list](https://github.com/matiassingers/awesome-readme#tools) or this [checklist](https://github.com/Remi-Gau/readme-checklist) that are more specific to README files.

In terms of code I guess the ideal is [self-documenting code](http://wiki.c2.com/?SelfDocumentingCode). [Read the docs](https://readthedocs.org/) is a good option that also allows for continuous integration.  Python also apparently has this thing called [Sphinx](http://www.sphinx-doc.org/en/master/) that helps *create intelligent and beautiful documentation* (that alone should make matlab users envious). There are also ways to make it part of a [continuous integration](https://predictablynoisy.com/circle-documentation-build).
