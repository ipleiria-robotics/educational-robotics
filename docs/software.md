---
layout: default
datatable: true
---

## Software resources data table

Below you find a summary table with existing software resources for programming and teaching robotics for K-12 studends. You can search by column or the entire table. The column search is only applied when you press ENTER.

This is a community effort, so your help in keeping this information up to date is important. Please check the help page to see how you can contribute.

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