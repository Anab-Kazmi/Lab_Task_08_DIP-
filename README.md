# 2023-SE-06_Lab_Task_08_DIP-

Prompt:

Write a Python program using OpenCV, NumPy, Matplotlib, and scikit-image to demonstrate image restoration techniques on a grayscale image.
The program should perform the following tasks:
Allow the user to upload a grayscale image safely in Colab.
Display the original image.
Add noise to the image:
Gaussian noise
Salt & Pepper noise
Motion blur
Apply restoration techniques:
Gaussian noise → Wiener filter
Salt & Pepper noise → Median filter
Motion blur → Inverse/Wiener filtering
Compute the PSNR of each restored image compared to the original.
Display Original, Noisy/Blurred, and Restored images side by side for each noise type.
Print PSNR values for all restoration methods.
Provide a brief analysis summarizing the best restoration method for each noise type and explain why.
Ensure the code is well-commented, lab-ready, and compatible with Colab, with proper normalization and dtype handling.
