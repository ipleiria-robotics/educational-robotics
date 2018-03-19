---
layout: default
---

## Welcome to another page

_yay_


<ol>
{% for item in site.data.data-software %}
  <li>
      {{ item.Project }}
  </li>
{% endfor %}
</ol>

{% assign mydata=site.data.data-software %}

<table>
    <caption>Table caption</caption>
    <thead>
        <th>{{ mydata[0] }}</th>
    {% for column in mydata[0]}
	{% if forloop.index == 1 %}
            <th>{{ column[0] }}</th>
	{% else %}
            <th>{{ column[0] }}</th>
        {% endif %}
    {% endfor %}
    </thead>
    <tbody>
    {% for row in mydata %}
        <tr>
	
	<td>{{ row.Project }}</td>
	<td>{{ row.Link }}</td>
        {% for cell in row offset:2 %}
            <td>{{ cell[1] }}</td>
        {% endfor %}
        </tr>
    {% endfor %}
    </tbody>
</table>



[back](./)