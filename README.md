# ViTAttnViz
MVP to visualize attention of a ViT network's attention tables

# Setup
Please setup a `venv` to install requirements.

# What is here
1. `visualizer_template.html` a JS/HTML library to let you make attention maps of ViT attention values (you can look at it to see demo data directly in JS/HTML).
2. `compiler.py` a CLI and function to try and visualize HTML pages for your images and ViT attention tensors. You can run it to get a demo using the demo data, but written to a new HTML file with python-generated values and code generation.
3. `jupyter_demo_dummy_tensors.ipynb` a demo that just uses the compiler on the demo data (you can get it to see that this works in JUPYER specifically).
4. TODO there will be a demo using Segment Anything 2.0 (SAM-2).

# How to run
1. Just open in a browser.
2. Please run the script below (with title for this).
3. Just run the jupyter.
4. Same as 2 but the following one.

## Running CLI Demo
```bash
python3 compiler.py ./demo/cat.png ./demo/horse.png ./demo/spacex.png \
    --input-file visualizer_template.html \
    --output-file visualizer.html \
    --no-clobber
```

## Running With SAM 2.0 (Segment Anything 2.0)
TODO(Adriano)