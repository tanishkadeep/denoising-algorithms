# Report on Denoising Algorithms: Performance Metrics Comparison

This report provides a comparative analysis of three denoising algorithms: **Gaussian Filter**, **Median Filter**, and **Non-Local Means Denoising**. The performance metrics were evaluated using both CPU and GPU implementations in Python and C++. The key metrics include **CPU usage**, **RAM usage**, **inference time**, **PSNR (Peak Signal-to-Noise Ratio)**, **GPU memory usage**, and **GPU load**.

## Gaussian Filter

### Python Implementation
- **CPU:**
  - **Total CPU Usage:** 27.95%
  - **Total RAM Usage:** 160.96 MB
  - **Total Inference Time:** 0.60 ms
  - **Average PSNR:** 22.94 dB
- **GPU:**
  - **GPU Memory Usage:** 1.77 MB / 22.00 MB
  - **GPU Load:** 0.0%
  - **Average Inference Time:** 1.37 ms
  - **Average PSNR:** 22.90 dB

### C++ Implementation
- **CPU:**
  - **Total CPU Usage:** 8.82%
  - **Total RAM Usage:** 95.95 MB
  - **Total Inference Time:** 0.000107843 ms
  - **Average PSNR:** 23.2 dB
- **GPU:**
  - **GPU Memory Usage:** 0 MB
  - **GPU Load:** 0%
  - **Average Inference Time:** 0.739379 ms
  - **Average PSNR:** 23.2 dB

## Median Filter

### Python Implementation
- **CPU:**
  - **Total CPU Usage:** 56.4%
  - **Memory Usage:** 10.8%
  - **Inference Time:** 642.84 ms
  - **PSNR:** 23.77 dB
- **GPU:**
  - **GPU Memory Usage:** 3.53 MB / 20.00 MB
  - **GPU Load:** 0.0098%
  - **Inference Time:** 4.84 ms
  - **PSNR:** 21.45 dB

### C++ Implementation
- **CPU:**
  - **Total CPU Usage:** 4.90%
  - **Total RAM Usage:** 95.84 MB
  - **Total Inference Time:** 3.92157e-05 ms
  - **Average PSNR:** 27.73 dB
- **GPU:**
  - **GPU Memory Usage:** 103 MB
  - **GPU Load:** 0%
  - **Average Inference Time:** 5.98327 ms
  - **Average PSNR:** 21.45 dB

## Non-Local Means Denoising

### Python Implementation
- **CPU:**
  - **Total CPU Usage:** 41.8%
  - **Total RAM Usage:** 1026.22 MB
  - **Average Inference Time per Image:** 614.09 ms
  - **Average PSNR:** 26.01 dB
- **GPU:**
  - **GPU Memory Usage:** 0 MB
  - **GPU Load:** 0.00%
  - **Average Inference Time per Image:** 503.24 ms
  - **Average PSNR:** 26.01 dB

### C++ Implementation
- **CPU:**
  - **Total CPU Usage:** 67.43%
  - **Total RAM Usage:** 95.68 MB
  - **Average Inference Time per Image:** 761.92 ms
  - **Average PSNR:** 41.36 dB
- **GPU:**
  - **GPU Memory Usage:** 0 MB
  - **GPU Load:** 0%
  - **Average Inference Time per Image:** 607.06 ms
  - **Average PSNR:** 26.01 dB
