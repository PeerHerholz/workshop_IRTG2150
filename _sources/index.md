
```{toctree}
---
hidden: true
includehidden: true
titlesonly: true
---
```
<img src="https://nipy.org/img/nipy.svg" alt="workshop logo" width="300" style="margin:0 0 0 0"/>

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/peerherholz/mybinder_workshop_IRTG2150/HEAD)
[![GitHub size](https://img.shields.io/github/repo-size/peerherholz/workshop_IRTG2150.svg)](https://github.com/peerherholz/workshop_IRTG2150/archive/main.zip)
[![Docker Hub](https://img.shields.io/docker/pulls/peerherholz/workshop_IRTG2150)](https://hub.docker.com/r/peerherholz/workshop_IRTG2150/)
[![License](https://img.shields.io/github/license/peerherholz/workshop_IRTG2150)](https://github.com/PeerHerholz/workshop_IRTG2150)

# Welcome!

<div style="text-align: justify;">
Hello everyone and welcome to the "MRI analysis in Python using Nipype, Nilearn and more" workshop conducted for the <a href="https://www.irtg2150.rwth-aachen.de/">IRTG 2150</a> at the <a href="https://www.rwth-aachen.de/cms/~a/root/?lidx=1">RWTH Aachen</a>, we're glad to see you here!

<br>
<br>

Within these pages, we provide information on how to follow the workshop, as well as respective materials. This [jupyter book](https://jupyterbook.org/intro.html) will include the used slides and code in a way that they can be explored in an interactive manner. You can navigate through the respective sections via the TOC on the left side and within sections via the TOC on the right side. The three symbols in the top allow to enable full screen mode, link to the underlying [Github repository](https://github.com/PeerHerholz/workshop_IRTG2150) and allow you to download the contents as a pdf or jupyter notebook respectively. Some sections will additionally have a little rocket in that row which will allow you to interactively rerun certain analyses via cloud computing. Additionally, we support public reviews and comments through an [hypothes.is plugin](https://web.hypothes.is/) with which you can interact on the right side. All of this awesomeness (talking about the infrastructure and resource) is possible through the dedicated and second to none work of the [Jupyter community](https://jupyter.org/community), specifically, the [Executable/Jupyter Book](https://executablebooks.org/en/latest/) and [mybinder project](https://mybinder.org/).
</div>

````{margin}
```{warning}
These pages are currently under construction and will be updated continuously.
Please visit this page again in the next few weeks for further information.
````

# Python & neuroimaging
  
<div style="text-align: justify;">

As you can see in the `TOC` on the left sidebar, there’s quite a bunch going on here. You may ask: “Oh my, is all of this really necessary?”. Well, it might depend on who you ask but this workshop and the people conducting it think so and here’s why: working with neuroimaging data is incredibly complex and creating a structured and holistic way to empirically train folks needs time, effort, details, and dedication. Additionally, to increase openness and sustainability, and thus ultimately the success rate of the materials at hand, these things need to be prepared and supplied in a way that is findable, accessible, interoperable and re-usable (FAIR) for as many people as possible. This workshop is therefore designed to provide only `FAIR` content and materials.

You can use the following sections to navigate through the content of the workshop:
</div>


::::{card-carousel} 2

:::{card}
:margin: 3
:class-body: text-center
:class-header: bg-light text-center
:link: https://peerherholz.github.io/workshop_IRTG2150/overview.html
**A short introduction**
^^^
```{image} 
:height: 100
```

What's this workshop about and how is it organized?
+++
Explore this section {fas}`arrow-right`
:::

:::{card}
:margin: 3
:class-body: text-center
:class-header: bg-light text-center
:link: https://peerherholz.github.io/workshop_IRTG2150/setup.html

**Setup**
^^^
```{image} 
:height: 100
```

How are things implemented and supposed to work?
+++
Explore this section {fas}`arrow-right`
:::
::::


::::{card-carousel} 2

:::{card}
:margin: 3
:class-body: text-center
:class-header: bg-light text-center
:link: https://peerherholz.github.io/workshop_IRTG2150/outline.html
**Outline**
^^^
```{image} 
:height: 100
```

What are the specific topics and aspects taught?
+++
Explore this section {fas}`arrow-right`
:::

:::{card}
:margin: 3
:class-body: text-center
:class-header: bg-light text-center
:link: https://peerherholz.github.io/workshop_IRTG2150/prerequisites.html

**Prerequisites**
^^^
```{image} 
:height: 100
```

What are the prerequisites for the workshop?
+++
Explore this section {fas}`arrow-right`
:::
::::


::::{card-carousel} 2

:::{card}
:margin: 3
:class-body: text-center
:class-header: bg-light text-center
:link: https://peerherholz.github.io/workshop_IRTG2150/data.html
**Neuroimaging data basics**
^^^
```{image} 
:height: 100
```

Basics of neuroimaging data handling in `python`.
+++
Explore this section {fas}`arrow-right`
:::

:::{card}
:margin: 3
:class-body: text-center
:class-header: bg-light text-center
:link: https://peerherholz.github.io/workshop_IRTG2150/advanced.html

**Advanced topics**
^^^
```{image} 
:height: 100
```

Specific neuroimaging analyses in `python`.
+++
Explore this section {fas}`arrow-right`
:::
::::

# I've got a question!

<div style="text-align: justify;">

In case you have any questions or difficulties going through the workshop, please don’t hesitate a single second to get in touch with
us. A great way to do this is to
[open an issue](https://github.com/PeerHerholz/workshop_IRTG2150/issue) on the
[GitHub site of the Workshop](https://github.com/PeerHerholz/workshop_IRTG2150) (also possible via the GitHub button at the top of the pages).
We would also highly appreciate and value every feedback or idea or you
might have (via [issues](https://github.com/PeerHerholz/workshop_IRTG2150) or [hypothes.is annotation feature](https://web.hypothes.is/) on the right).

</div>

## Acknowledgements

<div style="text-align: justify;">

This workshop was organized by the [IRTG 2150](https://www.irtg2150.rwth-aachen.de/), specifically Dr. Philippa Hülpen.

![Local Image](static/Logo3.png)
![Local Image](static/DFG_Logo.png)


<br>
<br>
Peer Herholz' work on and ability to compile this workshop was enabled through training received at the <a href="https://www.mcgill.ca/neuro/">Montreal Neurological Institute</a>, specifically the <a href="https://neurodatascience.github.io/">NeuroDataScience - ORIGAMI lab</a> supported by funding from the Canada First Research Excellence Fund, awarded to McGill University for the <a href="https://www.mcgill.ca/hbhl/">Healthy Brains for Healthy Lives initiative</a>, the <a href="https://www.nih.gov/">National Institutes of Health (NIH)</a> <a href="https://www.repronim.org/">NIH-NIBIB P41 EB019936 (ReproNim)</a>, the <a href="https://www.nimh.nih.gov/">National Institute Of Mental Health</a> of the NIH under Award Number <a href="https://www.neurosynth.org/">R01MH096906 (Neurosynth)</a>, a <a href="https://conp.ca/">research scholar award from Brain Canada, in partnership with Health Canada, for the Canadian Open Neuroscience Platform initiative</a>, as well as an <a href="https://sites.google.com/view/unique-neuro-ai">Excellence Scholarship from Unifying Neuroscience and Artificial Intelligence - Québec</a>.

</div>
