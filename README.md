Landmark with Regressition in Python
====
Now It only supportes LBF(Local Binary Features) regression(Based on the [matlab version](https://github.com/jwyang/face-alignment)) with [AFLW](http://lrs.icg.tugraz.at/research/aflw/) dataset format.      

#### __Dependencies__    
---    
* python2.7    
* numpy    
* scipy    
* scikit-learn    

#### __Usage__    
---    

* __Train__    
`
./demo_train.py ../config/config.py
`

* __Test__    
`coming soon`

* __Evaluate__   
`coming soon`    

#### __Extend__
---    
* __Training with your own dataset__    
You should implement your own reader. Please refer to `AFLWReader` in `./cascade/dator/data.py`.

* __Implement other regression algorithm__ 
Please refer to `cascade/regressor/lbfRegressor.py`. And then wrapped in `cascade/regressor/regressorWrapper.py`


#### __TODO__    
---     
* [__TODO__] Support Face Detector to detect the face instead of getting face rect via landmarks
* [__TODO__] Support `Explicit Shape Regression`    
* [__TODO__] Try random ferns instead of random forest   
* [__TODO__] Try finding the best split when training Random Forest. Now using random split    
* [__TODO__] Try different interpolations when computing `Pixel Difference Feature`      



#### __References__    
---    
1. Face Alignment at 3000 FPS via Regressing Local Binary Features    
2. Face Alignment by Explicit Shape Regression

#### __Contact__    
If you have any questions, please email shenfei1208@gmail.com or creating an issue on GitHub.