---
layout: default
---

## Welcome to another page

_yay_

{% assign mydata=site.data.data-software %}

<table>
    <caption>Table caption</caption>
    <thead>
    {% for column in mydata[0] %}
	    {% if forloop.index == 2 %}
            {% continue %}
	    {% else %}
            <th>{{ column[0] }}</th>
        {% endif %}
    {% endfor %}
    </thead>
    <tbody>
    {% for row in mydata %}
        <tr>
        <td><a href="{{ row.Link }}">{{ row.Project }}</a></td>
        {% for cell in row offset: 2 %}
            <td>{{ cell[1] }}</td>
        {% endfor %}
        </tr>
    {% endfor %}
    </tbody>
</table>



[back](./)