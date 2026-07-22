# audio-scripts: various scripts for analyzing/processing/modifying audio files

### alyz
- analyze audio file with ffmpeg commands, print the summaries nicely
example:
```
$ ./alyz ../masters/ep1/padded/Z*

Loudness (LUFS): Zeroth.aif

  Integrated loudness:
    I:         -15.2 LUFS
    Threshold: -25.5 LUFS

  Loudness range:
    LRA:         7.8 LU
    Threshold: -35.4 LUFS
    LRA low:   -21.1 LUFS
    LRA high:  -13.3 LUFS


Volume data: Zeroth.aif
    n_samples: 0
    n_samples: 25244374
    mean_volume: -16.3 dB
    max_volume: -0.8 dB
    histogram_0db: 28
    histogram_1db: 752
    histogram_2db: 7391
    histogram_3db: 32025
```

### padsongs
- adds silence to the start and end of each .aif in the /raw directory

### lufs
- measures lufs of an audio file

### exportfinals 
- copies the finished /padded songs to my onedrive folder
- note that Tag Editor 2 before exporting to add metadata to each song
