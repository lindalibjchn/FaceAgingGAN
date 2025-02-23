#### General data analysis

The experiment on the Google Colab, the aim is general checking the age and gender distribution in three datasets, UTKFace, IMDB_WIKI and CACD2000, <b>Analysis_DATASET(IMDBWIKI+UTKFace+CACD2000).ipynb</b>

#### Face alignments for data processing 

1. Precondition: 

   (1) Install dependencies under the anaconda virtual environment (experiment environment)
   
    <b> Suggestion</b>: it is better to create a new virtual environment for data processing
```
      conda install -c menpo dlib 
      conda install -c conda-forge opencv
      pip install imutils
      pip install dlib
```

   (2) General install method
```
    pip install imutils
    pip install dlib
    pip install opencv-python
```
    

2. Run programme with custom setting
```
   python aligment_faceimages.py \
       --root_dir "../DATA/" \  # directory to source data
       --des_dir "training_align" \ # directory to destination for aligned data
       --notdetect_dir "notdetect" # directory to dir
```
3. Results
<p align="center">
  <img src="images/alignedface.png" height="200",width="800">
</p>

#### Reference
1. https://github.com/contail/Face-Alignment-with-OpenCV-and-Python.git
2. https://www.pyimagesearch.com/2017/05/22/face-alignment-with-opencv-and-python/
