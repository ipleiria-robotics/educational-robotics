---
layout: default
datatable: true
---

## Software resources data table

Below you find a table collecting and compating existing software resources for programming and teaching robotics for K-12 studends. You can search by column or the entire table (using the box in the top right of the table), or make individual column searches by inputing text in the box above each collumn (this search is only applied when you press ENTER).

This is a community effort, so your help in keeping this information up to date is important. Please check theContributors Manual to see how you can help.

The following applies to the entire table:

{% assign mydata=site.data.data-software %}

<table id="datatable" class="display">
    <!-- <caption>Software table</caption> -->
    <thead>
        <tr>
        {% for column in mydata[0] %}
            {% if forloop.index == 2 %}
                {% continue %}
            {% else %}
                <th>{{ column[0] }}</th>
            {% endif %}
        {% endfor %}
        </tr>
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