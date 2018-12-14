	Features and labels are in npy file formats
	As file and datasets size are too large so we can not push all files on the github repo


# ASR_2018_T01
## Data pre processing
Run ```python import_timit.py --timit=./TIMIT --preprocessed=False```
to compute the features and store them in a folder.
This script also converts the [NIST "SPHERE" file format](https://www.isip.piconepress.com/projects/speech/software/tutorials/production/fundamentals/v1.0/section_02/s02_01_p04.html) to [WAVE PCM format](http://soundfile.sapp.org/doc/WaveFormat/).
If you have already converted the files, set ```--preprocessed=True``` to skip the conversion process.

## References:
- Mel Frequency Cepstral Coefficient (MFCC) tutorial :
    - [http://practicalcryptography.com/miscellaneous/machine-learning/guide-mel-frequency-cepstral-coefficients-mfccs/](http://practicalcryptography.com/miscellaneous/machine-learning/guide-mel-frequency-cepstral-coefficients-mfccs/)
- TIMIT related documents: 
    - [https://nvlpubs.nist.gov/nistpubs/Legacy/IR/nistir4930.pdf](https://nvlpubs.nist.gov/nistpubs/Legacy/IR/nistir4930.pdf) 
    - [https://github.com/philipperemy/timit](https://github.com/philipperemy/timit)
- Implementation references:
    - [http://scikit-learn.org/stable/index.html](http://scikit-learn.org/stable/index.html)
    - [http://scikit-learn.org/stable/modules/generated/sklearn.mixture.GaussianMixture.html](http://scikit-learn.org/stable/modules/generated/sklearn.mixture.GaussianMixture.html)
    - [http://www.pitt.edu/~naraehan/python2/pickling.html](http://www.pitt.edu/~naraehan/python2/pickling.html)
    - [https://github.com/belambert/asr-evaluation](https://github.com/belambert/asr-evaluation)
## This repo contains
- [x] Code to read files and compute MFCC features
- [x] Computing MFCC for time slices given in .PHN files
- [x] Dumping computed features to a folder
- [ ] Dumping phone-wise features to a folder
- [ ] GMM training
- [ ] GMM model dumping
- [ ] GMM evaluation
- [ ] PER computation

## Expected:
    - Implement and run train.py and test.py
    - Please feel free to modify any part of the code to implement the solution
	
	
	Features and labels are in npy file formats
	As file and datasets size are too large so we can not push all files on the github repo
