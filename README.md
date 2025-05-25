# 🖼️ Image Compression using K-Means Clustering

This project demonstrates how to compress images by reducing the number of unique colors using the **K-Means Clustering algorithm**.

Instead of millions of colors, the compressed image uses a smaller palette (e.g.,20 colors), significantly reducing image complexity while retaining visual similarity.

---

## 🔧 Technologies & Libraries Used

- **Python**
- **PIL (Pillow)** – for image loading and saving
- **NumPy** – for numerical operations and distance calculations

---

## 🧠 How It Works

1. **Read image** using `PIL` and convert it to a NumPy array.
2. **Reshape the image** to a 2D array of pixels .
3. **Initialize K centroids randomly** from the pixels.
4. **Assign each pixel to the nearest centroid** using Euclidean distance.
5. **Recompute centroids** as the mean of assigned points.
6. Repeat steps 4–5 for several iterations.
7. **Replace each pixel** with its centroid to create a compressed image.
8. Reshape and save the image back using `PIL`.

---

