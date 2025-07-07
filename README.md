#  Dynamic Parking Pricing System

This project implements a multi-model, dynamic pricing system for parking lots, developed as part of a data science competition. It adjusts parking prices based on real-time factors like occupancy, queue length, traffic level, and competition with nearby lots. The final model can recommend rerouting drivers or changing prices, maximizing both revenue and lot utilization.

---

##  What this repo contains

- A **Google Colab notebook** with:
  - Model 1: occupancy-based pricing.
  - Model 2: multi-factor demand pricing with thresholds.
  - Model 3: competitive pricing with referrals and location intelligence.
  - Visualizations for prices, referral scores, and decisions.

- A **report PDF** summarizing:
  - Assumptions and thresholds used.
  - Demand functions and pricing logic.
  - Key insights and conclusions.

- Supporting code and documentation.

---

## 🛠 Tech Stack

- Python, Pandas – data analysis and modeling
- Bokeh – interactive visualizations
- Pathway – streaming data pipelines
- Jupyter/Colab – running and documenting the project

---

## 📐 Architecture Diagram

```mermaid
flowchart TD
    A[CSV Data or Streaming Data]
    B[Pathway Pipeline]
    C[Compute Lot State]
    D[Calculate Referral & Distance Scores]
    E[Make Decision: Refer or Adjust Price]
    F[Write Results to CSV & Generate Plots]

    A --> B --> C --> D --> E --> F
