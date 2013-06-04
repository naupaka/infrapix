Infrapix
============

Python library and command line tools for processing publiclab's Infragram images and movies.


Installation
============
Debian Linux system (though Windows and OS X should also be possible with slightly different initial steps):

1. Install dependencies:
```sudo apt-get install git python-numpy python-matplotlib libav-tools ubuntu-restricted-extras```

2. Download lastest package from github:
```
    cd ~
    mkdir src
    cd src
    git clone https://github.com/Pioneer-Valley-Open-Science/infrapix.git
```

3. Run the setup script:
```
    cd infrapix
    sudo python setup.py install
```

4.  Go to a directory with an infrablue movie and run, for example to get dynamic range:
```infrapix_render -i BeePondFuschia.mp4 --show_histogram -o BeePondFuschia_NDVI_hist_dynamic-range.mp4```
    to get fixed range
```infrapix_render -i BeePondFuschia.mp4 --vim -1.0 --vmax 1.0 --show_histogram -o BeePondFuschia_NDVI_hist_dynamic-range.mp4```

5.  Wait a really long time... enjoy.  Hint, run
```infrapix_render -h``` for help.
