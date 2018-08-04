---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "**Wenting Zhao**, Lijin Wang, Yilong Yin, et al"
    title: "
	Sequential Quadratic Programming Enhanced Backtracking Search Algorithm"
    #keywords: "Locu"
    month: "April"
    year: "2018"
    address: "Beijing, China"
    booktitle: "Frontiers of Computer Science"
    url: 2018SQPBSA.pdf


  - author: "**Wenting Zhao**, Lijin Wang, Bingqing Wang, Yilong Yin"
    title: "Best Guided Backtracking Search Algorithm for Numerical Optimization Problems"
    month: "October"
    year: "2016"
    address: "Passau, Germany"
    booktitle: "9th International Conference on Knowledge Science, Engineering and Management **(KSEM 2016)**"
    url: 2016BGBSAzhao.pdf
    slides: 2016BGBSAzhaoslides.pdf

  - author: "**Wenting Zhao**, Lijin Wang, Yilong Yin, Bingqing Wang, Yi Wei, Yushan Yin"
    title: "An Improved Backtracking Search Algorithm for Constrained Optimization Problems"
    url: 2014IBSAzhao.pdf
    month: "October"
    year: "2014"
    address: "Sibiu, Romania"
    booktitle: "7th International Conference on Knowledge Science, Engineering and Management **(KSEM 2014)**"

  - author: "**Wenting Zhao**, Lijin Wang, Yuxiao Shi, Xiaoming Xi, Yilong Yin, Yuchun Tang"
    month: "July"
    year: "2017"
    title: "A Multi-objective Framework for Brain MRI Threshold Segmentation"
    url: 2017Multiobjective Framework.pdf
    address: "Fuzhou, China"
    booktitle: "8th International Conference on Information Technology in Medicine and Education **(ITME 2016)**"

---

# Publications
________________________________________________________________________________

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).

    {% endif %}
{% endunless %}
{% endfor %}
