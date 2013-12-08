File Descriptions
--------
main.py is our python code base that can call Quakers' R code on [error diagrams](https://github.com/SunnySunnia/TheQuakers/blob/master/MDA/mda_test.r)
of testing u from 4.7 to 6 based off [Luen’s code](https://github.com/SunnySunnia/TheQuakers/blob/master/MDA/etas-training.R).

**Step by Step instructions**

*For Mac*

If `x11()` `plot(1,1)` runs in your R studio, then `install.packages("sfsmisc")`, `library("sfsmisc")`
- Download & Install package ["Xquartz"](http://xquartz.macosforge.org/landing/)
- In your terminal `git clone https://github.com/wliang88/STAT-157-Checking-Group-`
- `cd STAT-157-Checking-Group-`
- `export DISPLAY=:0`
- `python main.py`

If `x11()` `plot(1,1)` doesn't runs in your R studio
- Download & Install package ["Xquartz"](http://xquartz.macosforge.org/landing/)
- Open the "Terminal" under "Application" in "Xquartz"
- open up R
- `install.packages("sfsmisc")`
- `library("sfsmisc")`
- exit R
- `git clone https://github.com/wliang88/STAT-157-Checking-Group-`
- `cd STAT-157-Checking-Group-`
- `python main.py`
 
