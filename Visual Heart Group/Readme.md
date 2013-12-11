# Earthquake Project: Visual Heart Group

## Group Main Repo
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
#####[ecdf.R](https://github.com/SunnySunnia/TheQuakers/blob/master/ECDF/ecdf.R)
- Added x axis label in terms of date. This essentially addresses all 3 items mentioned above.
- Added horizontal grids to make it easier to read.
- Some important settings are hard coded in the original code, e.g. boundary of magnitude interval, location of vertical grid etc. So it works fine with 250.csv but not the new records which contain 6598 events from 1932 to 2013. The new code will setup these settings adaptively to make it work with data of any size.
- Wrap up the code as a function, the only argument required is the data frame loaded from data file. I verified the code with both the 250.csv and the new records of events from 1932 to 2013.

#####[etas-training.R](https://github.com/SunnySunnia/TheQuakers/blob/master/MDA/etas-training.R)
- Clean up unnecessary code. Replace the original "placeholder"+"for loop" with sapply functions.
- Rewrite the internal loop of error estimate in the Mag-dependent automatic model and etas.CI to improve run time performance. The latest code runs about 3 times faster.
- Re-organize the code and add comments to make it more readable.
- Add grids to the plot to make it more readable. 

#####[Quakers-EarthquakeSuccessors.R](https://github.com/SunnySunnia/TheQuakers/blob/master/Successors/Quakers-EarthquakeSuccessors.R)
- Added title for each plot to help people understanding the brief idea of each graph.
- Adjusted legend and y-label for each plot to help people understanding details of each graph.
- Rewrote the internal loop to make sure the index never exceed the length of the vector.
- Add tons of comments to make the code easy to read.
