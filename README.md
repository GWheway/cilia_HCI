# cilia_HCI
CellProfiler scripts for analysis of cilia and other cellular components from high throughput confocal imaging. Produced using CellProfiler v.3.8.1.

Imaging plates must be immunostained with; DAPI; rabbit anti ARL13B and goat anti rabbit AlexaFluor 488; mouse anti c-myc and goat anti mouse AlexaFluor 568.

STEP 1.
'2019-06-20 Max projections GW FINAL.ccproj' takes individual output .flex image files from Perkin Elmer Opera confocal high content imaging system and i) splits blue, green and red channels, ii) produces maximum intensity projections from multiple imagees in a z-stack iii) saves maximum intensity projection images from each channel as 3 separate output 16bit .tiff files

STEP 2.
'2019-12-06 find nuclei find green cilia find red myc in nuc_b_with_outlines.cpproj' takes 16bit .tiff files produced from STEP 1 and i) identifies nuclei, ii) identifies cells, iii) identifies cilia in the green channel, iv) identifies cells with one single cilium, v) identifes nuclei with red staining, vi) measure intensity of red nuclear staining, vii) measure nuclei size, viii) measure colocalisation of red and blue nuclear staining, ix) overlay outlines on nuclei, cells, cilia, x) export data and save images with outlines.
