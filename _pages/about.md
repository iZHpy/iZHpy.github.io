---
permalink: /
title: ""
author_profile: true
hide_sidebar_avatar_name: true  # name and photo are shown in the intro below instead
redirect_from: 
  - /about/
  - /about.html
---

<h1 class="home-name">{{ site.author.name }}</h1>

<div class="home-intro" markdown="1">
<div class="home-intro__text" markdown="1">

Hi there! 👋 I am a third-year Ph.D. student in Computer Engineering at the [University of Southern California (USC)](https://www.usc.edu/), advised by [Prof. Paul Bogdan](https://cps.usc.edu/). I received my B.E. in Electronic Information and Communication Engineering from [Huazhong University of Science and Technology (HUST)](https://english.hust.edu.cn/) in 2024.

My research focuses on **Multi-Agent LLM Systems** and **Machine Learning Systems (MLSys)**, with interests in agentic post-training, LLM modeling, and efficiency. I am particularly interested in long-context reasoning and the latency and efficiency of multi-agent systems, as well as MLSys topics including reasoning compression and efficient operators (kernels). I have also worked on LLM agents for hardware design (spec-to-HDL generation) and graph neural networks (GNNs).

I am always open to potential collaborations, please feel free to reach out.

</div>
<div class="home-intro__photo">
<img src="{{ site.author.avatar | prepend: '/images/' | relative_url }}" alt="{{ site.author.name }}" fetchpriority="high"/>
</div>
</div>

🔥 News
======
------

- *2026.10*: &nbsp;🎉 One paper accepted to **EMNLP 2026**!
- *2026.07*: &nbsp;🎉 One paper accepted to **ICCAD 2026**!
- *2026.07*: &nbsp;🎉 One paper published in **npj Computational Materials**!
- *2026.02*: &nbsp;🎉 One paper accepted to **MLSys 2026**!

📚 Educations
======
------

<div class="exp-item">
<img class="exp-item__logo" src="{{ '/images/logos/usc.png' | relative_url }}" alt="USC logo"/>
<div class="exp-item__text">
<strong>University of Southern California (USC)</strong>, Los Angeles, CA<br/>
<strong>Ph.D. in Computer Engineering</strong>&nbsp;&nbsp; <span class="exp-item__date">Aug 2024 – Present</span>
</div>
</div>

<div class="exp-item">
<img class="exp-item__logo" src="{{ '/images/logos/hust.png' | relative_url }}" alt="HUST logo"/>
<div class="exp-item__text">
<strong>Huazhong University of Science and Technology (HUST)</strong>, Wuhan, China<br/>
<strong>B.E. in Electronic Information and Communication Engineering</strong>&nbsp;&nbsp; <span class="exp-item__date">Aug 2020 – Jun 2024</span>
</div>
</div>


💻 Internship Experience
======
------

<div class="exp-item">
<img class="exp-item__logo" src="{{ '/images/logos/baidu.png' | relative_url }}" alt="Baidu logo"/>
<div class="exp-item__text">
<strong>Baidu Research</strong>, Beijing, China<br/>
<strong>Machine Learning Research Intern</strong>&nbsp;&nbsp; <span class="exp-item__date">May 2023 – Jan 2024</span>
</div>
</div>



📑 Publications
======
------

<p class="pub-note">* Equal contribution</p>

{% include publications-home.html %}





<!-- 💬 Services
======
------ -->

🔬 Academic Experience
======
------

<div class="exp-item">
<img class="exp-item__logo" src="{{ '/images/logos/tsinghua.png' | relative_url }}" alt="Tsinghua University logo"/>
<div class="exp-item__text">
<strong>Tsinghua University</strong>, Beijing, China<br/>
<strong>Visiting Student</strong>&nbsp;&nbsp; <span class="exp-item__date">Jan 2023 – Feb 2024</span><br/>
Supervisor: <a href="https://lars-group.github.io/">Prof. Quanming Yao</a>
</div>
</div>


😊 Honors and Awards
======
------

+ **Annenberg Graduate Fellowship**, USC, 2024
+ **Outstanding Undergraduate Graduates**, HUST, 2024
+ **National Olympiad in Informatics in Province (NOIP)**, JIANGSU
{: .compact-list}

{% comment %} Visitor map: shown only once _includes/visitor-map.html contains the embed code {% endcomment %}
{% capture visitor_map %}{% include visitor-map.html %}{% endcapture %}
{% assign visitor_map_code = visitor_map | strip %}
{% if visitor_map_code != "" %}
<div class="visitor-map">{{ visitor_map_code }}</div>
{% endif %}




<!-- A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured Markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various Markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your Markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over - just be sure to save the Markdown files! You can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

For those users that need more advanced functionality, the template also supports the following popular tools:
- [MathJax](https://www.mathjax.org/) for mathematical equations
- [Mermaid](https://mermaid.js.org/) for diagraming
- [Plotly](https://plotly.com/javascript/) for plotting

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this template](https://github.com/academicpages/academicpages.github.io) by clicking the "Use this template" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one Markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a Markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each Markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual Markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the Markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and Markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
