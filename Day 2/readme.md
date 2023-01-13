
T1: I opened the spectral images from my measurement session. I then opened the spectral .raw file of images that were marked with a red check mark, as we did in lectures on Colab, using the data from the respective .hdr file.

T2: I attempted to open an ENVI format spectral camera image in Colab, which was acquired by a Japanese camera. However, it was noted that this camera does not have a header file. The known information about the camera includes a sensor resolution of 1280x1024 and the data type being uint16. The number of bands in the image is not known, but the image is in the ENVI format.

T3: I opened the ENVI format image from the camera, which has a different byte order parameter. To do this, I used the appropriate function and passed the necessary parameter to open the image with the correct byte order. Once the image was opened, I previewed it.

T4: I saved the ENVI format spectral image with the interleave set to "bil/bip". I then loaded it in Colab and modified the spectral cube so that I could save it with an interleave of "bip". I saved the new spectral cube as an ENVI spectral file. I then manually modified the .hdr header file to reflect the change in the interleave to "bip".

