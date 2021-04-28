# Data_science_Master
Work on cells
This work consists of scanning network and counting cells detected in different places. More precisely, it consists of counting new cells detected after each survey.
In the excel attached named ‘Cells_sny_final’, you can see that the experiment took place in 12 different places ( Riponne ,Chaudron, Lausanne-gare, Ouchy,…). These places are rallied in 4 areas: Riponne, Chaudron and Lausanne are considered as Ville. Ouchy, Préverenges and UNIL are considered as Lac. Forel, Essertes and Les Cullayes are considered as Campagne. Finally, Denges, Ecublens and Bussigny are considered as Périphérie.
So, for each place, 15 surveys were made and each surveys consist of a list of Cell IDs that represent cells. The goal is to count how many new cells you get after every survey. So, you have to compare Cell Ids from survey n with cells ID of all previous surveys to know how many new cells are detected. 
I considered that surveys are idd (independent and identically distributed). So, results from surveys have no influence on eachother and you have 15! different orders of surveys. The order could be {Survey 1, Survey 2, Survey 3,…, Survey 15} or {Survey 1, Survey 3, Survey 2…, Survey 15} or {Survey 2, Survey 1, Survey 3…, Survey 11}   so 15! possibilities.
I need you to plot all these possibilities in something like this:
 
So, the x axis is the number of surveys made (that is 15). The y axis is the number of the cells detected (varies depending on the area). So, in this graph, I plot 4 examples. We see that in the first example it detected 70 cells at survey 1, at survey 2 it detected 20 new cells compared to survey 1. At survey 3 it detects 17 new cells compared to survey 1 and 2 and so on. 
Another example: if survey 1 give {1010, 17890, 2345,879}, survey 2 gives {1010,879, 4567} and survey 3 gives {1010,17890, 879,2345}. So, survey one has 4 cell ID. From survey 1 to survey 2 we have one new cell (4567) and 0 new cells from survey 2 to survey 3. So, in the graph we plot [0;4], [1,1] and [2;0] for this order.
So, in total, I need four graphs. One for each area (Ville, Lac, Campagne and Périphérie) which contains the 3 different places. For example, for the ‘Ville’ graph, I need you to plot surveys from Riponne then plot surveys from Chaudron and then surveys of Lausanne-Gare. After this, I need the mean of cells detected at each survey (in red in the example above) and the variation at each surveys ( in black in the example above) for the area Ville.
These 4 graphs will have millions of data so it will be different from the example above. And be free to modify the colours and the markers if it is clearer.




















