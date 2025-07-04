# 🏙️ Urban Development Trends using SpaceNet 7 Dataset

This project explores **urban development patterns** using high-resolution satellite imagery from the [SpaceNet 7 Multi-Temporal Urban Development Dataset](https://www.kaggle.com/datasets/amerii/spacenet-7-multitemporal-urban-development). The goal is to extract meaningful **spatiotemporal insights** about how urban areas evolve over time, with a particular focus on **seasonal and temporal changes**.
Implemented two complementary approaches for urban development analysis using extracted binary building masks from 60+ satellite image tiles.

##-Approach 1 (Clustering): Used pixel-based KMeans clustering to detect construction by comparing first and last month's masks, and to identify monthly growth patterns without geographic data.
##-Approach 2 (IOU + Distance): Utilized geographic coordinate data from building masks to track individual buildings using IOU and distance-based matching across months.

---

## 🎯 Key Objectives

- To analyze urban development over time using multi-temporal satellite imagery.

- Perform monthly and seasonal analysis of urban expansion.

- Visualize and interpret change using heatmaps and bar plots for insights.

---

## 📂 Dataset Overview

**Source**: [Kaggle - SpaceNet 7 Multi-Temporal Urban Development Dataset](https://www.kaggle.com/datasets/amerii/spacenet-7-multitemporal-urban-development)

- Satellite imagery from **Maxar’s WorldView-2/3 sensors**
- Covers **101 global Points of Interest (POIs)** from **2018 to 2020**
- Each POI includes **time-series satellite imagery** and corresponding **building footprint labels**
- High spatial resolution (~0.3m), ideal for urban analysis
- Includes both **RGB and Near-Infrared (NIR)** bands

---

## 🌍 Geographic and Temporal Coverage

- Data spans **3 years (2018–2020)** with multiple time steps per location  
- Global distribution of POIs enables **cross-regional urban comparison**
- Images are **georeferenced**, allowing integration with GIS tools

---

## 🛠️ Tools & Libraries

- Python (Pandas, NumPy)
- GeoPandas
- Matplotlib / Seaborn
- Rasterio, Shapely
- Optional: Folium for interactive mapping

---
