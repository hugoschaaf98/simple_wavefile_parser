# Simple Wavefile Parser
Ultra lightweight simple .wav LPCM decoder originaly developed for AVR 8bits targets.
Everything you need is ```wavefile.h``` which contains the parser header function ```wavefileParseHeader()```.

## How To use the example

###### Configure :
Inside ```example_parse_wavefile.c``` you can uncomment the line ```#define USE_EXAMPLE_HEADER 1```.
```
$ ./parse_wavefile
channels : 1
sampleRate : 44100
byteRate : 44100
bytesPerSample : 1
bitsPerSample : 8
dataSize : 104832
```
###### Build :
simply
```$ make```
###### Run :
if you've uncommented the line ```#define USE_EXAMPLE_HEADER 1``` simply
```$ ./example_parse_wavefile```

Otherwise you can specify filenames
```$ ./example_parse_wavefile myWaveFile0.wav myWaveFile1.wav myWaveFile2.wav```
