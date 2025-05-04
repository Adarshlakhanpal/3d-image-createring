
# Photo/Text to 3D Model Generation and Viewer

This repository contains two Jupyter notebooks that demonstrate the generation and visualization of 3D models from either text or photo input using AI-powered techniques.

## 📁 Notebooks

### 1. `Photo_or_Text_to_3D_Model.ipynb`
This notebook allows users to input either a **photo** or **text description**, and generates a corresponding 3D model using a pretrained model (e.g., via OpenAI's Point-E or a similar framework). It provides:
- Image and prompt input interface
- Model generation pipeline
- Visualization of the 3D model (e.g., point cloud)

### 2. `Prompt-to-3D Shape Viewer.ipynb`
This notebook focuses on **prompt-to-3D** workflows, enabling:
- Direct generation of 3D models from natural language prompts
- Interactive 3D visualization of the result
- Useful for inspecting generated shapes before export or further processing

## 🛠️ Requirements

Install the following packages before running the notebooks:

```bash
pip install open3d matplotlib torch torchvision transformers ipywidgets
```

Depending on the model used (e.g., Point-E), you may also need:

```bash
pip install git+https://github.com/openai/point-e.git
```

## 📌 Features

- 🔤 Text-to-3D model generation
- 🖼️ Photo-to-3D model conversion (if supported)
- 🌀 Point cloud and mesh visualization
- 🧠 Integrates with pretrained generative models

## 📂 Output

The generated 3D shapes are typically saved as:
- `.ply` or `.obj` files
- Displayed in a browser using `Open3D`, `Plotly`, or other visualization tools

## 🧪 Usage

1. Open either notebook in Jupyter or JupyterLab.
2. Provide a text prompt or image input.
3. Run the cells to generate and view the 3D model.

## 📸 Example Prompts

- `"A red sports car"`
- `"A medieval castle"`
- `"An astronaut on the moon"`

## 🔒 License

This project is for educational and research use only. Check the licenses of external models/libraries used (e.g., OpenAI Point-E).

## 🙌 Acknowledgements

- [OpenAI Point-E](https://github.com/openai/point-e)
- [Open3D](http://www.open3d.org/)
- [HuggingFace Transformers](https://huggingface.co/transformers/)
