![Untitled design (32)](https://user-images.githubusercontent.com/87215545/234714585-bb1f1baf-b242-4ad0-b4fa-4667aae5fc1f.png)

# Social Network Analysis Project

## Introduction 

Given the extent of political polarisation in the US, it is important to understand how receptive people are to ideas from the other side of the political spectrum. This implies an important research area about the state of political bi-partisanship in the US. 

This project investigates about the state of political bi-partisanship in light of the 2004 United States elections and analyse the purchasing patterns of people to political books the other side of the spectrum. We argue that the co-purchasing patterns might be indicative of whether people seek out opposing opinions or prefer to have their own views reinforced. Moreover, understanding how ideas and opinions are bridged across the political spectrum is of great interest. By employing a social-network-based research, we hope to provide an insight into the level of partisanship and open-mindedness in the US, at least in 2004.

## Dataset 
This project use the dataset of a network of books about US politics published around the time of the 2004 presidential election and sold by the online bookseller Amazon.com. Edges between books represent frequent copurchasing of books by the same buyers. The network was compiled by V. Krebs and is unpublished, but can found on Krebs' web site (http://www.orgnet.com/).

<ul>
  <li>Each node represents a book, categorized according to political orientation : Conservative (c), Liberal (l) or Neutral (n). The assignment of these political orientations was done by Mark Newman on the basis of his reading of the descriptions and associated comments on each book’s Amazon page.</li>
  <li>Each edge represents frequent co-purchasing of books by the same buyers. In essence, these are the books that are suggested by Amazon with the feature that says: “customers who bought this book also bought...".</li>
  <li> With respect to the size of the dataset, there are 105 nodes, with 441 edges between them, yielding an average degree of 8.4 per node, which means that it is of sufficient size to be analysed. The diameter, which is the number of nodes on the longest of the shortest paths between any two nodes, is 7, which gives an indication of the inter-connectedness of the data. The clustering coefficient of 0.35 suggests that there is sufficient clustering for our analysis to be able to discern distinct communities of co-purchased books, to enable useful insights to be drawn.</li>
</ul>
<br>
<img width="1500" alt="Network of Political Books" src="https://user-images.githubusercontent.com/87215545/234359208-8eff5668-bcc5-43bd-9412-ba28a8c37575.png">
<b>Summary of Key statistics</b>
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
<br>
<b>Community Detection</b> : involves identifying groups of nodes that are more tightly connected to each other than to the rest of the network. Communities could represent clusters of books frequently co-purchased together, perhaps corresponding to different political ideologies or topics. 
<ul>
  <li> <b>Modularity Maximisation (Newman Algorithm) </b> : Find a partition of the network by iteratively removing the edges of the graph, based on the edge betweenness centrality value, until maximum modularity is achieved.</li>
  <li><b>Louvain Algorithm (Hierarchical) </b> : A hierarchical clustering algorithm that optimizes modularity in a bottom-up manner. Iteratively merges nodes into communities</li>
</ul>




## Results

The graph below is a reorganization of the the nodes and edges depending on the categorization of each book. At a first glance, there appears to be little connections between conservative books, marked by the red circles, and liberal books, marked by the green circle. 

![graph (3)](https://user-images.githubusercontent.com/87215545/233957903-eee5180d-dce2-4310-a401-a907b83df057.png)



## Limitations

In terms of limitations, there were three limitations we ran into with our social network and data. Firstly, the number of books (which is also the number of nodes), 105, may not be enough to have a comprehensive conclusion of what the results represent/mean in a larger sense and cannot generalize our findings onto the greater U.S. population. Secondly, political orientation, the idea behind this was that the type of book an individual bought may not be representative of their political orientation/beliefs. To explain, there are a multitude of reasons why an individual would purchase a liberal book, for example, (school required readings, work, research, etc.) and they may not be liberal at all. This is why the research results may not be accurate enough to describe each buyer as liberal, conservative or neutral. Finally, population, because the data was collected on political books that were purchased on Amazon’s website, that means that the population of purchasers had to be Amazon members. Because of this reason, we cannot assume that Amazon users are representative of the whole population, therefore we cannot generalize and/or reflect these results onto a larger population since not all Americans are Amazon members. 

## Conclusion

To conclude, the type of book Amazon users purchased may represent their political orientation/preferences, but the results of this study cannot be generalized onto the greater U.S. population as 105 books sold is too small of a number to be representative. As per the results, most users weren’t too keen on purchasing books that differ from their political beliefs (as the # of neutral books sold were few compared to the latter). For those that purchased both types of books (edge), these customers seem to have been already politically neutral and the only common books between customers with different political beliefs were neutral books. To conclude, the analysis present is mostly quantitative based, but with more research we can further analyze more qualitatively (by looking at communities, reason for book purchases, etc.) to identify the bridge nature more clearly.

### Libraries Used
<img width="771" alt="Screenshot 2023-04-24 at 12 09 18 AM" src="https://user-images.githubusercontent.com/87215545/233868771-83b6ebef-4933-4667-81bd-c4e923497fb5.png">

## Appendix
This project is for SNA2 : Social Network Analysis in Digital Age at AY22-23 Sciences Po Paris.
<p>
<img width="200" alt="Logo_SP" src="https://user-images.githubusercontent.com/87215545/233868820-2139d220-2f73-4213-a371-bc19b97c1f88.png">
