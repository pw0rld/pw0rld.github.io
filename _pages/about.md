---
permalink: /
title: "Personal profile"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## Hi there 👋
Hi, everyone! I'm Wei Peng, and I graduated from **Xi'an University of Posts and Telecommunications (XUPT)** in July 2021 with a Bachelor of Engineering in **Cybersecurity**. Welcome to my personal page.

I currently work at [Teenet](https://x.com/teenet_io), where I focus on **TEE + Web3**. You can also follow Teenet on [X/Twitter](https://x.com/teenet_io).

I am enthusiastic about trusted execution environments, confidential computing, software analysis, and attack detection. Building secure systems at the intersection of TEE and Web3 is one of my current research and engineering interests.

## Research Interests
- Trusted Execution Environments (TEE)
- Confidential Computing
- TEE + Web3
- Software Security
- Software Analysis and Attack Detection

## Work Experience
- **Current**: **Teenet**, working on **TEE + Web3** infrastructure and secure systems.
- **Previous**: **Research Assistant**, **Teecertlab**, Southern University of Science and Technology (SUSTech).
  Worked on confidential computing and security analysis under the supervision of [Yinqian Zhang](https://yinqian.org/).

## Education
- **2021**: B.Eng. in **Cybersecurity**, Xi'an University of Posts and Telecommunications (XUPT), Xi'an, China.

## Publications
{% assign publications = site.publications | sort: "date" | reverse %}
{% for post in publications %}
### [{{ post.title }}]({% if post.paperurl %}{{ post.paperurl }}{% else %}{{ base_path }}{{ post.url }}{% endif %})
{% if post.authors %}{{ post.authors }}{% endif %}

*{{ post.venue }}*

{% if post.excerpt %}{{ post.excerpt }}{% endif %}

{% if post.paperurl %}[Paper]({{ post.paperurl }}){% endif %}{% if post.projecturl %} | [Project]({{ post.projecturl }}){% endif %}{% if post.codeurl %} | [Code]({{ post.codeurl }}){% endif %}{% if post.artifacturl %} | [Artifact]({{ post.artifacturl }}){% endif %} | [Details]({{ base_path }}{{ post.url }})

{% endfor %}

## Honors and Awards
- (2023/11)**(WorkShop)** IDASH PRIVACY & SECURITY WORKSHOP 2023 - [Track 3](http://www.humangenomeprivacy.org/2023/index.html), the first place
