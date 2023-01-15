<h1 style="color:green;">
    GeeksforGeeks
</h1>
  
<table>
  
    <tr>
        <th>S.No</th>
        <th>Title</th>
        <th>Geek_id</th>
    </tr>
    <tr id="row1">
        <td>Geek_1</td>
        <td>GeekForGeeks</td>
        <th>Geek_id_1</th>
    </tr>
    <tr>
        <td>Geek_2</td>
        <td>GeeksForGeeks</td>
        <th>Geek_id_2</th>
    </tr>
    <tr>
        <td>Geek_3</td>
        <td>GeeksForGeeks</td>
        <th>Geek_id_2</th>
    </tr>
    <tr>
        <td>Geek_4</td>
        <td>GeeksForGeeks</td>
        <th>Geek_id_2</th>
    </tr>
</table>
<br>
  
<button onclick="Geeks()">
    Click here
</button>
  
<script>
    function Geeks() {
        document.getElementsByTagName("tr")[3].remove();
    }
</script>