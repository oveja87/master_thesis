# DRUM SOUND ANALYSIS
## Recognition and Differentiation of Drum Sounds as Extension to the E-Learning Platform Easydrum
### Master’s thesis submitted in fulfillment of the requirements for the degree Master of Science

This thesis describes the concept for an extension of the online drum school Easydrum.
The aim of this thesis is to provide a system that allows to use an analog drum set with
the Easydrum platform. This system is able to receive the sound of the drum set on
a web browser by using a microphone. It detects strokes on drums and cymbals of a
pre-configured drum kit in real-time and differentiates them from each other. Therefore,
an onset detection algorithm based on the time domain of the incoming audio stream
is developed and two different approaches for classification are tested. The algorithms
are tested with MatlabR and Weka.

The first classification approach is based on the extraction of a feature vector that is
used to build a decision tree with the J48 algorithm.

In the second approach templates of the minimum and maximum frequency spectrum
of each trained stroke type are created. By analyzing correlations in the spectral
shapes between these templates and an unseen data instance, a class label for the
unseen instance can be determined. The method is tested with single strokes as well
as with two simultaneously played strokes.

Furthermore, this thesis gives an introduction to the Web Midi API, which is required
to develop the further application. An example for receiving an audio stream on the
browser and displaying it on a HTML canvas element is given.

### Keywords
audio signal processing, signal processing, classification, decision tree,
J48, onset detection, Web Audio API, MatLab, percussive sound, real-time



### Contents
1 Introduction
2 Basic Concepts
2.1 Easydrum
2.1.1 Technologies 
2.1.2 Architecture 
2.2 Components of a Drum Set 
2.3 Notation 
2.4 Audio Signal Processing 
2.4.1 Audio Signals 
2.4.2 Sampling and Quantization 
2.5 Frequency Spectrum Analysis of Digital Signals 
2.5.1 Discrete Fourier Transformation 
2.5.2 Short Time Spectral Analysis and Windowing 
2.5.3 Fast Fourier Transformation 
2.6 Onset Detection 
2.7 Classification 
2.7.1 Feature Extraction
2.7.2 Feature Based Classification
2.7.3 Decision Trees
2.7.4 Further Classification Methods 
2.7.5 Evaluation
2.8 Tools
2.8.1 MatLabR
2.8.2 Weka 
2.9 Audio Processing in the Web 
3 Related Work 
3.1 Onset Detection 
3.2 Classification 
3.3 Real-Time Approach 
4 Methods 
4.1 Test Drum Set and Hardware 
4.2 Onset Detection 
4.2.1 Test Data 
4.2.2 Analysis of Drum Recordings 
4.2.3 Method 
4.2.4 Tests 
4.3 Analysis of the Frequency Spectra of Different Drums and Cymbals 
4.3.1 Bass Drum 
4.3.2 Tom Toms
4.3.3 Snare drum 
4.3.4 Hi-hat
4.3.5 Crash and Ride Cymbal
4.4 Training and Training Set 
4.5 Test Set 
4.6 Classification by Decision Trees 
4.6.1 Pre-Processing
4.6.2 Feature Extraction
4.6.3 Feature Sets 
4.6.4 Classification in Weka
4.6.5 Results Feature Set 1
4.6.6 Results Feature Set 2
4.6.7 Results Feature Set 3 
4.7 Classification by Templates Based on the Spectral Shape
4.7.1 Template Creation 
4.7.2 Counting Frequency Bins in the Acceptable Range
4.7.3 Counting Frequency Bins in the Acceptable Range within a Predefined Frequency Band 
4.7.4 Calculating the Distance from the Acceptable Range 
4.8 Classification of Simultaneously Played Strokes 
4.8.1 Test set 
4.8.2 Classification of Simultaneous Strokes by Subtraction 
4.8.3 Classification of Simultaneous Strokes by Extension of the Training Set
4.9 Web Audio Demo Application 
5 Discussion and Outlook 115
