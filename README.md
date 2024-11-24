I've used A* Search with Linear Conflict(extension of Manhattan Distance), A* Search with Manhattan Distance, A* Search with Hamming Distance, Breadth-First Search, and Depth-First Search with Bound for the puzzle problem. You can find my results below corresponding to different methods. A* Search with Linear Conflict(Improved Manhattan Distance) gives the most efficient results. When the PUZZLE_DIM is high, Breadth-First Search and Depth-First Search with Bound are not efficient. Note that Quality and the Cost depend on Initial State.

|Strategy|RANDOMIZE_STEPS|PUZZLE_DIM fitness|Quality(# of actions in the solution)|Cost(Total number of actions evaluated)|
|-------|-----------|---------------|------------|---------|
|A* Search with Linear Conflict(Informed Strategy)|100_000|4|46|180595|
|A* Search with Manhattan Distance(Informed Strategy)|100_000|4|46|1414443| 
|A* Search with Hamming Distance(Informed Strategy)|100_000|4|46|>>1414443 - Not efficient(2 hour passed then I stopped the execution)|
|Breadth-First Search(Uninformed Strategy)|100_000|4|46|>>1414443 - Not efficient(2 hour passed then I stopped the execution)|
|Depth-First Search with Bound(Uninformed Strategy)|100_000|4|46|>>1414443 - Not efficient(2 hour passed then I stopped the execution)|
|A* Search with Linear Conflict(Informed Strategy)|100_000|3|24|572|
|A* Search with Manhattan Distance(Informed Strategy)|100_000|3|24|1087| 
|A* Search with Hamming Distance(Informed Strategy)|100_000|3|24|28595|
|Breadth-First Search(Uninformed Strategy)|100_000|3|24|130601|
|Depth-First Search with Bound(Uninformed Strategy)|100_000|3|24|28595 - When I decreased bound from 60 to 24, I obtained a very time efficient result|
|A* Search with Linear Conflict(Informed Strategy)|100_000|2|2|3|
|A* Search with Manhattan Distance(Informed Strategy)|100_000|2|2|3| 
|A* Search with Hamming Distance(Informed Strategy)|100_000|2|2|3|
|Breadth-First Search(Uninformed Strategy)|100_000|2|2|5|
|Depth-First Search with Bound(Uninformed Strategy)|100_000|2|2|5|

![alt text](image-1.png)
![alt text](image.png)
![alt text](image-2.png)