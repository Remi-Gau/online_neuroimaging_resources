# REPORTING METHODS AND RESULTS

<!-- TOC -->

- [REPORTING METHODS AND RESULTS](#reporting-methods-and-results)
  - [A checklist: COBIDAS report](#a-checklist-cobidas-report)
  - [Percent signal change (   ???   )](#percent-signal-change-------)
  - [Making figures (   ???   )](#making-figures-------)
    - [Color maps](#color-maps)
  - [Tools to check results/statistics (   ???   )](#tools-to-check-resultsstatistics-------)
  - [Peer review (   ???   )](#peer-review-------)

<!-- /TOC -->

## A checklist: COBIDAS report

The organization from human brain mapping (OHBM) created the Committee on Best practices In Data Analysis and Sharing (COBIDAS) that published a report with a set of [guidelines](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5685169/) with an appended [checklist](https://www.biorxiv.org/content/early/2016/07/10/054262.full.pdf+html) on how to conduct and report fMRI studies. It is a very useful resource to use to make sure you are not forgetting anything when writing up your article.
See also Jeanette Mumford's [video](https://www.youtube.com/watch?v=bsM4KowO5Vc) about it.

* Journal specific requirements or checklists like those of Nature (   ???   ) or Elife (   ???   )

* [21 words solution] (   ???   )

* [Constraints on generality] (   ???   )

* Other checklists:
-   [here](http://biostat.mc.vanderbilt.edu/wiki/Main/ManuscriptChecklist)

-   http://jonathanpeelle.net/blog/2016/3/23/a-manuscript-checklist-for-improving-science

## Percent signal change (   ???   )

* a FAQ [article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3896880/) on the GLM by Cyril Pernet with [matlab code](https://www.frontiersin.org/articles/file/downloadfile/58014_supplementary-materials_datasheets_1_zip/octet-stream/Data%20Sheet%201.ZIP/2/58014) to go through has some mention on reporting PSC.

* See also this FSL [guide](http://mumford.bol.ucla.edu/perchange_guide.pdf) by Jeanette Mumford (   ???   ) for reporting results in PSC.

* This [post](http://blogs.warwick.ac.uk/nichols/entry/spm_plot_units/) by [Tom Nichols](https://twitter.com/ten_photos) can be helpful to understand what are the units that SPM paranter estimates are reported in.

* The [MarsBAR](http://marsbar.sourceforge.net/) SPM toolbox can also help you deal with PSC.

* From the [ArtRepair webiste](https://cibsr.stanford.edu/content/dam/sm/cibsr/documents/tools/methods/artrepair-software/FMRIPercentSignalChange.pdf)

## Making figures (   ???   )

<!-- TO DO

I keep hearing that the books by Edward R. Tufte are great
https://www.amazon.com/dp/0961392118/?tag=codihorr-20
https://www.amazon.com/dp/0961392126/?tag=codihorr-20

http://mkweb.bcgsc.ca/essentials.of.data.visualization/
https://www.jisc.ac.uk/full-guide/data-visualisation
https://jimgrange.wordpress.com/2016/06/15/solution-to-barbarplots-in-r/
https://f1000research.com/articles/4-466/v1 -->

blog and paper guillaume Rousselet
http://eelkespaak.nl/blog/customizing-common-m-eeg-plots-part-2-the-time-frequency-representation-tfr/

### Color maps
-   http://colorbrewer2.org/#type=sequential&scheme=BuGn&n=3
-   color blind friendly
-   the JET colormap is EVIL
-   https://davidmathlogic.com/colorblind/#%23D81B60-%231E88E5-%23FFC107-%23004D40
-    Dual coded statistical maps
[Code](http://mialab.mrn.org/datavis/) to display beta values and t values on the same map. From the *Data visualization in the neurosciences: overcoming the curse of dimensionality* [paper](https://www.ncbi.nlm.nih.gov/pubmed/22632718).

## Tools to check results/statistics (   ???   )

Those recent tools cannot be applied to statistical maps but they can be useful for any behavioural results. Many of them can be used on a paper you are about to publish to check for errors or on a paper you are reviewing / reading.

* [Statcheck](http://statcheck.io/) developed by automatically checks for errors in statistical reporting making sure that your p values match with your t/F values and degrees of freedom.

* [GRIM test](http://www.prepubmed.org/grim_test/) checks for Granularity-Related Inconsistency of Means. Developed by [Nick Brown](https://twitter.com/sTeamTraen) and [James Heathers](https://twitter.com/jamesheathers) makes sure that the mean reported are plausible given a measurement scale (liek a Likert scale or a visual analog scale) and a sample size. There are [GRIMMER](http://www.prepubmed.org/grimmer/, GRIMMEST extension to standard deviations and F values.

* [SPRITE](https://peerj.com/preprints/26968v1/) stands for Sample Parameter Reconstruction via Iterative TEchniques and allows to generate the possible data distribution given a scale, a mean and variability measure [web app](http://www.prepubmed.org/sprite/), [shiny app](https://steamtraen.shinyapps.io/rsprite/), [code](https://osf.io/pwjad/).

* There is also the [p-checker shinyapp](https://shinyapps.org/apps/p-checker/) that lets you inspect/diagnose a group of results by doing a p-curve analysis, a test of insufficient variance, z-curve analysis, …

## Peer review (   ???   )

<!-- TO DO -->

[Peer review openness (PRO) initiative](https://opennessinitiative.org/) to ask for data
