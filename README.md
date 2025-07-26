# 📝 Daily Habit Tracking
<h2>📌 Project Description:</h2>
<p>This project uses the Pixela API to track daily activities (e.g., cycling distance) visually via a graph. Users can create a profile, generate a graph, and log (or update/delete) data entries on a specific date. The data is displayed on a graph which Pixela hosts and updates automatically.</p>
<h3>🛠️ Python Modules Used</h3>
<ul>
  <li><strong>requests:</strong>	Used to send HTTP requests (POST, PUT, DELETE) to the Pixela API.</li>
  <li><strong>datetime:</strong>	To get the current date in YYYYMMDD format required by the API.</li>
</ul>
<h3>Pixela API Endpoints Used</h3>
<table>
  <thead>
    <tr>
      <th>Operation</th>
      <th>Method</th>
      <th>Endpoint</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Create User</td>
      <td><code>POST</code></td>
      <td><code>https://pixe.la/v1/users</code></td>
    </tr>
    <tr>
      <td>Create Graph</td>
      <td><code>POST</code></td>
      <td><code>https://pixe.la/v1/users/&lt;USERNAME&gt;/graphs</code></td>
    </tr>
    <tr>
      <td>Add Pixel (Entry)</td>
      <td><code>POST</code></td>
      <td><code>https://pixe.la/v1/users/&lt;USERNAME&gt;/graphs/&lt;GRAPH_ID&gt;</code></td>
    </tr>
    <tr>
      <td>Update Pixel</td>
      <td><code>PUT</code></td>
      <td><code>https://pixe.la/v1/users/&lt;USERNAME&gt;/graphs/&lt;GRAPH_ID&gt;/&lt;DATE&gt;</code></td>
    </tr>
    <tr>
      <td>Delete Pixel</td>
      <td><code>DELETE</code></td>
      <td><code>https://pixe.la/v1/users/&lt;USERNAME&gt;/graphs/&lt;GRAPH_ID&gt;/&lt;DATE&gt;</code></td>
    </tr>
  </tbody>
</table>









<p><strong>Operation</strong><strong>    Method</strong><strong>   Endpoint</strong></p>
<p>Create User	   POST	   https://pixe.la/v1/users</p>
<p>Create Graph	   POST	   https://pixe.la/v1/users/<USERNAME>/graphs</p>
<p>Add Pixel (Entry)	   POST	   https://pixe.la/v1/users/<USERNAME>/graphs/<GRAPH_ID></p>
<p>Update Pixel	   PUT	   https://pixe.la/v1/users/<USERNAME>/graphs/<GRAPH_ID>/<DATE></p>
<p>Delete Pixel	   DELETE	   https://pixe.la/v1/users/<USERNAME>/graphs/<GRAPH_ID>/<DATE></p>







Important Links
✅ Pixela API Documentation: https://docs.pixe.la/

📊 Graph Visualization Example:
After creating the graph, you can visit your graph at:

bash
Copy
Edit
https://pixe.la/v1/users/<USERNAME>/graphs/<GRAPH_ID>.html
For your case:

bash
Copy
Edit
https://pixe.la/v1/users/shahbaz123/graphs/graph1.html
