# Audio-signal-separation
Analyzing monoaural mixed signal and separating it into its sources. Classifying and predicting the source of the sound signal. 
------------------------------------------------------------------------------------------------------------------------------
Update in source code from soundnet (MIT):
The original code was showing UnicodeDecodeError in Python, to solve this I had included the following line in the code
in function build_model()
 model_weights = np.load('models/sound8.npy', mmap_mode=None, allow_pickle=True, fix_imports=True,
         encoding='latin1').item()
         

Note the following installations are required in Python, Open command Window in Python (I used Spyder IDE)

1.Keras: pip install keras

2.pysoundfile (pip install pysoundfile)

3.numpy (conda install numpy)

4.scikit-learn (conda install scikit-learn)

5.for .mp3 files: conda install -c conda-forge ffmpeg

6.librosa: pip install librosa

