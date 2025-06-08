# Misspecified Statistics and Autoregressive Processes: An Analysis of Cramér-Rao Bounds

This research project, supervised by two professors from Télécom SudParis and conducted by three students, contains the code and resources investigating the crucial role of misspecified statistics in signal processing, particularly when model assumptions, such as data Gaussianity, are violated.

Our work is fundamentally based on the methodologies and insights presented in the following key research papers:

* "Matched, mismatched, and robust scatter matrix estimation and hypothesis testing in complex t-distributed data" by *Stefano Fortunati, Fulvio Gini, and Maria S. Greco (EURASIP Journal on Advances in Signal Processing, 2016)*.
* "Performance Bounds for Parameter Estimation under Misspecified Models" by *Stefano Fortunati, Fulvio Gini, Maria S. Greco, and Christ D. Richmond (Published by IEEE)*.

Leveraging these works, we focus on the **complex t-distribution** and **autoregressive (AR(1)) processes** to demonstrate the limitations of classical estimation tools like the standard **Cramer-Rao Bound (CRB)**. We show that the CRB can significantly underestimate the true variance of estimators when the underlying data model is incorrectly assumed.

## Key Contributions and Findings

* **Implementation and analysis of the Misspecified Cramer-Rao Bound (MCRB):** We demonstrate that the MCRB, as derived in the referenced papers, provides a more realistic assessment of estimator precision, especially when data deviates from Gaussianity. Our simulations illustrate that the MCRB becomes notably higher than the standard CRB under these conditions, a discrepancy that persists even with large sample sizes.
* **Comparison of matched, mismatched, and robust approaches:** The project delves into the implications of using estimators designed for a specific data distribution versus those robust to model deviations, building upon the theoretical frameworks.
* **Application to AR(1) processes:** We extend the analysis to dynamic systems, highlighting the impact of misspecification in time-series modeling.
* **Practical implications:** The results underscore the importance of employing adaptive estimators, such as those derived from the Newton method for t-distributed noise, to achieve significant improvements in estimation performance under misspecified conditions.

This project underscores the need for robust statistical approaches in real-world signal processing applications where ideal data conditions are rarely met.

## Project Report & Code

The full project report is available(`Cassiopee_Project_Report.pdf`).
An associated Jupyter Notebook containing the implementation and analysis is also uploaded to this repository.
