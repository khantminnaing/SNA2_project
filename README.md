# Social Network Analysis Project

## Introduction 
This project investigates about the state of political bi-partisanship in light of the 2006 United States elections and analyse the purchasing patterns of people to political books the other side of the spectrum. Understanding which nodes are the most central to the network could also give an indication of how ideas and opinions are bridged


## Dataset 
This project use the dataset of a network of books about US politics published around the time of the 2004 presidential election and sold by the online bookseller Amazon.com. Edges between books represent frequent copurchasing of books by the same buyers. The network was compiled by V. Krebs and is unpublished, but can found on Krebs' web site (http://www.orgnet.com/).

<img width="1500" alt="Network of Political Books" src="https://user-images.githubusercontent.com/87215545/234359208-8eff5668-bcc5-43bd-9412-ba28a8c37575.png">


<ul>
  <li>Each node represents a book, categorized according to political orientation : Conservative (c), Liberal (l) or Neutral (n)</li>
  <li>Each edge represents frequent co-purchasing of books by the same buyers</li>
</ul>
<b>Key statistics</b>
<ul>
  <li>Number of nodes = 105</li>
  <li>Number of edges = 441</li>
  <li>Diameter = 7</li>
  <li>Clustering coefficient = 0.35</li>
  <li>Average degree = 8.4</li>
</ul>





## Methodology
<b>Degree Centrality</b> : measures the number of connections (or edges) each node (or book) has. Books with high degree centrality would be those that were frequently co-purchased with many other books.
<br>
<br>
<b>Betweenness Centrality</b> : measures the extent to which a node lies on the shortest paths between other nodes in the network. 
Books with high betweenness centrality would be frequently co-purchased with other books that were not necessarily directly connected to each other.
<br>
<b>Community Detection</b> : involves identifying groups of nodes that are more tightly connected to each other than to the rest of the network. Communities could represent clusters of books frequently co-purchased together, perhaps corresponding to different political ideologies or topics. 



## Results
![graph (3)](https://user-images.githubusercontent.com/87215545/233957903-eee5180d-dce2-4310-a401-a907b83df057.png)

### Libraries Used
<img width="771" alt="Screenshot 2023-04-24 at 12 09 18 AM" src="https://user-images.githubusercontent.com/87215545/233868771-83b6ebef-4933-4667-81bd-c4e923497fb5.png">

## Appendix
This project is for SNA2 : Social Network Analysis in Digital Age at AY22-23 Sciences Po Paris.
<p>
<img width="200" alt="Logo_SP" src="https://user-images.githubusercontent.com/87215545/233868820-2139d220-2f73-4213-a371-bc19b97c1f88.png">
