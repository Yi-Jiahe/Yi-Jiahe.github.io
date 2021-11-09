# Guitar Companion

The guitar companion is a collection of tools written in Python, utilizing PortAudio which visualizes and transforms audio input. It is so named as many of the transformations are based off guitar effects, with the user interface built to look like a pedalboard. The system worked by taking the real time audio input from a microphone, which could also be the output of an electric guitar, and progressively altering the signal across a number of modular effects, before returning it to the speaker.

![Effects Board](\assets\images\eguitarmod\EffectsBoard.png)

Visualization options included the time-amplitude plot of the transformed plot alongside the fourier domain frequency plot of the transformed signal and a frequency-time spectrogram. Transformation options included amplitude adjustment, equalization and modulation and frequency shifting.

![Signal Visualizer](\assets\images\eguitarmod\SignalVisualizer.png)

The main learning points I obtained from this project was an insight into digital signal processing and some practical experience with the numerical operations that can be performed on digital signals, as well as how to handle real time buffer data.

### [Back to Home](/)
