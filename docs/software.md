---
layout: default
datatable: true
---


## Welcome to another page

_yay_

<table id="sampleTable" class="display">
   <thead>
      <tr>
         <th>Parameter</th>
         <th>Description</th>
         <th>Type</th>
         <th>Default Value</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>Parameter 1</td>
         <td>Sample description
         </td>
         <td>Sample type</td>
         <td>Sample default value</td>
      </tr>
      <tr>
         <td>Parameter 2</td>
         <td>Sample description
         </td>
         <td>Sample type</td>
         <td>Sample default value</td>
      </tr>
    <tr>
       <td>Parameter 3</td>
       <td>Sample description
       </td>
       <td>Sample type</td>
       <td>Sample default value</td>
    </tr>
      <tr>
         <td>Parameter 4</td>
         <td>Sample description
         </td>
         <td>Sample type</td>
         <td>Sample default value</td>
      </tr>
   </tbody>
</table>




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



<script>
$(document).ready(function(){

    $('table.display').DataTable( {
        paging: true,
        stateSave: true,
        searching: true
    }
        );
});
</script>

[back](./)