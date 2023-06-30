---
layout: page
title: UW-Madison Data Science Institute
description: UW-Madison Data Science Institute
img: assets/img/University-of-Wisconsin-logo.png
importance: 1
category: 2023
---

Here is a list of example of a commitments. 

 * Membership in the NumFOCUS Academic Consortium
 * Direct contribution to software
    * Join a network of emergency / backup maintainers that can step in triage style for projects that lost maintainer (e.g. due to personal reasons, change in circumstances, etc.)
    * Contribute to documentation
    * updating documentation to keep it up to date with current releases
    * contributing to technical writing 
    * submitting issues highlighting areas where documentation could be improved together with concrete suggestions
 * Project management tasks
    * Running meetings for maintainers, note taking, etc.
    * Updating Kanban boards and other project management tools
 * Community support
    * Social media
    * Running trainings
 * Space 
    * Provide office to core developers and project maintainers
    * Provide meeting rooms for project meetings, code sprints, etc.
    * Contributions targeting digital accessibility and interoperability with assistive technologies.


# Example contributions to Open Source (Optional) 

It's not clear we want to do any or all of this, but let's try exercising the functionality of the `al-folio` theme. This is generated automatically from the data in the `uw-madison-repositories.yml` file in the [`_data` directory](https://github.com/cranmer/open-source-pledge/tree/master/_data).

## GitHub users

{% if site.data.uw-madison-repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.uw-madison-repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.uw-madison-repositories.github_users %}
  {% if site.data.uw-madison-repositories.github_users.size > 1 %}
  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.html username=user %}
  </div>

  ---

{% endfor %}
{% endif %}
{% endif %}

## GitHub Repositories

{% if site.data.uw-madison-repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.uw-madison-repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}