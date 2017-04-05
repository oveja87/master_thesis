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
are tested with Matlab and Weka.

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
1. Introduction
1. Basic Concepts
    1. Easydrum
        1. Technologies 
        1. Architecture 
    1. Components of a Drum Set 
    1. Notation 
    1. Audio Signal Processing 
        1. Audio Signals 
        1. Sampling and Quantization 
    1. Frequency Spectrum Analysis of Digital Signals 
        1. Discrete Fourier Transformation 
        1. Short Time Spectral Analysis and Windowing 
        1. Fast Fourier Transformation 
    1. Onset Detection 
    1. Classification 
    1. Feature Extraction
        1. Feature Based Classification
        1. Decision Trees
        1. Further Classification Methods 
        1. Evaluation
    1. Tools
        1. MatLab
        1. Weka 
    1. Audio Processing in the Web 
1. Related Work 
    1. Onset Detection 
    1. Classification 
    1. Real-Time Approach 
1. Methods 
    1. Test Drum Set and Hardware 
    1. Onset Detection 
        1. Test Data 
        1. Analysis of Drum Recordings 
        1. Method 
        1. Tests 
    1. Analysis of the Frequency Spectra of Different Drums and Cymbals 
    1. Bass Drum 
        1. Tom Toms
        1. Snare drum 
        1. Hi-hat
        1. Crash and Ride Cymbal
    1. Training and Training Set 
    1. Test Set 
    1. Classification by Decision Trees 
        1. Pre-Processing
        1. Feature Extraction
        1. Feature Sets 
        1. Classification in Weka
        1. Results Feature Set 1
        1. Results Feature Set 2
        1. Results Feature Set 3 
    1. Classification by Templates Based on the Spectral Shape
        1. Template Creation 
        1. Counting Frequency Bins in the Acceptable Range
        1. Counting Frequency Bins in the Acceptable Range within a Predefined Frequency Band 
        1. Calculating the Distance from the Acceptable Range 
    1. Classification of Simultaneously Played Strokes 
        1. Test set 
        1. Classification of Simultaneous Strokes by Subtraction 
        1. Classification of Simultaneous Strokes by Extension of the Training Set
    1. Web Audio Demo Application 
1. Discussion and Outlook 115
