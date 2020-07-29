# CARSKit

### Introduction
-------------------

**CARSKit** (original version: https://github.com/irecsys/CARSKit/) is an open-source Java-based context-aware recommendation engine, where it can be used, modified and distributed under the terms of the GNU General Public License. (Java version 1.7 or higher required). It is specifically designed for context-aware recommendations. 


### GPL License
-------------------

CARSKit is [free software](http://www.gnu.org/philosophy/free-sw.html): you can redistribute it and/or modify it under the terms of the [GNU General Public License (GPL)](http://www.gnu.org/licenses/gpl.html) as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. CARSKit is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details. You should have received a copy of the GNU General Public License along with CARSKit. If not, see http://www.gnu.org/licenses/.

### Modifications
----------------------------

The following modifications have been made to the original version:

* Added a Random recommendation algorithm, where items are assigned a random integer between 1 and 1000 and are ranked based on this number.
* Added a ItemPopularity recommendation algorithm, where items are ranked based on the amount of ratings/interactions that they have had.
* Modified that the first line of any output recommendation list contains an integer, which represents the amount of recommended items for each user-song(-context) combination.
* Modified that the header of the recommendation lists contains unique column names for each recommended item, e.g. 'p1' for the recommended item on position 1, 'p2' for the second etc.
* Modified that the system also outputs the fold that has been left out in each iteration over all the folds. Our re-rank system needs to know for each iteration which ratings/listening events are used for evaluation of performance.
* Modified that next to the specific fold, the system also outputs another file containing the index of all positive items across all recommendation lists. This data is used to visualize the distribution of positive items for the initial recommender algorithm to get a general idea about the recommendation accuracy.








