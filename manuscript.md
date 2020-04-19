---
author-meta:
- Christopher W. Tessum
bibliography:
- content/manual-references.json
date-meta: '2020-04-19'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="A Distributed Science Manifesto: Framework for Equitable Funding, Dissemination and Synthesis" />

  <meta name="citation_title" content="A Distributed Science Manifesto: Framework for Equitable Funding, Dissemination and Synthesis" />

  <meta property="og:title" content="A Distributed Science Manifesto: Framework for Equitable Funding, Dissemination and Synthesis" />

  <meta property="twitter:title" content="A Distributed Science Manifesto: Framework for Equitable Funding, Dissemination and Synthesis" />

  <meta name="dc.date" content="2020-04-19" />

  <meta name="citation_publication_date" content="2020-04-19" />

  <meta name="dc.language" content="en-US" />

  <meta name="citation_language" content="en-US" />

  <meta name="dc.relation.ispartof" content="Manubot" />

  <meta name="dc.publisher" content="Manubot" />

  <meta name="citation_journal_title" content="Manubot" />

  <meta name="citation_technical_report_institution" content="Manubot" />

  <meta name="citation_author" content="Christopher W. Tessum" />

  <meta name="citation_author_institution" content="Department of Civil and Environmental Engineering, University of Illinois" />

  <meta name="citation_author_orcid" content="XXXX-XXXX-XXXX-XXXX" />

  <meta name="twitter:creator" content="@ctessum" />

  <link rel="canonical" href="https://ctessum.github.io/lrs/" />

  <meta property="og:url" content="https://ctessum.github.io/lrs/" />

  <meta property="twitter:url" content="https://ctessum.github.io/lrs/" />

  <meta name="citation_fulltext_html_url" content="https://ctessum.github.io/lrs/" />

  <meta name="citation_pdf_url" content="https://ctessum.github.io/lrs/manuscript.pdf" />

  <link rel="alternate" type="application/pdf" href="https://ctessum.github.io/lrs/manuscript.pdf" />

  <link rel="alternate" type="text/html" href="https://ctessum.github.io/lrs/v/660a5201a7520f6c4b2daad4db4fb6cf7cc993ea/" />

  <meta name="manubot_html_url_versioned" content="https://ctessum.github.io/lrs/v/660a5201a7520f6c4b2daad4db4fb6cf7cc993ea/" />

  <meta name="manubot_pdf_url_versioned" content="https://ctessum.github.io/lrs/v/660a5201a7520f6c4b2daad4db4fb6cf7cc993ea/manuscript.pdf" />

  <meta property="og:type" content="article" />

  <meta property="twitter:card" content="summary_large_image" />

  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />

  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />

  <meta name="theme-color" content="#ad1457" />

  <!-- end Manubot generated metadata -->'
keywords:
- markdown
- publishing
- manubot
lang: en-US
manubot-clear-requests-cache: false
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
title: 'A Distributed Science Manifesto: Framework for Equitable Funding, Dissemination and Synthesis'
...






<small><em>
This manuscript
([permalink](https://ctessum.github.io/lrs/v/660a5201a7520f6c4b2daad4db4fb6cf7cc993ea/))
was automatically generated
from [ctessum/lrs@660a520](https://github.com/ctessum/lrs/tree/660a5201a7520f6c4b2daad4db4fb6cf7cc993ea)
on April 19, 2020.
</em></small>

## Authors



+ **Christopher W. Tessum**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [XXXX-XXXX-XXXX-XXXX](https://orcid.org/XXXX-XXXX-XXXX-XXXX)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [ctessum](https://github.com/ctessum)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [ctessum](https://twitter.com/ctessum)<br>
  <small>
     Department of Civil and Environmental Engineering, University of Illinois
  </small>



## Abstract {.page_break_before}




(Citations and supporting information to be added throughout.)

## Introduction


Scientific discovery is necessarily a slow process: results of individual studies must be verified, vetted, and synthesized, and decisions must be made how to allocate resources among future investigative directions before work can continue.
These processes happen both at the micro scale within an individual scientist or lab group, and at the macro scale within members of a society.
The document is concerned with the latter scale.

At the society scale, vetting and synthesizing scientific results and allocating resources to future represent a coordination problem: many scientific stakeholders must coordinate to allocate constrained resources toward publishing existing studies and funding new ones.

Typically, the coordination problem is solved by centralization.
Organizations and individuals act as gatekeepers to determine which studies get peer-reviewed and published and which researchers and ideas are funded to continue their work.

The current system has delivered great increases in human understanding and quality of life, and should not be discarded, but has well-documented shortcomings.
An incomplete list includes the monetization and the monopolization of access to academic research output by for-profit publishing companies, and the concentration of funding allocation power in the hands of a small number of decision-makers who—like all humans—are biased may have narrow interests.
The most common alternative to centralized decision-making — market-based coordination — can be effective for funding research with clear monetization potential, but is not considered effective for research where the profit potential is not clear.

The centralization of scientific funding, synthesis, and dissemination is a bottleneck for the rate scientific advancement.
This document describes design constraints for a distributed system for scientific funding, dissemination, and synthesis, and then describes the components of a component distributed science framework.


## Sort, don't filter

Traditional scientific journals make binary publishing decisions: articles are either accepted or rejected.
This was necessary when physical, printed journals were the only method of dissemination, but is vestigial in the current electronic-delivery paradigm.
This is evidenced by the rapid adoption of preprint servers (e.g., https://arxiv.org/) and journals with pre-review "discussion" versions, both of which are much less selective of which articles they will publish than conventional journals.

However, preprint and discussion publishers seem to be supplementing rather than replacing traditional journals, suggesting that the peer-review process serves a valuable function of signaling which articles are the most important and useful.


## Distributed, compensated review

The traditional academic publishing system relies on reviews volunteered by scientist peers, where the definition of "peer" is determined by article authors and journal editors.
In addition to the fact that this results in for-profit publishers benefit from unpaid labor, this system results in reviewers being hard to find, the final number of reviews being small, and the review process taking a long time.
Additionally, the amount of thought put into each review can vary widely.
Because reviews are not credited or compensated, ideas and attitudes in reviews are skewed toward those of individuals for whom those considerations are less important, and therefore not necessarily representative of scientific stakeholders as a whole.

Scientific review should be compensated, and it should not be limited to the social networks of the article authors and journal editors.
Solutions exist for distributed review (e.g., https://prereview.org/, https://openreview.net/) and review recognition (e.g., https://www.sciencemag.org/careers/2016/02/getting-credit-peer-review), but stop short of offering monetary compensation or an equivalent incentive.


## Minimize barriers to access to and participation in science

In practice, the legacy publication system is only accessible to scientists who work for institutions that can afford subscriptions to journal packages, and even then it can be difficult to download articles, especially when off-campus.
For scientists and aspiring scientists not associated with such an organization, even when between jobs, and especially for those in low and low and middle income countries, access is often not possible.
Open-access journals aim to solve this problem, but in practice fees are often just shifted from readers to authors, making open-access publication an option only for highly-funded researchers.


# Distribute funding decisions

The current system of centralized funding decisions through public and private granting agencies and foundations, which rely on tacit knowledge accumulated within a relatively small set of individuals to predict which projects will be worthwhile and successful.
However, centralized decision-making can be inefficient and can propagate biases held by in-group grant officers and reviewers against out-group applicants and ideas.

We believe a distributed decision framework could provide a complementary utility to the existing centralized systems.
Distributed decision systems tend to have different biases from centralized systems, and the software systems which facilitate distributed decision making can be designed to reduce those biases.
Buterin et al. (2018; https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3243656) describe a new system for distributed funding decision which will serve as the core of our framework.


## Preserve data ownership

Scientific manuscripts are valuable, as are the reviews contributed by scientific peers and data that is collected regarding numbers of article downloads, social media shares and sentiment, etc.
Scientific publishers should commit to sharing revenue generated using this data with the individuals the contributed the data.


## Break network effects

Existing publishers benefit from strong network effects: scientists want to publish in established, prestigous journals to gain a wide readership and to signal the quality of their work.
Any successful upstart must have a strategy from overcoming these network effects and establishing its own.


## Distributed Science Framework

Here we propose a candidate framework for meeting the design constraints above, the Distributed Science Framework (DSF).
The candidate framework acts both as a publisher and a funder of science.
At its core is the concept of Liberal Radicalism (LR; Buterin et al., 2018), a system for the efficient allocation of grant funding.
The key components are users, credits, articles, reviews, and grants.

### Components

#### Users

DSF users are online entities that are verified to be individual humans.
Verification is critical to avoid the gaming of the system, and will be accomplished by requiring each user to have an email address issued by an institution that is registered with DSF.

#### Credits

DSF credits are a digital currency system that can be converted to and from dollars or other global currencies.
Credits are used to distribute grants and review compensation and to pay for article uploads and downloads.

#### Articles

Articles are scientific manuscripts, equivalent to articles in existing scientific journals.
Authors pay a fee to upload a manuscript, which is published immediately.
Authors must provide contribution percents for each author (adding up to 100% for all authors) upon uploading an article.
Articles are only available to users; this could be enforced using DRM or blockchain technology, or using weaker methods currently favored by traditional publishers.
A new user gets one article download for free, subsequent articles must be paid for using credits.
The credits required to download an article will be approximately equivalent to the credits given for reviewing an article, so users not able or wishing to pay for articles with money can pay for a new article by submitting a review of their previous download.

#### Reviews and metareviews

Users can submit reviews of articles they have read both using quantitative rubrics and text responses, similar to existing journals.
Unlike existing journals, reviewers would be compensated using credits.
Users will also receive compensation for submitting metareviews (reviews of reviews).

#### Grants

Agencies and individuals who wish to provide financial funds for science can register grants through DSF.
Funders can specify criteria that users must meet to be eligible for a grant (including topics of previous articles, location, etc.) and restrictions regarding what the grant money can be spent on.
Then, grant funds will be allocated among qualified users based on the quality of their previous articles.

Article quality will be determined by an algorithm that includes number of unique users that have downloaded the article, citations, and reviews.
Review scores will be weighted by results of metareviews and by the quality scores of articles authored by the reviewer.

#### Operational overhead and revenue model

DSF would need to be implemented and operated by an organization.
Functions of the organization would include creating and maintaining the DSF software infrastructure, moderating user content, and policing for abuse of the system.

These activities could be funded by grant overhead.
As machine learning and artificial intelligence technology improves over time, AI could potentially be used to synthesize information contained in the articles and reviews into revenue-generating products (for example, automatic literature reviews) that could provide operating revenue and additional compensation for authors and reviewers.

### How DSF meets the design constraints

* __Sort, don't filter__: Articles are published immediately, but ranked according to reviews and metareviews. DSF will include searching and sorting algorithms the prioritize the return of high-quality articles.
* __Distributed, compensated review__: Users will be paid for reviews, and financially-constrained users can submit reviews in lieu of paying for article downloads and uploads
* __Minimize barriers to access to and participation in science__: Downloading and publishing articles can be paid for by submitting reviews
* __Distribute funding decisions__: Grants are distributed algorithmically based downloads and a distributed review system.
* __Preserve data ownership__: Users are compensated for reviews and for publishing high-quality articles.
* __Break network effects__: Early adopters be incentivised to participate by the relatively easy access to grant funding. As the number of users increases, the competition for grant funding will increase, as will the prestige associated with having a highly-rated article.


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
