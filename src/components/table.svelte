<table>
	<thead>
	<tr>
		<th>Centimeters</th>
		<th>Inches</th>
	</tr>
	</thead>
	<tbody>
	<tr>
		<td>1</td>
		<td>0.3937008</td>
	</tr>
	<tr>
		<td>2</td>
		<td>0.7874016</td>
	</tr>
    <tr>
		<td>3</td>
		<td>1.1811024</td>
	</tr>
    <tr>
		<td>4</td>
		<td>1.5748031</td>
	</tr>
    <tr>
		<td>5</td>
		<td>1.5748031</td>
	</tr>
    <tr>
		<td>6</td>
		<td>2.3622047</td>
	</tr>
    <tr>
		<td>7</td>
		<td>2.7559055</td>
	</tr>
    <tr>
		<td>8</td>
		<td>3.1496063</td>
	</tr>
    <tr>
		<td>9</td>
		<td>3.5433071</td>
	</tr>
    <tr>
		<td>10</td>
		<td>3.9370079</td>
	</tr>
    <tr>
		<td>11</td>
		<td>4.3307087</td>
	</tr>
    <tr>
		<td>12</td>
		<td>4.7244094</td>
	</tr>
    <tr>
		<td>13</td>
		<td>5.1181102</td>
	</tr>
    <tr>
		<td>14</td>
		<td>5.511811</td>
	</tr>
    <tr>
		<td>15</td>
		<td>5.511811</td>
	</tr>
	</tbody>
</table>

<style>
table {
  float: right; 
  width: 35%; 
  border-collapse: collapse; 
  margin: 8rem;
}
/* Zebra striping */
tr:nth-of-type(odd) { 
  background: #eee; 
}
th { 
  background: #333; 
  color: white; 
  font-weight: bold; 
}
td, th { 
  padding: 12px 20px; 
  border: 1px solid #ccc; 
  text-align: left; 
}
@media 
only screen and (max-width: 760px),
(min-device-width: 768px) and (max-device-width: 1024px)  {

	/* Force table to not be like tables anymore */
	table, thead, tbody, th, td, tr { 
		display: block; 
	}
	
	/* Hide table headers (but not display: none;, for accessibility) */
	thead tr { 
		position: absolute;
		top: -9999px;
		left: -9999px;
	}
	
	tr { border: 1px solid #ccc; }
	
	td { 
		/* Behave  like a "row" */
		border: none;
		border-bottom: 1px solid #eee; 
		position: relative;
		padding-left: 50%; 
	}
	
	td:before { 
		/* Now like a table header */
		position: absolute;
		/* Top/left values mimic padding */
		top: 6px;
		left: 6px;
		width: 45%; 
		padding-right: 10px; 
		white-space: nowrap;
	}
	
	/*
	Label the data
	*/
	td:nth-of-type(1):before { content: "Centimeters"; }
	td:nth-of-type(2):before { content: "Inches"; }
}
</style>

<script>
    
</script>