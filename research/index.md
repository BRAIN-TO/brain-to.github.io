---
title: Research
nav:
  order: 1
  tooltip: Software, datasets, and more
---

# {% include icon.html icon="fa-solid fa-wrench" %}Research

The BRAIN-TO Lab strives for advancing our understanding of the human brain by research in three core areas:
- MR Physics
- Artificial Intelligence (AI) & Cognitive Neuroscience
- Clinical Applications

{% include tags.html tags="mr-physics, ai, clinical" %}

{% include search-info.html %}

{% include section.html %}

## Core Areas

{%
  include feature.html
  image="images/mr_physics.png"
  title="MR Physics"
  text="Magnetic resonance imaging (MRI) offers a unique opportunity to non-invasively study the human brain, equipped with a wealth of contrasts (to disentangle structures and functions), and a favourable window of spatiotemporal resolution. But to expand its clinical and neuroscientific scope, MRI has to become faster and more robust. A key ingredient to this end is a mechanistic understanding of the imaging physics, and its consideration in the way we acquire and reconstruct MR images. This comprises the choice of optimal sequence and sampling strategy for the target application (e.g., spiral trajectories for short echo-time) a detailed characterization of both hardware imperfections (e.g., heating/field drift and trajectory errors) and subject-related noise sources (e.g., breathing, motion) giving rise to image artifacts, the accurate inclusion of this information into an expanded signal model of the MR imaging process and advanced image reconstruction techniques capable of inverting these intricate models. This integrated approach leads to better imaging data tailored to the analysis and diagnostic purpose of the MR exams. The characterization of each scan's imaging peculiarities allows for better comparability of multi-site studies in the era of big data. At the other end of the spectrum, personalized medicine requires individualized MR imaging protocols that are enabled by flexible and extendable signal models and reconstructions."
%}

{%
  include feature.html
  title="AI & Cognitive Neuroscience"
  image="images/modeling.jpg"
  text="The overall goal of this research line is to develop artificial neuronal network approaches that reproduces brain MR imaging data, representing the next neuroscience revolution (“neurobiologically-plausible artificial intelligence (AI) models”), fundamentally advancing our understanding of human brain function. We cannot develop more advanced models of brain functioning without a more thorough understanding of brain dynamics and networks. However, our understanding of the human brain is limited by biased approaches and limitations of traditional statistics, thus forcing us to rely on artificial machine learning algorithms to provide an alternative perspective. The goal is to dynamically and comprehensively describe cognitive processes as an emergent property of brain networks on healthy subjects and patients. This will then allow characterizing human brain function on a single-subject level for the purpose of personalized medicine. In the individual projects of this research line, we develop and apply advanced AI methods on human fMRI data and develop dynamic generative models of brain connectivity (aka Dynamic Causal Modeling)."
%}

{%
  include feature.html
  title="Clinical Applications"
  image="images/compare_7t-1.5t.jpg"
  text="The results of the research of the MRI physics and fundamental neuroscience pillars of the BRAIN-TO group will be translated into the clinical workflows in collaboration with clinical research groups within UHN. In particular, fast MRI acquisition and novel contrasts will enable to provide unprecedented information about the vasculature (Collaborator: Drs. Timo Krings, Paula Alcaide Leon), a highly relevant topic given that pathological vasculature is associated with many neurodegenerative diseases and tumors. We are working on novel perfusion MRI techniques to identify tumor mimickers, which can provide information to avoid unnecessary brain surgeries. Preoperative perfusion characterization of brain masses can assist in differential diagnosis and, hence, be very useful to inform surgical management in the context of this diagnostic dilemma. In addition, we are developing analysis and experimental approaches to assess the response of blood vessels to quantitative vasodilatory stimuli, called cerebrovascular reactivity (CVR) (Collaborator: Dr. David Mikulis). CVR is an essential function of healthy cerebral vessels that is altered by aging, various brain diseases and angiogenesis in brain tumors and radiotherapy. Our recent work has also identified a novel needle-free method for measuring tissue perfusion that uses endogenous hemoglobin, eliminating the need for injections of contrast agents, and utilize it for characterizing brain tumor tissue and vascular diseases routinely in patients at UHN. Finally, we are setting-up an innovative framework in which technological developments and processing pipelines can be readily translated into clinical practice. The computational infrastructure required will allow radiologists and clinical specialists to incorporate novel MRI contrasts, typically not available in the clinical workflow, to their assessments of brain patients."
%}

{% include section.html %}

## Projects

{% include list.html component="card" data="projects" filter="!group" style="small" %}
