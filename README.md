# Recruit Restaurant Visitor Forecasting
This is a [Kaggle competition](https://www.kaggle.com/c/recruit-restaurant-visitor-forecasting) in 2017

## Research Notes
* [Feature Engineering](https://hackmd.io/s/HJVz17xA7)
* [Methods and tools](https://hackmd.io/s/rJgju2JAm)
* [Final report](https://docs.google.com/document/d/1qRJV1Lii3t32h6BkBzvNmv9epSz00DbO4UlZljKEK8s/edit)

## Usage

Download and unzip the [dataset](https://www.kaggle.com/c/recruit-restaurant-visitor-forecasting/data)
Change the folder's name from "all" to "data"
In "code" folder, running [holiday+weekend.py, pre_store_info.py, reserve_feat.py, testdata_merge.py, time_visit_data.py, weather.py] separately will generate feature files in "features" folder.
Then run testdata_merge.py & merge.py. They will generate train data and test data.
Last, run arima.py or lgbm.py. The prediction will be stored in the submissions folder.

## Result(RMSLE)
ARIMA: Private 0.612, Public 0.580 LGBM: Private0.540, Public 0.502
