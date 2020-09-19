# position_tracking
An assortment of jupyter notebooks to track rodent position using deeplabcut.  

## Created to use deeplabcut to track animal position.   

Pipeline: 

1. Establish a new project by running ```initialize_project.ipynb```

* Run on local machine within DLC environment. You can find detailed instructions for setting up DLC [here](https://github.com/DeepLabCut/DeepLabCut).
* After running the notebook, you must save a copy of the project folder and video folder (videos to analyze) to your google drive and update paths in the ```config.yaml``` file. 

2. Open ```Colab_TrainNetwork_VideoAnalysis.ipynb``` in colab to make use of their GPUs.

* Training network and analyzing videos may take some time. Colab GPUs disconnect after extended use. Current version saves every 500 iterations. Training can resume at last saved iteration if GPU disconnects. 

3. Use ```Check_DLC.ipynb``` to verify tracking accuracy for each video. If tracking accuracy is poor, additional images can be labeled and network can be retrained to improve accuracy. 

Notebooks are not general. Paths or DLC parameters should be adjusted as needed. 
