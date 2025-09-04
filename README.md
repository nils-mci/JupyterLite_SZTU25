# Classroom JupyterLite (blank)

This site serves a **blank JupyterLite**: no example files, runs entirely in the browser.

## How to use
- Go to the Pages URL (after deployment).
- Drag & drop `.ipynb` or data files into the left pane, or use the Upload button.
- Use **File → Download** to save work back to your machine.

## Add your own starter materials
Put notebooks or data in the `content/` folder, then push to `main`.
They will appear in the left pane for everyone.

## Develop locally (optional)
```bash
python -m pip install "jupyterlite[pyodide]"
jupyter lite build --output-dir _output
python -m http.server --directory _output 8000
# open http://localhost:8000
