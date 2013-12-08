As of 2013-12-08

- [**Group 1 & 3**](http://github.com/aparker92/error_analyzers) 
 - Refactor [Luen's code](https://github.com/aparker92/error_analyzers/blob/master/etas-training.R) to generate an error diagram and a quantity for the area under the curve ([ErrorDiagram.R](https://github.com/aparker92/error_analyzers/blob/master/ErrorDiagram.R)) 

 - [Steps for Reproducibility](https://github.com/aparker92/error_analyzers/blob/master/Reproducibility.md) 


- [**Group 2**](https://github.com/stat157/analyzers) *we are trying to see if we can get their product into Amazon Web Services (AWS). That way people can access the codebase from anywhere*
  - Created [aftershock_arrival_plots.py](https://github.com/stat157/analyzers/blob/master/notebooks/aftershock_arrival_plots.py): plot aftershock arrival times, binned by magnitude in the x-axis, time in the Y-axis. 
  - Created [mda_with_curator_data.py](https://github.com/stat157/analyzers/blob/master/notebooks/mda_with_curator_data.py): Iterate upon aftershock-arrival plotting code to take the curators' sample data as input. Try different bin sizes (e.g. binning in magnitude ranges of 0.1, 0.2, 0.5, etc.), try if they can expand on the 2013 catalog to include more years.
  - [Vagrant box package] (https://github.com/stat157/analyzers/issues/9)
  - step-by-step instructions for [installing dependencies](https://github.com/stat157/analyzers/blob/master/notes/vagrant_setup.md)

- [**Group Q**](https://github.com/SunnySunnia/TheQuakers):   *We have our python code base that can call Quakers' R code on error diagrams, will continue trying to call all their main model codes* 
 - Built 2 models: [Empirical CDF](https://github.com/SunnySunnia/TheQuakers/tree/master/ECDF) & [Modified MDA](https://github.com/SunnySunnia/TheQuakers/tree/master/Quantile-Method)
 - Helper functions: [Functions that compute error rates](https://github.com/SunnySunnia/TheQuakers/tree/master/skeleton/SupportFunctions)
 - [Main Takeaways](https://github.com/SunnySunnia/TheQuakers/#final-results)
 
- [**Group #**](https://github.com/ashleysia/TeamHASHTAG):
 - [Time Series graphs in R](https://github.com/ashleysia/TeamHASHTAG/blob/master/R-Code.md%20)
 - [Geographical map of earthquakes](https://github.com/ashleysia/TeamHASHTAG/blob/master/Plot%20Raw.ipynb)


- [**Group C**](https://github.com/davidwang001/Group-C-Repo)
 - All code is written using Adobe Illustrator, there isn’t really much that can be reproduced because it is hard code essentially, the files are no dependent on anything besides having access to Adobe Illustrator.
 - Basic presentation of the overall classes attempt to solve this problem, basic slidedeck.

-----

*As of 2013-11-23*

- [**Group 1 & 3**](http://github.com/aparker92/error_analyzers) *We can't check in yet but their deadline is 11/25*
  - Refactor [Luen's code](https://github.com/aparker92/error_analyzers/blob/master/etas-training.R) to generate an error diagram given a dataset and a model; code includes includig both etas testing and MDA testing codes Luen used for his paper.
  - Their [group task](https://github.com/aparker92/error_analyzers/blob/master/taskfornov21.txt), deadline is 11/25. 

- [**Group 2**](https://github.com/stat157/analyzers) *We can run `aftershock_arrival_plots.ipynb` & `mda_with_curator_data.ipynb` but need to install scipy*
  - Created [aftershock_arrival_plots.py](https://github.com/stat157/analyzers/blob/master/notebooks/aftershock_arrival_plots.py): plot aftershock arrival times, binned by magnitude in the x-axis, time in the Y-axis. 
  - Created [mda_with_curator_data.py](https://github.com/stat157/analyzers/blob/master/notebooks/mda_with_curator_data.py): Iterate upon aftershock-arrival plotting code to take the curators' sample data as input. Try different bin sizes (e.g. binning in magnitude ranges of 0.1, 0.2, 0.5, etc.), try if they can expand on the 2013 catalog to include more years.

- [**Group Q**](https://github.com/SunnySunnia/TheQuakers):   *We have our python code base that can call Quakers' R code on error diagrams, will check whether the python code base can also be called on the [plotting successors.R file](http://github.com/SunnySunnia/TheQuakers/tree/master/Successors).* 

  - Finished their R code on [error diagrams](https://github.com/SunnySunnia/TheQuakers/blob/master/MDA/mda_test.r) of testing u from 4.7 to 6 based off [Luen’s code](https://github.com/SunnySunnia/TheQuakers/blob/master/MDA/etas-training.R). 
  - Trying to figure out an algorithm to compare the models, but were not able to vary tao on the x-axis of the error diagram for one specific window function. Waitting for Luen's explanation on his code about how he inplement K as in Ku^M in his code, namely, how did he vary different tao for the error diagram.
  - Currently working on the [optimization approach](https://github.com/SunnySunnia/TheQuakers/tree/master/Successors): simply gather all the times of first successors of earthquakes that are larger that magnitude 3 within an increment of 0.1, then find thier 90 percentile cut points as our window length for earthquakes within that magnitude range. 
  
- [**Group ❤**](https://github.com/annyeongjs/visualheart.task8): *We can't check in yet*
  - Currently [proofreading](https://github.com/annyeongjs/visualheart.task8/blob/master/LuenSummary.md) on Luen, Stark: [Testing Earthquake Predictions](http://projecteuclid.org/DPubS?verb=Display&version=1.0&service=UI&handle=euclid.imsc/1207580090&page=record)
  - Planning to [improve graphs](https://github.com/annyeongjs/visualheart.task8/blob/master/ImprovingGraphs.md)
  
- [**Group #**](https://github.com/ashleysia/TeamHASHTAG): *We can't check in yet*
  - Looking at various D3 visualizations and figuring out what type of interactive plot/graph/visual
  - Visualizing data geographicly in [python](https://github.com/ashleysia/TeamHASHTAG/blob/master/Plot%20Raw.py): Not sure how this work is going to help us, but communicating with them [here](https://github.com/ashleysia/TeamHASHTAG/issues/7).

- [**Group $**](https://github.com/joyyqchen/EarthquakeProject.Team-Chen.Hsiao.Kirschner.Liou.Tsai): *We can't check in yet*
  - Using D3 for Visuals: Research and learn how to employ D3 to create a dynamic visualization for the data

- [**Group C**](https://github.com/davidwang001/Group-C-Repo): *We can't check in yet*

  - Compliling notes on Luen's dissertation and Chris' HTML presentation.
  - Come up with a comprehensive list of new goals for the class to pursue
