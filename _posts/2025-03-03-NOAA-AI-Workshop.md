---
layout: post
title: My Presentation at NOAA's 7th AI Workshop
img: ufs2arco_presentation_cover_slide.png
categories:
    - Research
---

NOAA regularly produces a vast amount of high quality weather and climate data,
and makes it openly available to the public.
Today at NOAA’s 7th AI workshop, I presented PSL's efforts toward publishing these datasets in the cloud,
in an analysis ready format so that it can more easily be used for machine learning development,
as well as for traditional scientific analysis workflows.
It turns out that it’s tricky to execute data transformation pipelines like
this for datasets that are many terabytes to petabytes in size (who would've guessed?!).
Moreover, existing tools to perform this transformation are often best run in the cloud,
but our computational resources at NOAA are typically on-prem, or look like on-prem.

Recently, I’ve leveraged connections between the dataloaders that are used to feed
machine learning models during training in order to accelerate these
transformation pipelines.
Initial results are promising.
I've been able to move 1 year of NOAA's GEFS archive (or at least 2.6 TB of it)
using just 8 nodes CPU nodes in 5 minutes.

My slides for this talk are shown below - please feel free to reach out if you want to talk about this!

<object data="/assets/docs/ufs2arco_noaa_ai_workshop.pdf#toolbar=1&scrollbar=1&navpanes=0"
    type="application/pdf" width="100%" height="100%">
  <p> It appears you don't have a pdf plugin for this browser.
  You can <a href="/assets/docs/tsmith_od02_poster_osm2022.pdf"> click here to
  download the pdf file.</a></p>
</object>
