# Project Name: Bone Fracture Line Detection System

### Project Description:
#### Summary - 
We have attempted to develop a Fracture Line Detection System using MATLAB and its Image Processing 
Toolbox. The system aims to assist radiologists by processing X-ray images to automatically highlight potential bone fractures. The methodology involves Image Enhancement, Edge Detection and Segmentation. The core of the algorithm isolates internal fracture lines by logically subtracting the external bone perimeter 
(derived from the mask) from the complete set of Canny edges. The system successfully processes an X-ray, cleans the resulting candidates, and overlays the final detected fracture line in red on the original image, providing a clear visual aid for diagnosis. 

#### Course concepts used - 
1. Grayscale conversion
2. Image Enhancement
3. Dilation
4. Edge detection
5. Opening

   
#### Additional concepts used -
1. Anisotropic Diffusion
2. Contrast Adjustment
3. Seeded region growing
   
#### Dataset - 
[1] “Simple oblique or spiral tibial fracture,” Aofoundation.org, 
https://surgeryreference.aofoundation.org/orthopedic-trauma/pediatric-trauma/tibial-shaft/tibia-simpleoblique-or-spiral/definition#x-ray 

[2] B. M. Rafi and V. Tiwari, “[Figure, An x-ray of right forearm showing isolated ulna fracture Contributed by Vivek Tiwari],”www.ncbi.nlm.nih.gov,Aug.https://www.ncbi.nlm.nih.gov/books/NBK574580/figure/article-137044.image.f3/ 08,2023. 

#### Novelty - 
1. Hybrid Spatial Subtraction technique combining region-based and edge-based segmentation.

2. Dynamic exclusion mask generated from Region Growing of the bone and its morphological boundary.

3. Logical subtraction of the bone’s external contour from the global edge map to isolate true fracture lines.

4. Automatic separation of pathological internal discontinuities from healthy anatomical edges—beyond what standard edge detectors can achieve alone.

5. Anisotropic Diffusion preprocessing preserves fracture-relevant edges while suppressing X-ray noise.

6. Pure classical digital image processing pipeline. No deep learning or black-box models involved.

7. Fully implemented in MATLAB, ensuring reproducibility, transparency, and ease of modification.

   
### Contributors:
1. Shreya Rose Jimson (PES1UG23EC289)
2. Aryan Deshpande (PES1UG23EC059)

### Steps:
1. Clone Repository
```git clone https://github.com/Digital-Image-Processing-PES-ECE/project-name.git ```

2. Install Dependencies
```pip install -r requirements.txt```

3. Run the Code
```python main.py (for eg.)```

### Outputs:
* Important intermediate steps
* Final output images 

### References:
1. -
2. -
   
### Limitations and Future Work:
