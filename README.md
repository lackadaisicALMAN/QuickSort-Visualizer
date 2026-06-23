# QuickSort-Visualizer
Simple yet elegant visualizer to better understand Quick Sort method.


> **Live Demo:** https://lackadaisicalman.github.io/QuickSort-Visualizer/

This is a high-performance, aesthetically driven Quick Sort Visualizer built to make algorithmic tracking instantly intuitive (and look incredibly cool while doing it). 

Designed with a sleek, dark sci-fi dashboard theme, this visualizer moves away from standard, boring bar charts and uses glowing neon telemetry to show exactly how the pivot selection and partitioning steps happen in real-time.

---

## 👤 Student Information
* **Name:** Salman
* **Roll Number:** BSAI24067
* 
---

## 🎨 Visual States & Color Legend

To make the recursive nature of Quick Sort easy to follow, the elements dynamically shift colors based on their algorithmic state:
* **Icy Blue (Default):** Unsorted, inactive elements in the current sub-array.
* **⚡ Hot Pink / Neon Purple:** The current **Pivot** element.
* **🟢 Emerald Green (Left Pointer):** Scanning from the left to find elements greater than the pivot.
* **🔵 Electric Cyan (Right Pointer):** Scanning from the right to find elements smaller than the pivot.
* **👑 Glowing Gold:** Elements that have found their final, correctly sorted position. Includes a brief structural shimmer effect upon settling.

---

## 🧠 The Math Behind the Magic (Quick Sort Complexity)

Quick Sort is a Divide-and-Conquer algorithm. It picks an element as a pivot and partitions the given array around the picked pivot. 

### ⏱️ Time Complexity
* **Best Case: $\mathcal{O}(n \log n)$**
  Occurs when the pivot partition always splits the array into two nearly equal halves. The recursion tree depth is $\log n$, and processing each level takes $\mathcal{O}(n)$ time.
* **Average Case: $\mathcal{O}(n \log n)$**
  In practical scenarios with randomized data, the partitions are reasonably balanced, matching the best-case asymptotic runtime.
* **Worst Case: $\mathcal{O}(n^2)$**
  Occurs when the array is already sorted (forward or backward) and the worst possible pivot (like the smallest or largest element) is consistently chosen, causing highly unbalanced partitions.

### 💾 Space Complexity
* **Space Complexity: $\mathcal{O}(\log n)$**
  While Quick Sort sorts "in-place" (requiring $\mathcal{O}(1)$ auxiliary space for swapping elements), the recursive function calls require stack space. In the average/best case, the recursive call stack depth is $\mathcal{O}(\log n)$.

---

## 🛠️ Tech Stack
* **Frontend:** Vanilla JavaScript (ES6+ Asynchronous Promises for silky-smooth 60fps animations)
* **Styling:** Tailwind CSS CDN (Glassmorphic HUD controls, custom neon drop-shadows)
* **Structure:** Single-file `index.html` architecture for instant deployment.
