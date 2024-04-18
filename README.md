# ISIIS-mDPI-ImageProcessing
 Flat-fielding and segmenting images from the ISIIS, mDPI compact vehicle, and benchtop mDPI

These macros run in ImageJ and complete the process of flat fielding and segmentation on various iterations of shadowgraph imaging (the ISIIS, benchtop mDPI, and compact vehicle mDPI). Before running these macros in ImageJ, be sure to have your ImageJ enviornment set up correctly. First, you will need to install the Image Calculator Plus macro by following the instructions here https://imagej.net/ij/plugins/calculator-plus.html . Then you should download the StackAverage_.txt file and compile it in ImageJ by opening ImageJ and selecting Plugins -> Compile and Run. Then choose the .txt file with the Java code for StackAverage. Once both of these components are installed, you can run flat-fielding on images from these different devices.

The flat-fielding code runs on .avi files, .tiff stacks, or individual .tiffs. All of these codes will generate an average background and use that to divide it out, resulting in smooth lighting and blemish free images that are ready for segmentation.

Segmentation is the process of removing Regions of Interest (ROIs) within a certain size range as specified by the user. These ROIs are saved to their own directory and can be identified manually or automatically. An example StartupMacros.txt file is provided to demonstrate how you can use ImageJ to set up keyboard shortcuts to identify ROIs in a directory. There is also a keyboard shortcut to experiment with flat fielding a .tiff image stack. 

All macros require setting up directories on your machine for the output files or, in some cases, image statistics. Take note of when those directories are required, and edit the code to match them on your machine.

Macros for the mDPI were written by Patrick Duffy and include the full processing pipeline (flat-fielding and segmention) or itemized versions to run these processes separately.
