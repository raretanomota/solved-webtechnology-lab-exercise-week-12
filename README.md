Download Link: https://assignmentchef.com/product/solved-web_technology-lab-exercise-week-12
<br>
<strong>Question 1.</strong> Create a web page and display the following:​

The web page allows the user to enter the coordinates of the 3 vertices of a triangle.

When the user clicks the button, then draw the triangle on the canvas as above.

A median of a triangle is a straight line from a vertex to the midpoint of the opposite side. The drawing demonstrates a mathematical fact that: the 3 median lines intersect in a single point (which is called the triangle’s centroid).

This is a sample code for draggable elements:

<table width="624">

 <tbody>

  <tr>

   <td width="624">&lt;tagName id=”…”           draggable=”true”           onDragStart=”dragStart(event)”&gt;…&lt;/tagName&gt; function dragStart(event){// get the drag element id   var dragId = event.target.id;console.log(“dragId=” + dragId); // store the drag element id into the dataTransfer object   event.dataTransfer.setData(“dragId”, dragId); }</td>

  </tr>

 </tbody>

</table>







This is a sample code for droppable elements:

<table width="624">

 <tbody>

  <tr>

   <td width="624">&lt;tagName id=”…”onDrop=”drop(event)”           onDragOver=”dragOver(event)”&gt;…&lt;/tagName&gt; function dragOver(event){event.preventDefault();}function drop(event){// get the drop element ID   var dropId = event.target.id;console.log(“dropId=” + dropId); // retrieve the drag element id from the dataTransfer object   var dragId = event.dataTransfer.getData(“dragId”);   console.log(“dragId=” + dragId); // do the dropping logic// TO-DO}</td>

  </tr>

 </tbody>

</table>

<strong>Question 2.</strong> Create a web page and display the following:​










When an animal is dropped into a matching text then the corresponding counter is increased by 1. For example, if the cat is dropped correctly 3 times and the dog is dropped correctly 11 times then the web page shows the following:

<strong>Question 3.</strong> Create a web page and display the following:​

When an animal is dropped into a matching text then the web page will be updated in the following manner. For example, if the cat is dropped correctly 2 times and the dog is dropped correctly 3 times then the web page shows the following: