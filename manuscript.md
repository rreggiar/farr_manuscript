---
title: Anti-Racism and the Next Generation of Disease Diagnostic Tools
keywords:
- liquid-biopsy
- RNA
- equity
- inclusion
- racism
- diversity
- genetics
- genomics
- anti-racism
- engineering
lang: en-US
date-meta: '2022-12-01'
author-meta:
- Roman E. Reggiardo
header-includes: |-
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta name="dc.title" content="Anti-Racism and the Next Generation of Disease Diagnostic Tools" />
  <meta name="citation_title" content="Anti-Racism and the Next Generation of Disease Diagnostic Tools" />
  <meta property="og:title" content="Anti-Racism and the Next Generation of Disease Diagnostic Tools" />
  <meta property="twitter:title" content="Anti-Racism and the Next Generation of Disease Diagnostic Tools" />
  <meta name="dc.date" content="2022-12-01" />
  <meta name="citation_publication_date" content="2022-12-01" />
  <meta name="dc.language" content="en-US" />
  <meta name="citation_language" content="en-US" />
  <meta name="dc.relation.ispartof" content="Manubot" />
  <meta name="dc.publisher" content="Manubot" />
  <meta name="citation_journal_title" content="Manubot" />
  <meta name="citation_technical_report_institution" content="Manubot" />
  <meta name="citation_author" content="Roman E. Reggiardo" />
  <meta name="citation_author_institution" content="Department of Biomolecular Engineering, University of California at Santa Cruz" />
  <meta name="citation_author_orcid" content="0000-0001-6309-249X" />
  <meta name="twitter:creator" content="@rreggiar" />
  <link rel="canonical" href="https://rreggiar.github.io/farr_manuscript/" />
  <meta property="og:url" content="https://rreggiar.github.io/farr_manuscript/" />
  <meta property="twitter:url" content="https://rreggiar.github.io/farr_manuscript/" />
  <meta name="citation_fulltext_html_url" content="https://rreggiar.github.io/farr_manuscript/" />
  <meta name="citation_pdf_url" content="https://rreggiar.github.io/farr_manuscript/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://rreggiar.github.io/farr_manuscript/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://rreggiar.github.io/farr_manuscript/v/ffd7f94da637b958494abc00fca14b1ef594120c/" />
  <meta name="manubot_html_url_versioned" content="https://rreggiar.github.io/farr_manuscript/v/ffd7f94da637b958494abc00fca14b1ef594120c/" />
  <meta name="manubot_pdf_url_versioned" content="https://rreggiar.github.io/farr_manuscript/v/ffd7f94da637b958494abc00fca14b1ef594120c/manuscript.pdf" />
  <meta property="og:type" content="article" />
  <meta property="twitter:card" content="summary_large_image" />
  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />
  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />
  <meta name="theme-color" content="#ad1457" />
  <!-- end Manubot generated metadata -->
bibliography:
- content/manual-references.json
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
manubot-clear-requests-cache: false
...






<small><em>
This manuscript
([permalink](https://rreggiar.github.io/farr_manuscript/v/ffd7f94da637b958494abc00fca14b1ef594120c/))
was automatically generated
from [rreggiar/farr_manuscript@ffd7f94](https://github.com/rreggiar/farr_manuscript/tree/ffd7f94da637b958494abc00fca14b1ef594120c)
on December 1, 2022.
</em></small>

## Authors



+ **Roman E. Reggiardo**
  <br>
    ![ORCID icon](images/orcid.svg){.inline_icon width=16 height=16}
    [0000-0001-6309-249X](https://orcid.org/0000-0001-6309-249X)
    · ![GitHub icon](images/github.svg){.inline_icon width=16 height=16}
    [rreggiar](https://github.com/rreggiar)
    · ![Twitter icon](images/twitter.svg){.inline_icon width=16 height=16}
    [rreggiar](https://twitter.com/rreggiar)<br>
  <small>
     Department of Biomolecular Engineering, University of California at Santa Cruz<br>
     · Funded by UCSC Baskin Engineering FARR; NIDDK/KUH F99 DK131504
  </small>


::: {#correspondence}
✉ — Correspondence possible via [GitHub Issues](https://github.com/rreggiar/farr_manuscript/issues)

:::


## Abstract {.page_break_before}

Various forms of highly technical genetic analyses have a long history of being ignorant of race, ethnicity, class, and sex as well as being co-opted for explicitly eugenic, racist, homophobic, or otherwise hateful purposes. 
There is a critical ongoing discussion on how modern sequencing technologies can both contribute to reduction of suffering but also drive harmful narratives due to incomplete and/or unrepresentative results being interpreted as evidence for biological superiority or inferiority. 

A new class of medical technologies, called ‘liquid biopsies’, are poised to dramatically impact how and when cancer diagnoses are made by harnessing genetic information. 
These diagnostic tests account for mutations in one’s genome and/or changes in the abundance of certain expressed genes, measured from a simple blood draw. 

While the promise of liquid biopsies is a future where diagnoses are accessible, accurate, and non-invasive, they face the same potential shortcomings as other genetic tests: without adequate representation during development, it is impossible to say whether diagnostic performance and relevance extends inclusively and equitably across our diverse society. 
This burgeoning technology is intertwined with an equally impactful, far more pervasive, and demonstrably biased approach to classification problems: machine learning. 

In this report, I intend to both quantify and discuss the relevant barriers to equitable liquid biopsy diagnostics by surveying the existing published data and investigating the sources, details, and diversity of samples used to demonstrate liquid biopsy performance.

*<u>UC Santa Cruz Land Acknowledgement</u>*  
> “The land on which we gather is the unceded territory of the Awaswas-speaking Uypi Tribe. 
> The Amah Mutsun Tribal Band, comprised of the descendants of indigenous people taken to 
> missions Santa Cruz and San Juan Bautista during Spanish colonization of the Central Coast, 
> is today working hard to restore traditional stewardship practices on these lands and heal from historical trauma.”


## Introduction {.page_break_before}

Disease or illness, particularly cancer, must be identified and characterized before effective therapies can be applied. 
To make a diagnosis as such, there must be clearly "defined characteristics", also known as "biomarkers", detected at abnormal abundance relative to a pre-defined standard [@27010052]. 
Recent advances in diagnostic technology have enabled the creation of tests that rely on dozens or hundreds biomarkers.
This increased complexity, and in many cases improved performance, does not yet guarantee truly robust performance insulated from the pitfalls that have faced all of medicine and particularly modern diagnostics. 

### Genomics at the forefront of diagnostic technology

Molecular signatures available in biofluids have long been utilized to identify pathological events in diverse, at-risk populations.
Blood sugar concentration is used to continuously monitor diabetes patients, urine has been used to detect pregnancies and prostate cancer [@doi:10.1016/j.urology.2006.12.014], bronchial fluid captured via Bronchoalveolar lavage was considered a "liquid biopsy" of the lungs -- patient lung health could be assessed by the abundance and/or identity of components in the lavage [@2795925].
While bronchoalveolar lavage is used to identify cellular populations, most of the components detected in these liquid biopsies are molecular in nature: the glucose molecule can be targeted to determine blood sugar, human chorionic gonadotropin hormone is used to detect conception, and in that very same fluid a noncoding RNA, PCA3, is used to detect prostate cancer.
Healthy humans should all produce functional hormones and metabolize carbohydrates into glucose -- genetic material, however, is influenced by 

As the complexity of intended-to-diagnose diseases increases to multi-genic pathologies and multi-organ systems, the ability to acquire more complex and broadly informative extracellular signatures is paramount in the development of equivalent diagnostic approaches: Next Generation Sequecing (NGS) liquid biopsies.

Now, at the intersection of contemporary high-throughput NGS and robust machine-learning enabled classification models, liquid biopsies are being developed to sensitively and specifically diagnose diseases in broader at-risk populations. 
While the technologies are primed to deliver a new paradigm in diagnostics that reshape prognostic expectations, there are numerous challenges rooted in equitable representation and meaningful inclusion that require consideration. 
Among them are those questions that have dogged genomics-enabled genetics research in recent decades:

- *Who is data generated by? Who is data generated for?*  
- *How is data stored and who owns it?*  
- *Who benefits from the analyses and technologies built upon biomedical datasets?*  
- *How are social labels used to contextualize analysis?*  

This article seeks to contextualize the advent of minimally invasive, genetics- and genomics-based diagnostics within the current efforts to make genomics research and clinical development equitable and inclusive endeavors. 
In paricular, much has been made of the bias and danger inherent to proclamations derived from currently limited Human genomes and studies. 
Here the focus will be placed on the noisier, more heterogeneous output of the genome: *Transcription*.
As RNA expression becomes a critical tool in diagnosing disease, considering the intersection of this data-rich event with current challenges to genomic studies is critical to understanding its future role as a clinical diagnostic tool.

### DNA in the clinic, RNA at the bench

Revelatory applications of RNA to vaccines developed against SARS-CoV-2 infection notwithstanding, RNA has lagged behind DNA as a clinical tool.





















## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
