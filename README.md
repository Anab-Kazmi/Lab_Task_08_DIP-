 **Task 08: Image Restoration Techniques**

**Roll Number:** 2023-SE-06

### **Prompt**

*"Write a Python program using OpenCV, NumPy, Matplotlib, and scikit-image to demonstrate image restoration techniques on a grayscale image. The program should perform the following tasks:

* Allow the user to upload a grayscale image safely in Colab.
* Display the original image.
* Add noise to the image: Gaussian noise, Salt & Pepper noise, Motion blur.
* Apply restoration techniques:

  * Gaussian noise → Wiener filter
  * Salt & Pepper noise → Median filter
  * Motion blur → Inverse/Wiener filtering
* Compute the PSNR of each restored image compared to the original.
* Display Original, Noisy/Blurred, and Restored images side by side for each noise type.
* Print PSNR values for all restoration methods.
* Provide a brief analysis summarizing the best restoration method for each noise type and explain why.
* Ensure the code is well-commented, lab-ready, and compatible with Colab, with proper normalization and dtype handling."*

---

## **Objective**

The objective of this task is to demonstrate **image restoration techniques** for different types of degradation: Gaussian noise, Salt & Pepper noise, and motion blur. The task focuses on restoring image quality using suitable filters and quantitatively evaluating restoration using **PSNR**.

---

## **Methodology / Approach**

1. Upload a **grayscale image** in Google Colab using `files.upload()` and display it.
2. Add **Gaussian noise**, **Salt & Pepper noise**, and **motion blur** to the original image to create degraded versions.
3. Apply appropriate restoration techniques:

   * **Gaussian noise → Wiener filter**
   * **Salt & Pepper noise → Median filter**
   * **Motion blur → Inverse/Wiener filtering**
4. Compute the **PSNR** (Peak Signal-to-Noise Ratio) between the restored and original images to evaluate performance.
5. Display the original, degraded, and restored images **side by side** for visual comparison.
6. Summarize observations and compare the effectiveness of each restoration method.

---

## **Results / Observations**

* **Gaussian Noise:** Wiener filter successfully restores smooth intensity variations and achieves high PSNR.
* **Salt & Pepper Noise:** Median filter effectively removes impulse noise while preserving edges.
* **Motion Blur:** Wiener/Inverse filtering partially restores motion-blurred images; PSNR improvement is noticeable.
* PSNR values provide a quantitative measure of restoration quality.
* Optimal restoration depends on the type of noise; selecting the correct filter is crucial for best results.
* Advanced techniques (e.g., Non-Local Means, ML-based methods) can further improve restoration in complex scenarios.

---

## **Tools and Libraries Used**

* **Python 3.x**
* **OpenCV (cv2):** Image reading, grayscale conversion, and motion blur simulation
* **NumPy (np):** Array operations and noise simulation
* **Matplotlib (plt):** Visualization of original, noisy, and restored images
* **scikit-image (skimage):** Wiener filtering, metrics (PSNR), noise generation
* **Google Colab:** Image upload and execution environment

---

