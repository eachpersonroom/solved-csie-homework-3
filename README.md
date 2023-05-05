Download Link: https://assignmentchef.com/product/solved-csie-homework-3
<br>



<h1>Problem 1 – ADA Adventurer (Programming)</h1>

<h2>Problem Description</h2>

ADA Road, a prosperous country, was established by the ancestors’ wisdom long time ago. This country consists of <em>N </em>cities indexed from 1 to <em>N </em>and (<em>N </em>−1) roads. Each road connects two different cities, and all cities are connected. More formally, for any two different cities, a path exists from one to another along the given roads, and the distance between two cities is defined as the number of roads on this path.

To become a valiant ADA adventurer, you decided to visit this country. After arriving at the ADA Road, you discovered that the distance of some city pairs is too large, so villages need to pay lots of effort to reach one from another. To help the villages and get the experience points, you would like to help them resolve this problem. The only stuff allowed is to rebuild at most one road. That is, you can only remove at most one road from this country, and find a new pair of cities to build a road between them. The target is to minimize the farthest distance after rebuilding the road. Notice that you should avoid making some pairs of cities disconnected. Can you find the best way to complete it to win villages’ reliance?

<h2>Input</h2>

The first line only contains one integer <em>N</em>, describing the number of cities in ADA Road.

In the next <em>N </em>− 1 lines, each line contains two different integers <em>a,b </em>(1 ≤ <em>a,b </em>≤ <em>N</em>), describing a road connecting city <em>a </em>and <em>b</em>.

It is guaranteed that there exists a path from one city to another one for any pair of cities.

<table width="480">

 <tbody>

  <tr>

   <td width="328"><strong>Test Group 0 (0 %)</strong>•   Sample Input.<strong>Test Group 1 (20 %)</strong>•   2 ≤ <em>N </em>≤ 50.</td>

   <td width="152"><strong>Test Group 2 (30 %) </strong>• 2 ≤ <em>N </em>≤ 1000.<strong>Test Group 3 (50 %)</strong>• 2 ≤ <em>N </em>≤ 2 × 10<sup>5</sup>.</td>

  </tr>

 </tbody>

</table>

<strong>Output</strong>

Print one integer in a line, indicating the farthest distance after rebuilding the road.

<h2>Sample Input 1                                                        Sample Output 1</h2>

5                                                                                3

5 1

<ul>

 <li>1</li>

 <li>3</li>

</ul>

2 3

<h2>Sample Output 2 Sample Input 2</h2>

3

6

6 5

1 3

<ul>

 <li>2</li>

 <li>5</li>

</ul>

6 3

<h2>Sample Input 3                                                        Sample Output 3</h2>

10                                                                               4

8 3

2 8

7 9

6 5

4 6

9 1

3 10

3 5

2 9

<h1>Problem 2 –  kingdom</h1>

<h2>Problem Description</h2>

kingdom, a prosperous country, was established by the wisdom of the ancestors a long time ago.

This country consists of <em>N </em>cities indexed from 1 to <em>N </em>and <em>M </em>directed roads. Each road <em>e<sub>i </sub></em>connects two different cities <em>u<sub>i </sub></em>and <em>v<sub>i</sub></em>, indicating that you can visit city <em>v<sub>i </sub></em>from city <em>u<sub>i</sub></em>.

As a resident in the  kingdom, you find that there are specific cities where residents may not be able to visit all other cities in the  kingdom.

In order to meet everyone’s daily needs, you have to solve this problem by building new directed roads. Now you can propose a list of roads that need to be built and minimize the number of roads on the list.

<h2>Input</h2>

The first line contains two integers <em>T</em>, representing the number of test cases, and <em>flag </em>(<em>flag </em>∈ {0<em>,</em>1}), which will be described in the output section.

Each test case consists of two parts: the first line contains two space-separated integers <em>N,M</em>, representing the number of cities and the number of roads, respectively.

Each line of the following <em>M </em>contains two space-separated integers <em>u<sub>i </sub></em>and <em>v<sub>i</sub></em>, indicating a road connection from <em>u<sub>i </sub></em>to <em>v<sub>i</sub></em>.

<ul>

 <li>1 ≤ <em>N </em>≤ 1000</li>

 <li>0 ≤ <em>M </em>≤ min(1000<em>,N </em>× (<em>N </em>− 1))</li>

 <li>1 ≤ <em>u<sub>i </sub></em>≤ <em>N</em></li>

 <li>1 ≤ <em>v<sub>i </sub></em>≤ <em>N</em></li>

 <li><em>u<sub>i </sub></em>6= <em>v<sub>i</sub></em></li>

</ul>

It is guaranteed that the sum of <em>N </em>does not exceed 3000 and the sum of <em>M </em>does not exceed 3000.

<strong>Test Group 0 (0 %)                                                                               Test Group 2 (30 %)</strong>

<ul>

 <li><em>flag </em>= 0 Sample Input.</li>

</ul>

<strong>Test Group 3 (20 %)</strong>

<ul>

 <li><em>u<sub>i </sub>&lt; v<sub>i </sub></em><strong>Test Group 1 (30 %)</strong></li>

 <li><em>flag </em>= 0 <strong>Test Group 4 (20 %)</strong></li>

 <li><em>u<sub>i </sub>&lt; v<sub>i </sub></em> No additional constraints.</li>

</ul>

<strong>Bonus Group (2 points)</strong>

<ul>

 <li><em>N,M </em>≤ 100000</li>

 <li>The sum of <em>N </em>does not exceed 100000 and the sum of <em>M </em>does not exceed 100000.</li>

</ul>

<h2>Output</h2>

For each testcase, print an integer on the first line representing the number of roads <em>K </em>that need to be built.

If the <em>flag </em>mentioned in the input section is equal to 1, please furthermore print the following <em>K </em>lines: each line contains <em>s<sub>i </sub></em>and <em>t<sub>i</sub></em>, representing building a road from <em>s<sub>i </sub></em>to <em>t<sub>i </sub></em>in the list. If there are multiple ways to match this condition, you can print any of them.

<h2>Sample Input 1                                                        Sample Output 1</h2>

1 0                                                                              2

4 2

1 2

3 4

<h2>Sample Input 2                                                        Sample Output 2</h2>

2 1                                                                              3

5 2                                                                              2 3

1 2                                                                              4 5

3 4                                                                              5 1

3 3                                                                              0

<ul>

 <li>2</li>

 <li>3</li>

 <li>1</li>

</ul>

<h1>Problem 3 – I Want It All!!! (Programming)</h1>

<h2>Problem Description</h2>

Xiao Feng and Baluteshih are learning graph theory together from <strong>W</strong><strong>aynetu</strong>, a legendary grandmaster in graph theory. To make sure that they have good learning efficiency, <strong>W</strong><strong>aynetu </strong>decided to assign homework to them. The homework is described as follow:

Xiao Feng and Baluteshih are working on this homework together. Xiao Feng loves shortest-path trees, so he would like to find a shortest path tree starting from vertex 1. However, Baluteshih loves minimum spanning trees, so he would like to find a minimum spanning tree of the given graph. Please help Xiao Feng and Baluteshih to find a spanning tree that satisfies both of their preferences simultaneously or determine that it is impossible.

<h2>Input</h2>

The first line contains two integers <em>N,M</em>, describing the number of the vertices and the edges of the graph. The vertices are indexed from 1 to <em>N</em>.

In the next <em>M </em>lines, the <em>i</em><sup>th </sup>line contains three integers <em>a<sub>i</sub>,b<sub>i</sub>,c<sub>i</sub></em>, describing an undirected edge with index <em>i </em>which connects the vertices <em>a<sub>i </sub></em>and <em>b<sub>i </sub></em>with weight <em>c<sub>i</sub></em>.

It is guaranteed that the input forms a connected graph.

<strong>Test Group 0 (0 %)                                                                                       </strong>• 1 ≤ <em>c<sub>i </sub></em>≤ 10<sup>9</sup>.

<ul>

 <li>All <em>c<sub>i </sub></em>are distinct.</li>

 <li>Sample Input.</li>

</ul>

<strong>Test Group 2 (60 %)</strong>

<strong>Test Group 1 (40 %)                                                                                                                  </strong><sup>5</sup>.

<ul>

 <li>1 ≤ <em>N </em>≤ 10</li>

 <li>1 ≤ <em>N </em>≤ 10<sup>5</sup>. 0 ≤ <em>M </em>≤ 3 × 10<sup>5</sup>.</li>

 <li>0 ≤ <em>M </em>≤ 3 × 10<sup>5</sup>. 1 ≤ <em>a<sub>i</sub>,b<sub>i </sub></em>≤ <em>N,a<sub>i </sub></em>6= <em>b<sub>i</sub></em>.</li>

 <li>1 ≤ <em>a<sub>i</sub>,b<sub>i </sub></em>≤ <em>N,a<sub>i </sub></em>6= <em>b<sub>i</sub></em>. 1 ≤ <em>c<sub>i </sub></em>≤ 10<sup>9</sup>.</li>

</ul>

<h2>Output</h2>

If Xiao Feng and Baluteshih cannot find the same spanning tree of the input graph, please print “No” (without quotes) in the first line.

Otherwise, please print “Yes” (without quotes) in the first line. In the second line, please print <em>n</em>−1 integers, describing indices of the chosen edges of the spanning tree. If there are multiple choices of the spanning trees, you may print any of them.

<h2>Sample Input 1                                                        Sample Output 1</h2>

5 6                                                                              Yes

1 2 1                                                                             1 2 3 4

<ul>

 <li>3 2</li>

 <li>5 3</li>

</ul>

2 4 4

1 5 5

3 4 6

<h2>Sample Input 2                                                        Sample Output 2</h2>

7 9                                                                              Yes

5 7 3                                                                              1 2 3 4 5 9

3 2 4

1 4 18

3 4 17

2 5 10

1 5 49

1 3 35

3 5 14

6 5 19

<h2>Sample Input 3                                                        Sample Output 3</h2>

4 4                                                                             No

1 2 3

<ul>

 <li>3 5</li>

 <li>4 3</li>

 <li>4 1</li>

</ul>

<h2>Sample Input 4                                                        Sample Output 4</h2>

4 5                                                                              Yes

1 2 2                                                                            1 2 4

1 3 2

<ul>

 <li>4 4</li>

 <li>4 2</li>

 <li>4 2</li>

</ul>

<h2>Hint</h2>

<ol>

 <li>You may want to find “a shortest-path tree that forms a minimum spanning tree” instead of finding “a minimum spanning tree that forms a shortest-path tree”.</li>

 <li>Test Group 1 can only help you verify the correctness of your shortest-path tree and minimum spanning tree. Try not to regard it as a hint for full credit.</li>

</ol>

<h1>Problem 4 – Cats! (Programming) (13 points)</h1>

<h2>Problem Description</h2>

BB loves cats! There are <em>N </em>cats in his garden, and the cats are labeled from 1 to <em>N</em>. BB’s garden can be seen as a straight line, and the <em>i</em><sup>th </sup>cat is initially located at x-coordinate <em>x<sub>i</sub></em>.

Every once in a while, BB will place some food somewhere in the garden, which attracts some of the cats nearby. More precisely, there are <em>Q </em>sequential events, the <em>j</em><sup>th </sup>of which is of one of the two types:

<ul>

 <li>BB placed some food at x-coordinate <em>p<sub>j</sub></em>, and attracted all cats within radius <em>r<sub>j</sub></em>. That is, every cat within [<em>p<sub>j </sub></em>− <em>r<sub>j</sub>,p<sub>j </sub></em>+ <em>r<sub>j</sub></em>] moved to <em>p<sub>j</sub></em>.</li>

 <li>The <em>t<sub>j</sub></em><sup>th </sup>cat moved to x-coordinate</li>

</ul>

Unfortunately, BB feels like his garden might be a bit too crowded after some of the events. The cats might feel uncomfortable due to this. To try resolving this problem, BB would like to first know the <em>crowdedness </em>of his garden. <strong>He define </strong><em>crowdedness </em><strong>be the number of pairs </strong>(<em>i,j</em>)<strong>, </strong><em>i &lt; j</em><strong>, such that the </strong><em>i</em><strong><sup>th </sup>cat and the </strong><em>j</em><strong><sup>th </sup>cat are at the same location.</strong>

Please help BB find out the <em>crowdedness </em>after each event.

<h2>Input</h2>

The first line of the input contains two positive integers <em>N </em>and <em>Q</em>, denoting the number of cats on BB’s garden and the number of events, respectively.

The second line contains <em>N </em>space-separated integers <em>x</em><sub>1</sub><em>,x</em><sub>2</sub><em>,…,x<sub>N</sub></em>, denoting the initial x-coordinate of the cats.

Then <em>Q </em>lines follows. The <em>j</em>-th line of which is of one of the following two forms:

<ul>

 <li>1 <em>p<sub>j </sub>r<sub>j</sub></em>: BB placed some food at <em>p<sub>j </sub></em>with radius <em>r<sub>j</sub></em>.</li>

 <li>: The <em>t<sub>j</sub></em><sup>th </sup>cat moved to.</li>

</ul>

Note that the events happen one by one (i.e., the <em>j</em><sup>th </sup>event happens under the effect of all previous <em>j </em>− 1 events).

<ul>

 <li>1 ≤ <em>N,Q </em>≤ 10<sup>5</sup></li>

 <li></li>

 <li>1 ≤ <em>t<sub>j </sub></em>≤ <em>N</em></li>

</ul>

<h2>Output</h2>

Please output <em>Q </em>lines, where the <em>j</em><sup>th </sup>line denotes the <em>crowdedness </em>of BB’s garden after the <em>j</em><sup>th </sup>event.

<strong>Test Group 0 (0 %)                                                                               Test Group 1 (10 %)</strong>

<ul>

 <li>Sample Input <em>N,Q </em>≤ 100</li>

</ul>

<strong>Test Group 2 (20 %)                                                                           Test Group 3 (30 %)</strong>

<ul>

 <li><em>N,Q </em>≤ 5000 There are only events of type 1.</li>

</ul>

<strong>Test Group 4 (40 %)</strong>

<ul>

 <li>No Additional Constraint</li>

</ul>

<h2>Sample Input 1                                                        Sample Output 1</h2>

5 6                                                                              1

3 1 4 1 5                                                                      3

2 3 6                                                                           1

<ul>

 <li>2 1 3</li>

 <li>2 7 2</li>

 <li>3 2 10</li>

 <li>4 7</li>

</ul>

1 5 2

<h2>Sample Input 2                                                        Sample Output 2</h2>

8 5                                                                              2

1 1 2 3 5 8 13 21                                                          3

1 10 4                                                                         11

1 3 1                                                                           11

1 3 2                                                                           28

1 8 4

1 12 9

<h2>Hint</h2>

<ol>

 <li>STL is your good friend:

  <ul>

   <li>Use std::map or std::set to maintain the cats in ascending order of their x-coordinate.</li>

   <li>Use std::vector or std::list when you need arbitrary length array.</li>

   <li>Go to <a href="https://en.cppreference.com/w/">Cpp Reference</a> if you don’t know how to use an STL container or function.</li>

  </ul></li>

 <li>Be careful <strong>NOT </strong>to use std::endl since it might be very slow. Use ‘
’</li>

 <li>Let c be an std::map or std::set. Be careful <strong>NOT </strong>to use std::lower bound(c.begin(),</li>

</ol>

c.end(), x). Use c.lower bound(x) instead.

<ol start="4">

 <li>You should try to prove the time complexity of your code.</li>

 <li>The test data in Test Group 1 might be a lot weaker than other test groups. Passing this test group does not guaranteed your code is bug-free.</li>

</ol>

<h1>Problem 5 – Shi-Hei Robots (Hand-Written) (20 points)</h1>

<em>Note: In this problem, you </em><em>don’t have to write pseudocode as long as you clearly explain your method. If there are mistakes in your pseudocode, you will receive an additional penalty. You don’t have to prove the time complexity of your method unless the problem description asks you to do so.</em>

Stanley, Wang Jung Tsan (王榮燦), a famous video game streamer and a previous world champion of an online game, has always been accused of purchasing robots to boost his number of stream viewers. In fact, there are some “robots” watching him streaming — they are so-called “Shi-Hei robots.” “Shi-Hei robots (史黑機器人)” is a group of evil villains whose ultimate goal is to defame Stanley by convincing people that Stanley is buying robots. To be convincing, they always comment robot emojis in the chatroom so that they look like real robots. One day, you accidentally discover a secret of “Shi-Hei robots”: if a group member sees another group member that he/she knows to spam in the chatroom, he/she will continue commenting robot emojis, and eventually, they will be unstoppable. However, simply banning all of them is not feasible since Stanley is merciful and does not want to ban many people. As a MOD (moderator) of Stanley’s streaming channel, you must decide which member of “Shi-Hei robots” should be banned so that the villain group can be split into as many sub-groups as you can. If you can find out which member should be banned, you will receive a precious reward from Stanley — “Stanley Smile (王榮燦笑)”.

More precisely, we use <em>G</em>(<em>V,E</em>), an undirected graph, to denote the relationship among members of “Shi-Hei robots”. The goal is to find out the single vertex <em>v </em>∈ <em>V </em>whose removal from the graph split the graph into as many different connected components as possible.

In the following part of this problem, we will use <em>s</em>(<em>v,G</em>) to denote the number of connected components in the graph <em>G </em>after removing vertex <em>v </em>from <em>G</em>. You may assume that the initial graph <em>G </em>(before removing vertex) is connected, has at least two vertices, and is represented using the adjacency lists. Recall that you can output the neighbors of <em>v </em>in <em>O</em>(<em>deg</em>(<em>v</em>)) time and <em>deg</em>(<em>v</em>) in <em>O</em>(1) time for any vertex <em>v </em>∈ <em>V </em>when using the adjacency-list representation.

Here are the definitions of some terminologies used in this problem: For a tree <em>T</em>(<em>V,E</em>) with root vertex <em>r</em>, “the <em>ancestors </em>of vertex <em>v</em>” denotes all vertices on the path from <em>r </em>to <em>v</em>, and “the <em>descendants </em>of vertex <em>v</em>” denotes any vertex <em>x </em>such that <em>v </em>is an <em>ancestor </em>of <em>x</em>. Every vertex is both <em>ancestor </em>and <em>descendant </em>of itself. “<em>Child </em>of vertex <em>v</em>” denotes any <em>descendant x </em>of <em>v </em>such that edge (<em>x,v</em>) ∈ <em>E</em>.

<ul>

 <li><strong>(3 points) </strong>Let <em>T </em>be a DFS tree of <em>G </em>with root <em>r </em>∈ <em>V </em>. That is, <em>T </em>= (<em>V,E<sub>T</sub></em>), where <em>E<sub>T </sub></em>is a subset of <em>E</em>, connecting all vertices in <em>G</em>. Given <em>T</em>, please briefly describe how to find <em>s</em>(<em>r,T</em>) in <em>O</em>(1) time complexity and <strong>prove the correctness</strong>.</li>

 <li><strong>(4 points) </strong>Let <em>v </em>be a vertex other than the root <em>r </em>(i.e. <em>v </em>6= <em>r</em>). Suppose that there is no edge {<em>u,w</em>} ∈ <em>E </em>where <em>u </em>is an <em>ancestor </em>of <em>v </em>in <em>T</em>, and <em>w </em>is a <em>descendant </em>of <em>v </em>in <em>T</em>. Please briefly describe how to find <em>s</em>(<em>v,G</em>) in <em>O</em>(1) time complexity and <strong>prove the correctness</strong>.</li>

 <li><strong>(5 points) </strong>Let <em>D<sub>T</sub></em>(<em>w</em>) denotes in tree <em>T</em>, the set of <em>descendants </em>of vertex <em>w </em>∈ <em>V </em>including <em>w </em> Also, for a set <em>S </em>⊆ <em>V </em>, let <em>N<sub>G</sub></em>(<em>S</em>) denotes in graph <em>G</em>(<em>V,E</em>), the set of “neighbors of vertices in set <em>S</em>”, i.e. <em>N<sub>G</sub></em>(<em>S</em>) = {<em>y </em>∈ <em>V </em>: ∃<em>x </em>∈ <em>S </em>s.t. {<em>x,y</em>} ∈ <em>E</em>}.</li>

</ul>

Define up<em><sub>T</sub></em>(<em>w</em>) := min<em><sub>y</sub></em>∈<em><sub>N</sub></em><em><sub>G</sub></em>(<em><sub>D</sub></em><em><sub>T</sub></em>(<em><sub>w</sub></em><sub>)) </sub>depth<em><sub>T</sub></em>(<em>y</em>). That is, up<em><sub>T</sub></em>(<em>w</em>) denotes in tree <em>T</em>, the minimum depth of “any neighbor in <em>G </em>of any <em>descendant </em>of <em>w </em>in <em>T</em>”.

Suppose <em>v </em>is an arbitrary vertex that is not the root in <em>T</em>, with <em>children w</em><sub>1</sub><em>,w</em><sub>2</sub><em>,</em>··· <em>,w<sub>k</sub></em>. Please show how to compute <em>s</em>(<em>v,G</em>) as a function of <em>k,</em>up<em><sub>T</sub></em>(<em>w</em><sub>1</sub>)<em>,</em>up<em><sub>T</sub></em>(<em>w</em><sub>2</sub>)<em>,</em>··· <em>,</em>up<em><sub>T</sub></em>(<em>w<sub>k</sub></em>), and depth(<em>v</em>). Please <strong>prove the correctness </strong>of your method as well.

<ul>

 <li><strong>(8 points) </strong>Given <em>G</em>, please design an algorithm that computes <em>s</em>(<em>v,G</em>) for <strong>all </strong>vertices <em>v </em>∈ <em>V </em>with time complexity <em>O</em>(|<em>V </em>| + |<em>E</em>|). Analyze its time complexity and <strong>prove the correctness</strong>.</li>

</ul>

<h1>Problem 6 – Lost in Pekoland (Hand-Written) (30 points)</h1>

<em>Note: In this problem, if you’re asked to provide an algorithm, you should prove both its correctness and its time complexity, and you </em><em>don’t have to write pseudocode as long as you can clearly explain your method. You can directly use any algorithm taught in class</em>

Pekoland, a place full of hopes and dreams, is an amusement park constructed by ”Usada Kensetsu,” a construction corporation founded by its CEO, Usada Pekora. The park comprises numerous celebrated landmarks, including a magnificent Castle, the grand Pekora Gundam, some formidable roller coasters, and a creepy monument of a mysterious figure, Yagoo. With these features, Pekoland has long been an appealing tourist attraction around the continent.

One day, Pekora wants to build some railways so that it can be more convenient to commute between the sites in her park. Suppose that the Pekoland’s layout <em>G </em>looks like a set of sites denoted as <em>V </em>connected by a set of roads denoted as <em>E</em>, each road connects exactly two different sites with both of its two endpoints and can be traveled from both directions, every two sites are connected by at most one road, and for any two different sites <em>a </em>and <em>b</em>, one is always able to go from <em>a </em>to <em>b </em>by walking through a series of roads in <em>E</em>.

<h2>Part I</h2>

Pekora decides to transform some of these roads into railways, but she notices that each road <em>e </em>has its own width <em>w</em>(<em>e</em>)<em>, </em>suppose a <em>path </em>is a series of roads (<em>v</em><sub>0</sub><em>,v</em><sub>1</sub>)(<em>v</em><sub>1</sub><em>,v</em><sub>2</sub>)<em>…</em>(<em>v<sub>n</sub></em><sub>−1</sub><em>,v<sub>n</sub></em>) where all (<em>v<sub>i</sub>,v<sub>i</sub></em><sub>+1</sub>) ∈ <em>E, </em>we define the width of a path as the <em>minimum </em>width of the roads it consists of. Pekora hopes that after the railway construction, for any pair of sites <em>s </em>and <em>t</em>, one can travel from <em>s </em>to <em>t </em>entirely

0 through railways by some of the widest path between them, that is, if <em>E </em>is the subset of roads being transformed, then at least one of the widest path between <em>s </em>and <em>t </em>on <em>G</em>(<em>V,E</em>) is still included in

0                                 0                                                                                                                                                                                                                                                                         0

<em>G </em>(<em>V,E </em>), but since they only have limited funds, she hopes |<em>E </em>| can be as small as possible. Please

0 help her find the set <em>E </em>that meets her needs.

<ul>

 <li><strong>(3 points) </strong>Give a <em>O</em>(<em>E </em>log<em>V </em>) algorithm that finds the <em>maximum </em>spanning tree of <em>G</em>.</li>

 <li><strong>(5 points) </strong>Prove that for any pair of sites <em>s </em>and <em>t</em>, the maximum spanning tree of <em>G </em>contains</li>

</ul>

0 some of their widest path. Conclude that Pekora can find the required set <em>E </em>in <em>O</em>(<em>E </em>log<em>V </em>) time complexity.

<h2>Part II</h2>

Months later, Usada Kensetsu became so much richer and transformed all roads into railways. Now every road <em>e </em>has its length <em>d</em>(<em>e</em>), which is a positive real number. To get to any site from her castle as quickly as possible, Pekora wants to find a shortest path from her castle <em>s </em>(which also belongs to <em>V </em>) to every other site. Luckily, some of her employees had learned some algorithms and had found the shortest path from <em>s </em>to all the other sites for her. However, she finds out that sometimes when a road gets reconstructed, its length can be lengthened or shortened, and it may influence the shortest distance of a site from <em>s</em>. She becomes curious that at a moment, which roads have the property that the change of its length would alter the shortest path distance from <em>s </em>to some sites <em>v </em>∈ <em>V </em>?

We define that a road <em>e </em>is <em>upwards critical </em>if increasing <em>d</em>(<em>e</em>) by any positive real number <em>ε </em>would increase the shortest path distance from <em>s </em>to at least one site <em>v </em>∈ <em>V, </em>and is <em>downwards critical </em>if decreasing <em>d</em>(<em>e</em>) by any positive real number <em>ε </em>would decrease the shortest path distance from <em>s </em>to at least one site <em>v </em>∈ <em>V.</em>

<ul>

 <li><strong>(5 points) </strong>Prove that a road (<em>u,v</em>) ∈ <em>E </em>is downwards critical if and only if there is a shortest path from <em>s </em>to <em>u </em>or <em>v </em>that ends at (<em>u,v</em>)<em>.</em></li>

 <li><strong>(5 points) </strong>Referring to the claim above, make a claim of the if and only if condition of being upwards critical and prove your claim.</li>

 <li><strong>(6 points) </strong>Using the above claims, give an <em>O</em>(<em>E </em>log<em>V </em>) time complexity algorithm that determines all upwards critical roads and all downwards critical roads respectively.</li>

</ul>

<h2>Part III</h2>

Since that Pekora is very naughty and likes to prank others, she has set up several traps in her amusement park. As a result, Pekoland is also considered to be a dangerous place to go by many. One day Pekora notices that every site <em>v </em>∈ <em>V </em>is graded by a <em>dangerous value k</em>(<em>v</em>) ≥ 0 by travelers. It comes to her that it may be fun to build a new roller coaster that sets off from some <em>v </em>∈ <em>V </em>, traveling through some roads of <em>E </em>then finally ends at the starting point <em>v</em>, and she would like the sum of all the dangerous value of the sites on the cycle to be high.

Thus she asks Moona Hoshinova, the chief technical officer of her company, to conduct the plan, but since building a roller coaster is tiring and costly, she replies that if the total length of the cycle is too large, she would not be willing to take over the task. After some negotiation, they define a cycle <em>v</em><sub>1</sub><em>,v</em><sub>2</sub><em>,…,v<sub>n</sub>,v<sub>n</sub></em><sub>+1 </sub>= <em>v</em><sub>1 </sub>on <em>G, </em>where all <em>v<sub>i </sub></em>∈ <em>V </em>and all (<em>v<sub>i</sub>v<sub>i</sub></em><sub>+1</sub>) ∈ <em>E</em>, as an <em>exciting cycle </em>if it satisfies that

where <em>K </em>is a constant given by Moona, and they meet the consensus that if there is an exciting cycle on <em>G</em>, then Moona would agree to build the roller coaster on this cycle, but if there is not such a cycle, then she would object to the plan.

<strong>(6) (6 points) </strong>Please provide an algorithm running in <em>O</em>(<em>V E</em>) time that finds if there exists an <em>exciting cycle</em>.

Hint: you can try re-weighting the graph.