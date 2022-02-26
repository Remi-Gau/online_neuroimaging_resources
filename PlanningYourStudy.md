# PLANNING YOUR STUDY

- [PLANNING YOUR STUDY](#planning-your-study)
  - [Reusing data](#reusing-data)
  - [Defining your terms and your task](#defining-your-terms-and-your-task)
  - [Ontologies](#ontologies)
  - [Piloting ( ??? )](#piloting---)
  - [Optimizing your design](#optimizing-your-design)
  - [Design efficiency ( ??? )](#design-efficiency---)
  - [Power](#power)
  - [For MVPA: same analysis approach](#for-mvpa-same-analysis-approach)
  - [Defining your region of interest ( ??? )](#defining-your-region-of-interest---)
  - [Using previous results ( ??? )](#using-previous-results---)
  - [Localizers ( ??? )](#localizers---)
  - [Atlases](#atlases)
  - [Non-standard templates ( ??? )](#non-standard-templates---)

## Reusing data

Some of the main databases are:

- [Pain repository](https://www.painrepository.org/])

But there are [many](https://brainhack101.github.io/neurolinks/)
[possibilities](https://en.wikipedia.org/wiki/List_of_neuroscience_databases)
[of](https://www.nitrc.org/search/?type_of_search=group&rows=20&s=relevancy&cat=325%3AData)
[databases](https://www.nitrc.org/search/?type_of_search=group&offset=0&removeterm=&cat=313%3ADatabase&compare=&q=&rows=20&s=relevancy&file=%2Ffrs%2Fdownloadlink.php%2F9275&file=%2Ffrs%2Fdownloadlink.php%2F9336&file=%2Ffrs%2Fdownloadlink.php%2F3981&file=%2Ffrs%2Fdownload.php%2F9300%2Fdti_atlas.nrrd&file=%2Ffrs%2Fdownload.php%2F6716%2F3DMetricTools1.4.3-Windows.tar&file=%2Ffrs%2Fdownloadlink.php%2F5884&file=%2Ffrs%2Fdownload.php%2F860%2FLesionSegmentationTutorialData.tgz&file=%2Ffrs%2Fdownloadlink.php%2F10354&file=%2Ffrs%2Fdownload.php%2F7345%2FCONFREP_new_bvecs.zip&file=%2Ffrs%2Fdownload.php%2F5348%2FDemoData.zip&file=%2Ffrs%2Fdownload.php%2F10036%2F7T3T_NITRC.tar.gz&file=%2Ffrs%2Fdownloadlink.php%2F6725&file=%2Ffrs%2Fdownload.php%2F9277%2FLC_prob_atlas_mni05.zip&file=%2Ffrs%2Fdownloadlink.php%2F4074&file=%2Ffrs%2Fdownload.php%2F4969%2FaBEAT.zip&xrowsx=20&s=relevancy)
where you can find your raw and/or pre-processed data. Maybe your university or
your institute already ahs a repository of published data (e.g the
[Donders institute](https://data.donders.ru.nl/?0).

Chris Madan also has a nice
[Curated list of open-access databases with human structural MRI data](https://github.com/cMadan/openMorph)

[A list of brain imaging databases with multiple scans per subject](https://github.com/Conxz/multiBrain)
put together by Xiangzhen Kong

The recent
[google extension for databases](https://toolbox.google.com/datasetsearch) can
also be useful to locate datasets that might be of interest.

There are some tools that help you search through them like the metasearch tool
on the [Open Neuroimaging Laboratory](http://openneu.ro) but this is also where
[Datalad](#datalad) can become useful to
[browse or crawl those databases](https://www.datalad.org/for/data-discovery).

Open science resources for neuroimaging research
https://www.pathlms.com/ohbm/courses/8246/sections/12542/video_presentations/116089

## Defining your terms and your task

## Ontologies

> Inigo Montoya: You keep using that word. I don't think it means what you think
> it means. Ayotnom Ogini: Funny you should say that! I was about to tell you
> the same thing.

The use of alternate and even competitive terminologies can often impede
scientific discoveries.

- [The cognitive atlas](http://www.cognitiveatlas.org/)
- [The cognitive paradigm ontology](http://www.cogpo.org/)

- If you are doing intervention based studies
  [Declare design](https://declaredesign.org/) seems to be something to look
  into. See what [Dorothy Bishop](https://twitter.com/deevybee) had to
  [say about it](http://discuss.declaredesign.org/t/gentle-introduction-to-declaredesign-by-dorothy-bishop/51/1).
- [flexible measures](http://www.flexiblemeasures.com/) by
  [Malte Elson](https://twitter.com/maltoesermalte). A
  [post](http://blogs.discovermagazine.com/neuroskeptic/2016/04/05/flexible-measures-science/)
  by [Neuroskeptic](https://twitter.com/Neuro_Skeptic) about it.

## Piloting ( ??? )

Good piloting is very important but piloting is not meant to be about finding a
hypothesis you want to test: because of the small sample size of pilot studies,
anything interesting you see there is very likely to be a fluke. Piloting is
more about checking the overall feasibility of that experiment and that you can
get high [quality data](#ONCE YOU-HAVE-DATA:-quality-control), judged by
criteria that are unrelated to your hypothesis.

[Sam Schwarzkopf](https://twitter.com/sampendu) has a few interesting posts on
the topic
[here](https://neuroneurotic.net/2016/08/29/on-the-worthlessness-of-inappropriate-piloting/)
and
[there](https://neuroneurotic.net/2016/08/30/on-the-magic-of-independent-piloting/)

Piloting is usually a phase where it would be good to check with your local MRI
physicist and statistician. And you also might already have to make choices
about [pre-processing](#ONCE-YOU-HAVE-DATA:-preprocessing) and data analysis.

## Optimizing your design

Before you run your study there are a few things you can do to
[optimize your design](http://mumfordbrainstats.tumblr.com/post/149759511091/designing-your-pre-fmri-behavioral-study).
Two of them are doing a power analysis and optimizing the efficiency of your
fMRI design.

## Design efficiency ( ??? )

If you need a reminder about what
[design efficiency](http://imaging.mrc-cbu.cam.ac.uk/imaging/DesignEfficiency)
is.

Jeanette Mumford has a good
[video series](https://www.youtube.com/playlist?list=PLB2iAtgpI4YEnBdb_jDGmMcdGoIBwhCCY)
about design efficiency and another
[standalone one](https://neurohackademy.org/course/efficiency-and-design-optimization-for-fmri/)
from Neurohackademy 2016.

When you want to optimize it you have few options:

- you can compute the efficiency by hand and tweaking your design
  [to see what options work best](http://imaging.mrc-cbu.cam.ac.uk/imaging/DesignEfficiency).
  There is a function available
  [Rik Henson's](https://github.com/MRC-CBU/riksneurotools) repo to help you do
  that.
- but there are also more systematic ways to optimize your protocol: see
  [here](http://surfer.nmr.mgh.harvard.edu/optseq/),
  [here](http://psych.colorado.edu/~tor/Software/genetic_algorithms.html) or
  [there](http://www.cabiatl.com/CABI/resources/fmrisim/)
- the latest tool for design efficiency calculation is the website
  [neuropowertools](http://www.neuropowertools.org/). It actually offers options
  to run both your design efficiency optimization and your power analysis. They
  also have their respective python packages.

## Power

> In order to investigate whether an effect exists, one should design an
> experiment that has a reasonable chance of detecting it. I take this insight
> as common sense. In statistical language, an experiment should have sufficient
> statistical power. Yet the null [hypothesis significant testing] ritual knows
> no statistical power.

Gerd Gigerenzer in _Statistical Rituals: The Replication Delusion and How We Got
There_,
[DOI: 10.1177/2515245918771329](http://journals.sagepub.com/doi/10.1177/2515245918771329)

There is good evidence that the average statistical power has remained low for
several decades in psychology which increases the false negative rate and
reduces the positive predictive value of findings (i.e the chance that a
significant finding is actually true). Maybe neuroimaging could learn from that
mistake, especially that a large majority of neuroimaging studies seem to have
even lower statistical power.

link to neuroskeptic on power failure:
http://blogs.discovermagazine.com/neuroskeptic/2017/07/19/neuroscience-underpowered/
http://blogs.discovermagazine.com/neuroskeptic/2013/08/10/is-neuroscience-too-small/

link to Tal's response to Friston

link to tal's paper on why small studies give big correlations

link to law of small numbers paper by kanheman

link to figures of scanning the horizon

Add output from SIPS hackathon

[fMRI power](http://fmripower.org/) is a matlab based toolbox to help you run
your power analysis.

The website [neuropowertools](http://www.neuropowertools.org/) actually offers
options to run both your design efficiency optimization and your power analysis.
They also have their respective python packages.

## For MVPA: same analysis approach

If you intend to run a MVPA - classification analysis on your data, there are a
few things you can do BEFORE you start collecting data to optimize your design.
There is no app/toolbox for that so I am afraid you will have to read the
[paper](https://arxiv.org/abs/1703.06670)

## Defining your region of interest ( ??? )

If you don't want to run a whole brain analysis, then you will most likely need
to define your regions of interest (ROI). This must be done using data that is
independent from the data you will use in the end otherwise you will have a
circularity problem (also known as double dipping or voodoo correlation).

- around a coordinate identified in a previous study or in a
  [meta-analysis](#meta-analysis-( ??? )), or by using Neurosynth.
- using a localizer
  https://github.com/search?l=&p=1&q=Localizer+fmri&ref=advsearch&type=Repositories&utf8=%E2%9C%93
  https://github.com/search?p=1&q=Retinotopy&type=Repositories&utf8=%E2%9C%93

- or relying on a functional or anatomical atlas.

Some blog posts related to voodoo correlations:

- http://neuroskeptic.blogspot.com/2009/02/voodoo-correlations-in-fmri-whose.html
- http://blogs.discovermagazine.com/neuroskeptic/2012/01/31/voodoo-neuroscience-revisited/
- http://blogs.discovermagazine.com/neuroskeptic/2010/04/30/new-voodoo-free-fmri-technique/
- https://neurocritic.blogspot.com/2009/01/voodoo-correlations-in-social.html

## Using previous results ( ??? )

[Neurosynth](http://neurosynth.org/) can help with to run a meta-analysis to
create mask to define your ROI. See for example
[this](http://neurosynth.org/analyses/terms/auditory/) if you wanted to have a
ROI for brain region matching the search term `auditory` and see here for a
[tutorial](http://nbviewer.jupyter.org/github/neurosynth/neurosynth/blob/master/examples/neurosynth_demo.ipynb).

google data search engine

## Localizers ( ??? )

A typical example of a localizer are retinotopic mappings.
[Sam Schwarzkopf](https://twitter.com/sampendu) has good
[tutorial](https://figshare.com/articles/Retinotopic_mapping_tutorial/1513839)
for those.

retinotopy

tonotopy

motion localizer

face localizer

## Atlases

There are many atlases you could use to create ROIS. Some ship automatically
with some softwares otherwise you can find lists on the

- [SPM website](https://en.wikibooks.org/wiki/SPM/Atlases)
- [FSL website](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/Atlases)
- [AFNI website](https://afni.nimh.nih.gov/Atlases_page)
- [CARET website](http://brainvis.wustl.edu/wiki/index.php/Caret:Atlases)
- [NITRC website](https://www.nitrc.org/search/?type_of_search=group&offset=0&removeterm=&cat=578%3AAtlas+Data&compare=&q=&rows=20&s=relevancy&file=%2Ffrs%2Fdownloadlink.php%2F9275&file=%2Ffrs%2Fdownloadlink.php%2F9336&file=%2Ffrs%2Fdownloadlink.php%2F3981&file=%2Ffrs%2Fdownload.php%2F9300%2Fdti_atlas.nrrd&file=%2Ffrs%2Fdownload.php%2F6716%2F3DMetricTools1.4.3-Windows.tar&file=%2Ffrs%2Fdownloadlink.php%2F5884&file=%2Ffrs%2Fdownload.php%2F860%2FLesionSegmentationTutorialData.tgz&file=%2Ffrs%2Fdownloadlink.php%2F10354&file=%2Ffrs%2Fdownload.php%2F7345%2FCONFREP_new_bvecs.zip&file=%2Ffrs%2Fdownload.php%2F5348%2FDemoData.zip&file=%2Ffrs%2Fdownload.php%2F10036%2F7T3T_NITRC.tar.gz&file=%2Ffrs%2Fdownloadlink.php%2F6725&file=%2Ffrs%2Fdownload.php%2F9277%2FLC_prob_atlas_mni05.zip&file=%2Ffrs%2Fdownloadlink.php%2F4074&file=%2Ffrs%2Fdownload.php%2F4969%2FaBEAT.zip&xrowsx=20&s=relevancy)

https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0007200#s4

http://nilearn.github.io/modules/reference.html#module-nilearn.datasets

Some other retinotopics maps are apparently not listed in the above so here they
are:

- An anatomical template of human striate retinotopy
  (https://cfn.upenn.edu/aguirre/wiki/public:data_currbio_2012_benson)
- The HCP 7T Retinotopy Dataset: data1(https://balsa.wustl.edu/study/show/9Zkk);
  [data2](https://osf.io/bw9ec/);
  [paper](https://www.biorxiv.org/content/early/2018/08/30/308247)
- Probabilistic Maps of Visual Topography in Human Cortex:
  [data](https://scholar.princeton.edu/napl/resources);
  [paper](https://www.ncbi.nlm.nih.gov/pubmed/25452571)

http://gallantlab.org/pycortex/retinotopy_demo/

The problem then becomes **which atlas to choose**. To help you with this the
[Online Brain Atlas Reconciliation](https://www.nitrc.org/projects/obart/) Tool
can show the overlap that exist between some of those atlases. The links I had
to the website ([here](http://qnl.bu.edu/obart) and
[there](http://www.braincircuits.org/human-brain)) are broken at the moment so
at least here is a link to the
[paper](https://www.ncbi.nlm.nih.gov/pubmed/19787067)

Some toolboxes out there also allow you to create your own ROI and rely on
anatomical / cytoarchitectonic atlases:

- [AAL toolbox](http://www.gin.cnrs.fr/en/tools/aal-aal2/)
- [anatomy toolbox](http://www.fz-juelich.de/inm/inm-1/DE/Forschung/_docs/SPMAnatomyToolbox/SPMAnatomyToolbox_node.html)
- [MarsBAR](http://marsbar.sourceforge.net/)

## Non-standard templates ( ??? )

In case you want to normalize brains of children it might be better to use a
pediatric template. Some of them are listed
[here](https://www.nitrc.org/search/?type_of_search=group&rows=20&s=relevancy&cat=578%3AAtlas+Data).
