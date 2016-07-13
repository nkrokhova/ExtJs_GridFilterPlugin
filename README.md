<br>
<h1>Ext.ux.grid.GridFilter</h1>

<br>
  Grid plugin that adds a filtering row below grid header.
  Allows remote filtering, supports pagination grids.
<br>
  Copyright 2016 Roberto Rodriguez
<br>

<img src="http://res.cloudinary.com/titorobe/image/upload/v1468251216/ExtJs_GridFilterPlugin_ow2bvv.jpg"></img>

<br>

<h2>How it works</h2>

To add filtering to column, define "filter" property in the column configuration

When the user adds criterias to the filter and hits enter,
  The plugin reload the grid, including in the query params the values of the filters
  
  The values are collected just for the filters that are not empty,
  and are sent to the server in the format:
  dataIndex:VALUE    // Example  firstName: 'Roberto'
<br>
<br>
  Copyright 2016 Roberto Rodriguez
  <br>
  Email: robertoSoftwareEngineer@gmail.com
<br>
  Example:
<pre><code>
  var grid = new Ext.grid.GridPanel({
  columns: [
     {
        text: "User ID",
        dataIndex: 'userId', 
        filter: true
    },
    {
        text: "First Name",
        dataIndex: 'firstName', 
        filter: true
    },
    {
        text: "First Name",
        dataIndex: 'firstName', 
        filter: lastName
    }
  ],
  plugins:[{ptype:"gridFilter"}]
  ...
});
</code></pre>


<br>

<p2>Change Logs</p2>
<ul>
<li><p>0.1 version</p>

<ul>
	<li>Initial Commit</li>
</ul>

</ul>