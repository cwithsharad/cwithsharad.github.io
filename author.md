---
title: Author[s]
layout: default
description: A site dedicated to Computer Science and Technnology.It was Launched in 2017 for helping the students of Lucknow University in finding all the programs related to their course on a single site. The thought of launching this website came when I felt the need of a source which can help me in finding the programs related to my course and I saw that most of the sites or the blogs available are not that much oriented towards courses of Lucknow University, and  there are hardly few blogs or websites which are providing content for the students in Lucknow University.
---

 <h2 class="display-3" style="color:white!important">  Hi! there Folks, this is {{ site.author.name }}</h2>
  <p class="lead" style="color:blue!important">{{ site.author.description }}</p>

### Reason behind starting this blog

I felt the need of a source which can help me in finding the programs related to my course and I saw that most of the sites or the blogs available are not that much oriented towards courses of Lucknow University, and  there are hardly few blogs or websites which are providing content for the students in Lucknow University.

  <hr class="my-4">
  <h5 class="display-3">Skills</h5>
<div class="row">  
  {% for skill in site.skills %}
	<h6 style="color:white!important">{{ skill.title }} | {{skill.level}}%</h6>
		<div class="col-lg-12">
			<div class="progress progress-striped active">
				<div class="progress-bar progress-bar-{{skill.color}}" style="width: {{skill.level}}%"></div>
			</div>
		</div>	
{% endfor %}		
</div>	
