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
