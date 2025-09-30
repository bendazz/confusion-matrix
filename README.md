Confusion Matrix Visualizer (Front-end only)
===========================================

This repo hosts a tiny, framework-free web app to help students build intuition for binary classification before introducing confusion matrices.

What’s included
---------------

- `index.html` — A single-page app that:
	- Plots a simple 1D binary dataset with two classes:
		- Blue points at y = 0
		- Red points at y = 1
	- Draws an adjustable sigmoid curve p = σ(wx + b)
	- Lets you regenerate the dataset and tweak distribution parameters

How to run
----------

No build is required. You can open `index.html` directly in a browser, or serve it from a simple static file server to avoid cross-origin issues with local file URLs.

Option A: Open directly

1. Double-click `index.html` in your file explorer, or drag it into your browser.

Option B: Use a simple local server (recommended)

1. Python 3
	 - Navigate to this folder and run a simple HTTP server, then visit the printed URL in your browser.
	 - Example commands (pick one):
		 - `python3 -m http.server 8000`
		 - `python -m http.server 8000`

What’s next
-----------

- Add a threshold slider to create predictions from the sigmoid and compute TP/FP/TN/ FN live.
- Display the confusion matrix and derived metrics (accuracy, precision, recall, F1).
- Let students move points manually and see how the matrix changes.
# confusion-matrix