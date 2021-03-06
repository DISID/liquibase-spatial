Precondition: 'Spatial Index Exists'
------------------------------------

This precondition passes if the specified spatial index exists in the database.

<h3>Available Attributes</h3>
<table>
   <tr>
      <th>Attribute</th>
      <th>Description</th>
   </tr>
   <tr>
      <td>schemaName</td>
      <td>The name of the index's schema.</td>
   </tr>
   <tr>
      <td>indexName</td>
      <td>The name of the index.</td>
   </tr>
   <tr>
      <td>tableName</td>
      <td>The name of the table. <b>Required for Derby and H2.</b></td>
   </tr>
   <tr>
      <td>columnNames</td>
      <td>The name of the indexed column(s).</td>
   </tr>
</table>

<h3>Example</h3>
```XML
<preConditions>
   <spatial:spatialIndexExists tableName="SPATIAL_TABLE" columnNames="GEOMETRY_COLUMN" />
</preConditions>
```
