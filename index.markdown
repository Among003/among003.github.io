---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: single
tagline: "**\"You must always be curious.\"** <br/> -_Walt Whitman_"
title: About me
header:
  overlay_image: /assets/img/heading1.jpg
author_profile: true
author:  
  name: "Adrian Monges Rodriguez"
  avatar: "assets/img/profilepic.jpg"
  bio: "Computer Engineer B.S,  <br />Computer Science M.S. <br />**Always building cool stuff**"
  location: "Riverside County"
  links :
    - label: "LinkedIn"
      icon:  "fab fa-brands fa-linkedin"
      url:   "https://www.linkedin.com/in/adrian-monges-rodriguez-a904b0163/" 
            

---
## Hello 
I'm Adrian. I am a computer science and engineering graduate from the University of California, Riverside.

I generally program in C and C++, but love to reach out into other areas as well (check out my projects).
  
When I'm not programming, I'm usually playing guitar, walking my dog, or playing tennis.


## Education
{% for education in site.education %}
### {{education.school}} 
**{{education.degree}}** - ({{education.graduation_date}}) <br/> 
*{{education.subject}} - {{education.GPA}}*
{% endfor %}

## Work Experience
{% for experience in site.work_experience %}
### {{ experience.name }}  
  <details>
  <summary>
  {{ experience.position }} | {{experience.start_date}} - {{experience.end_date}} </summary>
 <p>{{ experience.content | markdownify }}</p>
  </details>
{% endfor %}
