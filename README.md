# 📌 Robust Virtual Content Integration and Occlusion Handling in 2D Video Streams  

**Author:** Aashka Desai  
**Year:** 2024  

---

## 📖 Overview  

This project introduces a robust system for **seamlessly overlaying virtual content** (such as logos and scoreboards) in live sports broadcasts while addressing key challenges like **player occlusion, camera vibrations, and real-time processing constraints**. By leveraging state-of-the-art **computer vision and AI techniques**, this system ensures overlays remain stable and realistic even in dynamic video conditions.  

---

## 🛠️ Key Features  

✅ **YOLOv5-based Object Detection** – Identifies static elements (stumps, pitch lines) and moving players in real-time.  
✅ **Dynamic Masking for Occlusion Handling** – Ensures virtual overlays do not cover players unnaturally.  
✅ **Camera Vibration Compensation** – Uses displacement tracking and smoothing algorithms to stabilize overlays.  
✅ **Edge Detection & ROI Definition** – Detects pitch boundaries and refines overlay placement for accuracy.  
✅ **Real-time Performance Optimization** – Ensures low-latency processing suitable for live broadcasting.  

---

## 🎯 System Workflow  

1️⃣ **Stump & Pitch Detection**  
   - Uses **YOLOv5** to detect static elements like stumps and pitch lines.  
   - Defines a **Region of Interest (ROI)** to focus processing only on relevant areas.  

2️⃣ **Player Detection & Dynamic Masking**  
   - Detects players and umpires to prevent overlay interference.  
   - Applies **real-time masking** to respect natural occlusions.  

3️⃣ **Displacement Tracking & Camera Stability**  
   - Tracks marker movements within ROI to **compensate for camera vibrations**.  
   - Smooths overlay positioning to prevent jitter.  

4️⃣ **Dynamic Banner Placement**  
   - Ensures **logos and scoreboards remain stable** within the video stream.  

---

## 📊 Performance & Results  

🔹 **High Detection Accuracy** – YOLOv5 achieves **near-perfect identification** of static and moving objects.  
🔹 **Real-time Processing** – Average frame latency: **50.41ms**, ensuring smooth performance.  
🔹 **Stable Overlays** – Displacement tracking minimizes visual jitter caused by camera motion.  

### 📈 Key Metrics  

| Metric | Value |
|--------|--------|
| **YOLOv5 Confidence Score** | ~1.0 (Near-perfect) |
| **Frame Processing Latency** | ~50.41ms |
| **Frames Processed in <60ms** | ~90% |
| **Overlay Stability** | High (Even in dynamic conditions) |

---

## 🚀 Future Enhancements  

🔹 Improve detection accuracy for extreme **motion blur and occlusions**.  
🔹 Optimize model performance using **hardware acceleration**.  
🔹 Implement **adaptive blending** for even more realistic overlay integration.  
🔹 Expand the system for **AR, film production, and interactive experiences**.  


