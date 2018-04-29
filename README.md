# TrainsAndTowns
Coding task regarding Graph

 *  Compilation:  `javac Main.java`
 *  Execution:    `java Main "AB5, BC4, CD8, DC8, DE6, AD5, CE2, EB3, AE7"`

### Description:
The local commuter railroad services a number of towns in Azerbaijan. Because of monetary concerns, all of the tracks are 'one-way.' That is, a route from `A` to `B` does not imply the existence of a route from `B` to `A`.
In fact, even if both of these routes do happen to exist, they are distinct and are not necessarily _the same distance_!

The purpose of this problem is to help the railroad provide its customers with information about the routes.
In particular, you will compute the
<ul>
 	<li>distance along a certain route,</li>
 	<li>the number of different routes between two towns,</li>
 	<li>and the shortest route between two towns.</li>
</ul>
&nbsp;

<strong>Input:</strong> A directed graph where a node represents a town and an edge represents a route between two towns. The weighting of the edge represents the distance between the two towns. A given route will never appear more than once, and for a given route, the starting and ending town will not be the same town.

<strong>Output:</strong> For test input 1 through 5, if no such route exists, output <code>'NO SUCH ROUTE'</code>. Otherwise, follow the route as given; do not make any extra stops! For example, the first problem means to start at city <code>A</code>, then travel directly to city <code>B</code> (a distance of 5), then directly to city <code>C</code> (a distance of 4).

<p><strong>1.</strong> The distance of the route <code>A-B-C</code>.</p>
<p><strong>2.</strong> The distance of the route <code>A-D</code>.</p>
<p><strong>3.</strong> The distance of the route <code>A-D-C</code>.</p>
<p><strong>4.</strong> The distance of the route <code>A-E-B-C-D</code>.</p>
<p><strong>5</strong>. The distance of the route <code>A-E-D</code>.</p>
<p><strong>6.</strong> The number of trips starting at <code>C</code> and ending at <code>C</code> with a maximum of <code>3</code> stops. In the sample data below, there are two such trips: <code>C-D-C</code> (2 stops) and <code>C-E-B-C</code> (3 stops).</p>
<p><strong>7.</strong> The number of trips starting at <code>A</code> and ending at<code> C</code> with exactly <code>4</code> stops. In the sample data below, there are three such trips: <code>A</code> to <code>C</code> (via <code>B</code>, <code>C</code>, <code>D</code>); <code>A</code> to <code>C</code> (via <code>D</code>, <code>C</code>, <code>D</code>);
and <code>A</code> to <code>C</code> (via <code>D</code>, <code>E</code>, <code>B</code>).</p>
<p><strong>8.</strong> The length of the shortest route (in terms of distance to travel) from <code>A</code> to <code>C</code>.</p>
<p><strong>9.</strong> The length of the shortest route (in terms of distance to travel) from <code>B</code> to <code>B</code>.</p>
<p><strong>10.</strong>The number of different routes from <code>C</code> to <code>C</code> with a distance of less than <code>30</code>. In the sample data, the trips are:
<code>CDC</code>,<code> CEBC</code>,<code> CEBCDC</code>,<code> CDCEBC</code>,<code> CDEBC</code>,<code> CEBCEBC</code>,<code> CEBCEBCEBC</code>.</p>

&nbsp;

<strong>Test Input:</strong>
For the test input, the towns are named using the first few letters of the alphabet from <code>A</code> to <code>E</code>. A route between two towns (<code>A</code> to <code>B</code>) with a distance of <code>5</code> is represented as <code>AB5</code>.
<p><code>Graph: AB5, BC4, CD8, DC8, DE6, AD5, CE2, EB3, AE7</code></p>

<strong>Expected Output:</strong>
* Output #1:    <code>9</code>
* Output #2:    <code>5</code>
* Output #3:    <code>13</code>
* Output #4:    <code>22</code>
* Output #5:    <code>NO SUCH ROUTE</code>
* Output #6:    <code>2</code>
* Output #7:    <code>3</code>
* Output #8:    <code>9</code>
* Output #9:    <code>9</code>
* Output #10:  <code>7</code>

