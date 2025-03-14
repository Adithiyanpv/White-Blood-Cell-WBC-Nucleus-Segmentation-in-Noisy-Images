# White Blood Cell (WBC) Segmentation

This repository contains the documentation and results of our study on white blood cell segmentation, a critical task in medical image analysis for diagnosing hematologic conditions such as leukemia.

---

## 1. Problem Definition & Dataset Overview

### 1.1 Problem Selection

White blood cell (WBC) segmentation is a crucial task in medical image analysis, particularly for diagnosing diseases like leukemia and other hematologic conditions. Accurate segmentation of WBC nuclei is essential to distinguish different types of white blood cells, including neutrophils, basophils, eosinophils, and monocytes. However, real-world microscopic images are often affected by noise due to staining variability, uneven illumination, and artifacts during slide preparation. This noise hampers accurate object detection and segmentation.

## Results We Achieved

<table style="width: 100%; border-collapse: collapse;">
  <thead>
    <tr>
      <th style="text-align: center; padding: 10px; border: 1px solid #ddd;">Input Image</th>
      <th style="text-align: center; padding: 10px; border: 1px solid #ddd;">Output Produced by our approach (RED BORDER)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/WhatsApp%20Image%202025-03-13%20at%2019.20.39.jpeg?raw=true" alt="Input Image 1" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/WhatsApp%20Image%202025-03-13%20at%2019.20.55.jpeg?raw=true" alt="Output Image 1" width="200" style="border: 3px solid red;"/>
      </td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/WhatsApp%20Image%202025-03-13%20at%2019.21.54.jpeg?raw=true" alt="Input Image 2" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/WhatsApp%20Image%202025-03-13%20at%2019.22.07.jpeg?raw=true" alt="Output Image 2" width="200" style="border: 3px solid red;"/>
      </td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/WhatsApp%20Image%202025-03-13%20at%2019.23.19.jpeg?raw=true" alt="Input Image 3" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/WhatsApp%20Image%202025-03-13%20at%2019.23.30.jpeg?raw=true" alt="Output Image 3" width="200" style="border: 3px solid red;"/>
      </td>
    </tr>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/WhatsApp%20Image%202025-03-13%20at%2019.24.39%20(1).jpeg?raw=true" alt="Input Image 4" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/WhatsApp%20Image%202025-03-13%20at%2019.25.37.jpeg?raw=true" alt="Output Image 4" width="200" style="border: 3px solid red;"/>
      </td>
    </tr>
  </tbody>
</table>

## Our own methodology which we used

<table style="width: 100%; border-collapse: collapse;">
  <thead>
    <tr>
      <th style="text-align: center; padding: 10px; border: 1px solid #ddd;">Original Image</th>
      <th style="text-align: center; padding: 10px; border: 1px solid #ddd;">Extracted Blue Plane</th>
      <th style="text-align: center; padding: 10px; border: 1px solid #ddd;">Binarized Image</th>
      <th style="text-align: center; padding: 10px; border: 1px solid #ddd;">Morphological Results</th>
      <th style="text-align: center; padding: 10px; border: 1px solid #ddd;">Background</th>
      <th style="text-align: center; padding: 10px; border: 1px solid #ddd;">Final Segmented Image</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/Screenshot%202025-03-14%20110843.png" alt="Original Image" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/Screenshot%202025-03-14%20110914.png" alt="Extracted Blue Plane" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/Screenshot%202025-03-14%20110932.png" alt="Binarized Image" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/Screenshot%202025-03-14%20110949.png" alt="Morphological Results" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/Screenshot%202025-03-14%20111006.png" alt="Background" width="200"/>
      </td>
      <td style="text-align: center; padding: 10px; border: 1px solid #ddd;">
        <img src="https://github.com/rahulbio/30_days_of_dsa/blob/main/Screenshot%202025-03-14%20111022.png" alt="Final Segmented Image" width="200"/>
      </td>
    </tr>
  </tbody>
</table>

---

## 2. Preprocessing & Filter Comparison

### Visual Comparison of Filters

- **Gaussian Filter:**  
  Produced smoother images but blurred small, detailed objects.

- **Median Filter:**  
  Preserved object boundaries while effectively removing isolated noise.

- **Wiener Filter:**  
  Reduced Gaussian noise while preserving fine image details. Compared to Gaussian blur, it maintained sharper edges by reducing noise more adaptively; however, its performance decreased in regions with high noise variance.

- **Bilateral Filter:**  
  Reduced noise while maintaining sharp edges, outperforming Gaussian and Wiener filters in preserving structural boundaries at the cost of higher computational expense.

---

## 3. Segmentation Techniques

Segmentation separates the foreground (WBC nuclei) from the background, which is critical for analyzing biological structures. We experimented with three segmentation algorithms:

### 3.1 K-Means Clustering

K-Means clustering is an unsupervised algorithm that partitions the image into clusters based on pixel intensity. We used it to segment the image into cell regions, background, and noise. Although it is computationally efficient and simple, it struggles with non-uniform illumination and overlapping regions. This method provided reasonable object separation but failed to capture finer object boundaries accurately.

### 3.2 Mean-Shift Segmentation

The Mean-Shift algorithm is a mode-seeking process that clusters pixels by iteratively shifting points toward areas of high density. Being non-parametric, it does not require a predefined number of clusters. Our experiments demonstrated that Mean-Shift segmentation not only produced smoother object boundaries but also excelled in differentiating subtle color differences (e.g., clearly distinguishing red and purple colored cells). Despite its computational intensity and slower performance on larger images, its emphasis on color makes it particularly effective for our application.

### 3.3 Graph-Based Segmentation

Graph-based segmentation treats the image as a graph where pixels are nodes connected by edges weighted by pixel similarity. We applied the Felzenszwalb algorithm, which produces region-based segmentation. This method accurately delineated object boundaries and separated closely connected objects. While it successfully detected all cells, it did not differentiate them based on color as effectively as Mean-Shift segmentation.

#### Visual Comparison of Segmentation Methods

- **K-Means:**  
  Resulted in coarse regions with inaccurate boundaries.

- **Mean-Shift:**  
  Captured smoother, more natural boundaries with superior color-based segmentation.

- **Graph-Based:**  
  Provided the most accurate boundary detection and object separation but lacked precision in color differentiation.

#### Summary Table

| **Technique**                | **Key Characteristics**                                                                                                                                       |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **K-Means Segmentation**     | Produced coarse segmentation with clear but rigid boundaries. Struggled with complex shapes and overlapping regions.                                          |
| **Mean-Shift Segmentation**  | Generated smoother and more natural object boundaries. Excels at color-based segmentation, effectively differentiating subtle color variations.              |
| **Graph-Based Segmentation** | Successfully detected all cells with highly accurate boundary detection, yet did not differentiate cells based on color as precisely as Mean-Shift.            |

> **Note:** In our experiments, **Mean-Shift segmentation** demonstrated a superior ability to distinguish subtle color variations (e.g., red vs. purple cells), making it the best choice for color-based segmentation tasks.

---

## 4. Our Approach

Our methodology combined color-based segmentation, morphological operations, and the watershed algorithm for precise boundary delineation:

1. **Preprocessing:**  
   - **Color Conversion:** The input image was converted from BGR to RGB for visualization.
   - **Blue-Plane Extraction:** A custom formula was used to extract the blue plane by subtracting half of the red and green channel intensities. This enhanced the contrast of the WBC nuclei relative to the background.

2. **Binary Mask Creation:**  
   - A threshold of **29** was applied (empirically determined via histogram analysis) to generate a binary mask.
   - Small objects with an area of less than **1000 pixels** were filtered out.
   - Morphological operations (closing and opening with an elliptical kernel) were applied to fill small holes and remove residual noise.

3. **Watershed Segmentation:**  
   - A distance transform was computed to emphasize the central regions of the nuclei.
   - Sure foreground and sure background regions were identified through thresholding and dilation, respectively.
   - The difference between these regions highlighted the unknown areas, where connected component labeling was used to mark nuclei.
   - The watershed algorithm was then applied, marking the nuclei boundaries distinctly in red.

4. **Evaluation:**  
   - The segmented output was compared to a pseudo-ground truth generated from the processed binary image.
   - Metrics such as **Intersection over Union (IoU)**, **Dice coefficient**, and **pixel accuracy** were computed.
   - Additional analyses included counting segmented nuclei, calculating nucleus area, and determining circularity to assess shape consistency.

---

## 5. Results and Discussion

### Quantitative Metrics and Nuclei Segmentation Details

| **Metric**                         | **Value / Description**                                                                                                                                                              |
|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Pixel Accuracy**                 | `0.9871`<br>98.71% of the pixels in the segmented image match the pseudo-ground truth, demonstrating high classification accuracy.                                               |
| **Intersection over Union (IoU)**  | `0.7610`<br>This score indicates a strong overlap between the segmented regions and the ground truth; a value above 0.7 is generally considered good.                              |
| **Dice Coefficient**               | `0.8643`<br>A Dice score close to 1.0 indicates excellent segmentation performance, balancing both precision and recall.                                                            |
| **Number of Segmented Nuclei**     | `1`<br>Indicates either a single nucleus was present or multiple overlapping nuclei were merged into one segment.                                                                   |
| **Area of Nucleus**                | `5166 pixels`<br>Provides a quantitative measure of the nucleus size, important for biological analysis.                                                                             |
| **Circularity of Nucleus**         | `0.57`<br>Suggests the nucleus has a moderately circular shape, typical for biological structures.                                                                                  |

---

## 6. Conclusion and Future Work

This study implemented and compared multiple image processing techniques for noise reduction, segmentation, and object extraction. Key findings include:

- **Noise Reduction:**  
  The median filter was superior due to its edge-preserving capabilities.

- **Segmentation:**  
  While Graph-Based segmentation delivered highly accurate boundary detection, Mean-Shift segmentation excelled at differentiating cells based on color, particularly in distinguishing subtle differences (e.g., red versus purple cells).

- **Post-Processing:**  
  Region-growing and connected component analysis further refined the segmentation by enhancing object completeness and reducing noise.

### Future Work

- **Integration with Deep Learning:**  
  Incorporate deep learning models to further improve segmentation accuracy.

- **Real-Time Processing:**  
  Optimize the pipeline for real-time applications.

- **User Interface Development:**  
  Create a user-friendly interface to facilitate easy use and visualization of results.

These enhancements aim to increase the robustness, usability, and real-world applicability of the segmentation system.

---

*End of Documentation*
