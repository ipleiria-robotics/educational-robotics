---
layout: default
datatable: true
---

<script type="text/javascript" src="js/datatable.min.js"></script>
//cdn.datatables.net/1.10.16/css/jquery.dataTables.min.css
<script>


var datatable = new DataTable(document.querySelector('#first-datatable-output table'), {
    pageSize: 5,
    sort: [true, true, false],
    filters: [true, false, 'select'],
    filterText: 'Type to filter... ',
    pagingDivSelector: "#paging-first-datatable"
});


</script>

<table class="table table-bordered">
    <thead>
        <tr>
            <th>Firstname</th>
            <th>Lastname</th>
            <th></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Linus</td>
            <td>Torvalds</td>
            <td>Computer Science</td>
        </tr>
        <tr>
            <td>Brian</td>
            <td>Kernighan</td>
            <td>Computer Science</td>
        </tr>
        <tr>
            <td>Blaise</td>
            <td>Pascal</td>
            <td>Mathematics</td>
        </tr>
        <tr>
            <td>Larry</td>
            <td>Page</td>
            <td>Computer Science</td>
        </tr>
        <tr>
            <td>Richard</td>
            <td>Hamming</td>
            <td>Mathematics</td>
        </tr>
        <tr>
            <td>Grace</td>
            <td>Hopper</td>
            <td>Computer Science</td>
        </tr>
        <tr>
            <td>Pierre</td>
            <td>Bezier</td>
            <td>Mathematics</td>
        </tr>
        <tr>
            <td>Shigeru</td>
            <td>Miyamoto</td>
            <td>Computer Science</td>
        </tr>
        <tr>
            <td>Leslie</td>
            <td>Lamport</td>
            <td>Computer Science</td>
        </tr>
        <tr>
            <td>Rasmus</td>
            <td>Lerdorf</td>
            <td>Computer Science</td>
        </tr>
        <tr>
            <td>Xavier</td>
            <td>Leroy</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Albert</td>
            <td>Einstein</td>
            <td>Physics</td>
		</tr>
        <tr>
            <td>Bill</td>
            <td>Gates</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Leonard</td>
            <td>De Vinci</td>
            <td>Mathematics</td>
		</tr>
        <tr>
            <td>Pierre</td>
            <td>De Fermat</td>
            <td>Mathematics</td>
		</tr>
        <tr>
            <td>René</td>
            <td>Descartes</td>
            <td>Mathematics</td>
		</tr>
        <tr>
            <td>Alan</td>
            <td>Turing</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Ada</td>
            <td>Lovelace</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Isaac</td>
            <td>Newton</td>
            <td>Physics</td>
		</tr>
        <tr>
            <td>Carl Friedrich</td>
            <td>Gauss</td>
            <td>Mathematics</td>
		</tr>
        <tr>
            <td>John</td>
            <td>Von Neumann</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Claude</td>
            <td>Shannon</td>
            <td>Mathematics</td>
		</tr>
        <tr>
            <td>Tim</td>
            <td>Berners-Lee</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Richard</td>
            <td>Stallman</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Dennis</td>
            <td>Ritchie</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Bjarne</td>
            <td>Stroustrup</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Steve</td>
            <td>Jobs</td>
            <td>Computer Science</td>
		</tr>
        <tr>
            <td>Steve</td>
            <td>Wozniak</td>
            <td>Computer Science</td>
		</tr>        <tr>
            <td>Mario</td>
            <td>Molina</td>
            <td>Chemistry</td>
        </tr>
    </tbody>
</table>
<div id="paging-first-datatable"></div>
