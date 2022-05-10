---
layout: page
permalink: /research/
title: Research
pubs:

    - title:   "Paper title in 3-7 words that sound like Clingon"
      author:  "M. McFly, D. Kirk, L. Skywalker, H.J. Potter, I. Jones, H. Houdini"
      journal: "Transactions on Black Magic"
      note:    "(presented at Oz)"
      year:    "2016"
      url:     "http://publish-more-stuff.org"
      doi:     "http://dx.doi.org"
      image:   "https://images.duckduckgo.com/iu/?u=http%3A%2F%2Fimages.moviepostershop.com%2Fthe-matrix-movie-poster-1999-1020518087.jpg&f=1"
      media:
        - name: "IMDB"
          url:  "http://www.imdb.com/title/tt0133093/"

---

You can find my Google Scholar profile [here](https://scholar.google.com/citations?hl=en&user=4Wbb_iUAAAAJ) and a listing of my publications on NASA ADS [here](https://ui.adsabs.harvard.edu/search/filter_property_fq_property=AND&filter_property_fq_property=property%3A%22refereed%22&fq=%7B!type%3Daqp%20v%3D%24fq_property%7D&fq_property=(property%3A%22refereed%22)&q=%20author%3A%22Agrusa%2C%20Harrison%22&sort=date%20desc%2C%20bibcode%20desc&p_=0).

As a grad student, my research has (mostly) focused on studying the dynamics of the Didymos binary asteroid in support of NASA's DART mission. The challenge with modeling the spin and orbital evolution of these small binary systems is that their shapes are irregular and the two components are close together, meaning the system has a high degree of spin-orbit coupling and that the dynamics are non-Keplerian. 



Here's an old gif where we simulated the Didymos system using pkdgrav, a parallel n-body code:
![gif](../images/research/pkdgrav_binary_orbit.gif)
 <!-- In my first paper, we benchmarked several codes and studied the sensitivity of the Didymos system to changes in initial conditions. Based on the findings of the benchmarking paper, we then studied the post-impact attitude evolution of Dimorphos as a function of its (unkown) shape and the momentum enhancement factor, ![\Large \beta](https://latex.codecogs.com/svg.latex?\Large&space;\beta). -->


Here's a movie where we simulate the dynamical evolution of the Didymos system following a DART-like impact. This animation shows the secondary component (Dimorphos) librating now that its orbit has become eccentric. Near the 1 minute mark, you can see Dimorphos become attitude unstable. The attitude stability properties are highly dependent on its shape and the magnitude of the perturbation provided by DART. We studied Dimorphos' post-impact attitude stability in-depth in this [paper](https://ui.adsabs.harvard.edu/abs/2021Icar..37014624A/abstract) if you want to learn more!
<iframe width="1120" height="630" src="https://www.youtube.com/embed/ZkdqxPbH5Pg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<!-- ![\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}](https://latex.codecogs.com/svg.latex?\Large&space;x=\frac{-b\pm\sqrt{b^2-4ac}}{2a})  -->




<!-- 
## Publications (peer reviewed)

{% assign thumbnail="left" %}

{% for pub in page.pubs %}
{% if pub.image %}
{% include image.html url=pub.image caption="" height="100px" align=thumbnail %}
{% endif %}
[**{{pub.title}}**]({% if pub.internal %}{{pub.url | prepend: site.baseurl}}{% else %}{{pub.url}}{% endif %})<br />
{{pub.author}}<br />
*{{pub.journal}}*
{% if pub.note %} *({{pub.note}})*
{% endif %} *{{pub.year}}* {% if pub.doi %}[[doi]({{pub.doi}})]{% endif %}
{% if pub.media %}<br />Media: {% for article in pub.media %}[[{{article.name}}]({{article.url}})]{% endfor %}{% endif %}

{% endfor %} -->
