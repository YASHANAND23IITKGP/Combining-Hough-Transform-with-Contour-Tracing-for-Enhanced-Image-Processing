# Combining-Hough-Transform-with-Contour-Tracing-for-Enhanced-Image-Processing
This is a Python implementation of the Fast Hough transform. It was done as a course Capstone project for Signal Processing System Design Laboratory (EE69205), under the guidance of Prof. Debdoot Sheet.

* The project report can be found [here](https://drive.google.com/file/d/1RZk386iDRkE_KJBXhzf-fqDofLo6PBYf/view?usp=drive_link).
* The paper can be found [here](https://ieeexplore.ieee.org/document/7782813).
* The official website for the project can be found [here](https://sites.google.com/view/xjguo/lime). The demo software provided by the authors contains `.p` mat files, for which source code can't be read.

This algorithm leverages an enhanced Hough transform, optimizing the classic approach by incorporating insights from a contour tracing technique known as the Moore-Neighbor algorithm. Departing from the conventional method of generating all potential lines for each edge map pixel, this approach selectively computes lines that genuinely pertain to the image. The objective is to streamline the process and focus computational efforts on lines with significant relevance to the given image.

#### Our Proposed Method
The idea behind the project is to keep track of the last contour's pixels and calculate the parameters only for a limited set of lines, instead of all the possible lines that pass through each point of the edge map. 
<br> 
![Basic idea](https://github.com/MarcoCadei/Fast-Hough-Contour/blob/master/images/intuition.png)

