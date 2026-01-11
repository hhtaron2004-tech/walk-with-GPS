# 🗺 Yerevan Walk and Car Trajectory Analysis

This project analyzes GPS and altitude data collected from walks and car trips in Yerevan. The goal is to calculate distances, speeds, accelerations, and visualize the 2D and 3D trajectories of movement.

## 📊 Features

- Data Processing:

> - Converts latitude and longitude from degrees to radians.

> - Calculates 3D distances between consecutive points using both the spherical law of cosines and Euclidean 3D distance formulas.

- Speed and Acceleration Computation:

> - Computes speed between consecutive points.

> - Estimates acceleration from speed changes.

> - Aggregates speed and acceleration over 10-minute intervals.

- Trajectory Visualization:

> - 3D plot of the full trajectory showing latitude, longitude, and altitude.

> - 2D plot of the trajectory for simplified visualization.

- Data Analysis:

> - Histograms of latitude, longitude, and altitude distributions.

> - Mean altitude change analysis over 10-minute intervals.

## 🛠️ Tools & Libraries

Python 3

Libraries: numpy, pandas, matplotlib

## 🔢 Methodology

1. Load GPS and altitude data from CSV.

2. Convert coordinates to radians.

3. Compute distances:

 - Spherical distance: Uses latitude, longitude, and altitude differences.

 - Euclidean 3D distance: Considers Earth as a sphere and altitude.

4. Compute instantaneous speed and acceleration.

5. Aggregate speed, acceleration, and altitude changes over 10-minute windows.

6. Visualize results in 2D and 3D.

7. Analyze distributions with histograms.

## 📈 Visualization Examples

- 3D Trajectory: Shows movement over time in space.

- 2D Trajectory: Projection of the path on a map plane.

- Histograms: Displays distributions of latitude, longitude, and altitude.

## ⚡ Notes

- Distances are calculated in kilometers.

- Speeds are scaled to km/h, and acceleration is scaled appropriately.

- The project is useful for GPS trajectory analysis, urban mobility studies, or vehicle tracking simulations.
