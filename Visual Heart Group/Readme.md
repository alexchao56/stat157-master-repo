# Earthquake Project: Visual Heart Group

## Group Main Repository
https://github.com/annyeongjs/visualheart.task8

## Members

<table border="0">
<tr>
<th>Name</th>
<th>Role</th>
<th>GitHub Id</th>
</tr>
<tr>
<td>Hong Shon</td>
<td>Presenter</td>
<td>@tzenarr</td>
</tr>
<tr>
<td>Christina Ho</td>
<td>Visualizer/ Operational Lead</td>
<td>@chocoho</td>
</tr>
<tr>
<td>Jinsoo Lee (Jason)</td>
<td>Visualizer</td>
<td>@annyoengjs</td>
</tr>
<tr>
<td>Hyungkyu Chang</td>
<td>Visualizer</td>
<td>@hkchang89</td>
</tr>
<tr>
<td>Sung Hoon Choi</td>
<td>Visualizer</td>
<td>@shchoi</td>
</tr>
<tr>
<td>Alisha Agrawal</td>
<td>Data Curator</td>
<td>@alisha791</td>
<tr>
<td>Jie Zhang</td>
<td>Data Curator</td>
<td>@jzhang980</td>
<tr>
<td>Qi Zhang</td>
<td>Analyzer</td>
<td>@qi-zhang</td>
<tr>
<td>Kuanwei Tseng</td>
<td>Data Curator</td>
<td>@kt0009</td>
</table>


## Improvements
#####Improvement to the [ecdf.R](https://github.com/SunnySunnia/TheQuakers/blob/master/ECDF/ecdf.R)
- Added x axis label in terms of date. This essentially addresses all 3 items mentioned above.
- Added horizontal grids to make it easier to read.
- Some important settings were hard coded in the original code, e.g. boundary of magnitude interval, location of vertical grid etc. So it worked fine with 250.csv but not the new records which contain 6598 events from 1932 to 2013. The new code can handle these settings adaptively and work with data of any size.
- Wraped up the code as a function, the only argument required is the data frame loaded from data file.
- The improved version was renamed to [ecdf_improved.R](https://github.com/qi-zhang/visualheart.task8/blob/master/ECDF_IMPROVED/ecdf_improved.R)

#####Improvement to the [etas-training.R](https://github.com/SunnySunnia/TheQuakers/blob/master/MDA/etas-training.R)
- Cleaned up unnecessary code. Replace the original "placeholder"+"for loop" with sapply functions.
- Re-wrote the internal loop of error estimate in the Mag-dependent automatic model and etas.CI to improve run time performance. The latest code runs about 3 times faster.
- Re-organized the code and add comments to make it more readable.
- Added grids to the plot to make it more readable. 
- The improved version was renamed to [etas_training_improved.R](https://github.com/qi-zhang/visualheart.task8/blob/master/ETAS_TRAINING_IMPROVED/etas_training_improved.R)

#####Improvement to the [Quakers-EarthquakeSuccessors.R](https://github.com/SunnySunnia/TheQuakers/blob/master/Successors/Quakers-EarthquakeSuccessors.R)
- Added title for each plot to help people understanding the brief idea of each graph.
- Adjusted legend and y-label for each plot to help people understanding details of each graph.
- Re-wrote the internal loop to make sure the index never exceed the length of the vector.
- Added tons of comments to make the code easy to read.
- The improved version was renamed to [Quakers-EarthquakeSuccessors_improved.R] (https://github.com/qi-zhang/visualheart.task8/blob/master/SUCCESSORS_IMPROVED/Quakers-EarthquakeSuccessors_improved.R)
