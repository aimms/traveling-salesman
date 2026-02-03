# Traveling Salesman 

[![Downloads](https://img.shields.io/github/downloads/aimms/traveling-salesman/total?style=for-the-badge&logo=github&labelColor=000081&color=1847c9)](https://github.com/aimms/traveling-salesman/releases)
![AIMMS Version](https://img.shields.io/badge/AIMMS-25.9-white?style=for-the-badge&labelColor=009B00&color=00D400)
![WebUI Version](https://img.shields.io/badge/WebUI-25.9.2.8-white?style=for-the-badge&labelColor=009B00&color=00D400)
![DEX Version](https://img.shields.io/badge/DEX-26.1.2.1-white?style=for-the-badge&labelColor=009B00&color=00D400)


This repository contains a comprehensive AIMMS example for the **Traveling Salesman Problem (TSP)**. It illustrates multiple approaches to solving one of the most famous optimization challenges: finding the shortest possible route that visits a set of cities and returns to the origin.

## 🎯 Business Problem

The TSP is a cornerstone of logistics and supply chain optimization. This model demonstrates how to:
- **Minimize Travel Distance:** Reducing fuel costs and transit time.
- **Compare Solvers:** Analyzing the trade-offs between fast **Heuristics** (2-opt) and exact **MIP** (Mixed Integer Programming) solutions.
- **Handle Subtours:** Implementing subtour elimination constraints to ensure a single, continuous tour.
- **Geocoding:** Converting city names into geographical coordinates using external Rest APIs.

## 📖 How to Use This Example

To get the most out of this model, we highly recommend reading our detailed step-by-step guide on the AIMMS How-to website:

👉 **[Read the Full Article: Traveling Salesman Guide](https://how-to.aimms.com/Articles/397/397-traveling-salesman.html)**

### Prerequisites
- **AIMMS:** You will need AIMMS installed to run the model. [Download the Free Academic Edition here](https://www.aimms.com/support/licensing/).
- **API Key:** A free API key from [PositionStack](https://positionstack.com/) is required for the geocoding features.
- **SQLite ODBC Driver:** Necessary for data integration and scenario management.

### Technical Highlights
- **Heuristic Algorithms:** Implementation of 2-opt initial, simultaneous, and cyclic heuristics with real-time visualization.
- **MIP with Lazy Constraints:** Uses a binary variable formulation with an exponential number of subtour elimination constraints added via callbacks.
- **Haversine Formula:** Precise distance calculation between geographical coordinates on a sphere.
- **REST API & DEX:** Advanced use of the AIMMS Data Exchange library to fetch and map JSON data from external web services.

## 🚀 Getting Started

1. **Download the Release:** Go to the [Releases](https://github.com/aimms/traveling-salesman/releases) page and download the `.zip` file.
2. **Set up API Key:** Open the project and enter your PositionStack access key in the `sp_apiKey` parameter.
3. **Run the Heuristics:** Use the "Heuristic" page to see the 2-opt algorithm iterating in real-time on the map.
4. **Solve to Optimality:** Switch to the MIP page to solve the problem using exact mathematical programming.

## 🤝 Support & Feedback

This example is maintained by the **AIMMS User Support Team**.
- Found an issue? [Open an issue](https://github.com/aimms/traveling-salesman/issues).
- Questions? Reach out via the [AIMMS Community](https://community.aimms.com).

---
*Maintained by the AIMMS User Support Team. We optimize the way you build optimization.*
