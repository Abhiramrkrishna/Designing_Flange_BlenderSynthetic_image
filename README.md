# Rendering Flanges in Blender - Python script of the whole process

I have been working on a project focused on image processing and machine learning, involving the development of a training model to refine the detection of Flanges from a bin. My work includes modeling different shafts in Blender, building textures and various illuminations setups, using Python and Blender libraries for scripting, working with compositing nodes for image analysis and semantic segmentations, and contributing to the implementation and training of YOLO networks using a blend of synthetic and real data, focusing on refining object localization precision through iterative model enhancements. 

## This is the Blender Scripting for the Generation of Synthetic Images with annotation.

1. We are generating RGB images from the viewer viewport with dimensions 256 x 256. We are also generating iteratively the synthetic data (image) with the same resolution and size along with the corresponding annotation file.
2.  The annotation file includes the following information:
   * 1. Classes (0 since we have only one class object)
   * 2. The x and y coordinate


I am including a sample synthetic image, a training image, and a sample annotation file. The box fits nine flanges.

This is an ongoing project with regular updates. There are two approaches for the placement of flanges in the box:
- The random placement without any overlapping
  - The downside of this attempt is that, since the placement is random without any overlapping there is less possibility of more shafts in the box.
  - If the run the code for 7 flanges, if there is no space for 5 or more in the frame, there will be a check of 1000 attempts to see if there is any, and then the iteration will fail.
- The grid-based placement
  - The issue is that the randomness is limited. But more guarantee that there will be a correct number of flanges if we run the code for 5 or more.
 
I am still working on this, attempting various approaches. 
_____________________________________________________________________________________________________

Content of folders:
- Synthetic Images 
- Training Images
- Real Images
- Annotation file
- Segmented images

_____________________________________________________________________________________________________


This is an ongoing project and I cannot share the latest codes and updates. I am sharing the part of the project that I did.

