# Audio-signal-separation
Analyzing monoaural mixed signal and separating it into its sources. Classifying and predicting the source of the sound signal. 
------------------------------------------------------------------------------------------------------------------------------
Update in source code from soundnet (MIT):
The original code was showing UnicodeDecodeError in Python, to solve this I had included the following line in the code
in function build_model()
 model_weights = np.load('models/sound8.npy', mmap_mode=None, allow_pickle=True, fix_imports=True,
         encoding='latin1').item()
         
-------------------------------------------------------------------------------------------------------------------------------
Note the following installations are required in Python, Open command Window in Python (I used Spyder IDE)
Keras: pip install keras
pysoundfile (pip install pysoundfile)
numpy (conda install numpy)
scikit-learn (conda install scikit-learn)
for .mp3 files: conda install -c conda-forge ffmpeg
librosa: pip install librosa
--------------------------------------------------------------------------------------------------------------------------------
