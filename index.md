---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{% assign image_files = site.static_files | where: "image", true %}





<style>
	.video-wrapper{
		float: none;
		width: 560px;
		margin: 0 auto;
		max-width: 100%;
	}
	.img-wrapper{
		float: none;
		width: 560px;
		margin: 0 auto;
		max-width: 100%;
	}
</style>
<div class='video-wrapper'>
<iframe width="560" height="315" src="https://www.youtube.com/embed/aDcKEEXl-2I?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<h1></h1>

<strong>CodingStrip</strong> is a proof-of-concept programming learning environment that implements <strong>concreteness fading</strong> for effective learning and teaching of programming and its concepts. 


{% for image in image_files %}
{% if image.basename == "concreteness_fading" %}
<img src="{{image.path}}">
{% endif %}
{% endfor %}

As shown above, <strong>concreteness fading</strong> progresses gradually from the <i>concrete</i> to the <i>abstract</i> stage, for the optimal learning and teaching of abstract ideas or concepts. 

Likewise, <strong>CodingStrip</strong> presents programming and its concepts from the <i>concrete</i> to the <i>abstract</i> stage. The image below demonstrates the high-level overview of the progression.

<br>
{% for image in image_files %}
{% if image.basename == "codingstrip" %}
<img src="{{image.path}}">
{% endif %}
{% endfor %}


Since images of each stage above are too small to see, we provide below the representations of each stage. The materials below teach the concept of double recursion. 

<br><br><br>
For the <strong>concrete representation</strong>, we chose comics, because, among many reasons, they are a powerful, interactive medium that delivers a "concrete" experience for readers.

{% for image in image_files %}
{% if image.basename == "comic" %}
<img src="{{image.path}}" style="width:100%">
{% endif %}
{% endfor %}


<br><br><br>
For the <strong>intermediate representation</strong>, we show a visualization of the drawing in the comic with the narrative details stripped away.  For example, as users step through the tree diagram visualization, the phrase "What is my bonus?"" is displayed, referencing the panel in the comic showing the mentees in an organizational hierarchy, and illustrating the recursive process mentioned in the abstract representation.
{% for image in image_files %}
{% if image.basename == "visualization" %}
<div class='img-wrapper'><img src="{{image.path}}"></div>
{% endif %}
{% endfor %}

<br><br><br>
For the <strong>concrete-code representation</strong>, we show the code where the function and variable names (e.g., `what\_is\_ my\_bonus`, `years\_of\_service`) closely maps to the comic and visualization.  At this stage, learners are asked to work with code without the support of the more concrete representations in the previous stages.  
{% for image in image_files %}
{% if image.basename == "concrete-code" %}
<div class='img-wrapper'><img src="{{image.path}}"></div>
{% endif %}
{% endfor %}

<br><br><br>
For the <strong>abstract-code representation</strong>, the interface presents code that has the same logic as the concrete code, but with abstract notations and names, such as `x` and `function`, for function and variable names, and without any reference to the previous narrative. 
{% for image in image_files %}
{% if image.basename == "abstract-code" %}
<div class='img-wrapper'><img src="{{image.path}}" style="width:65%"></div>
{% endif %}
{% endfor %}

<br><br><br>
Our findings show that <strong>CodingStrip</strong> can help learners understand programming constructs by leveraging multiple representations, and foster self-efficacy in novice learners.  Results also suggest that how users respond to concreteness fading can vary depending on their learning style preferences.




