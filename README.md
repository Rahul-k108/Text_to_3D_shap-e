# Text_to_3D_shap-e

🧠 Text-to-3D Model Generator using Shape-E
This project allows you to generate 3D models (.obj and .stl) from text prompts using OpenAI's Shape-E model. It supports running in Google Colab, automatically handles STL conversion, and lets you download the results.



🏗️ How Does It Work?

Choose Device: Automatically uses GPU if available, otherwise falls back to CPU.

Load Models: Downloads pre-trained SHAP-E models.

User Input: Enter a text prompt (like “a futuristic chair”).

Generate Model: Click the button, and the code:

Generates a 3D mesh from your prompt.

Saves it as both .obj and .stl.

Gives you download links.

(Optionally) Displays the model right in your notebook.



🛠️ Code Structure

Model Loader: Loads pre-trained text300M & transmitter models

Latent Generator: Generates latents from text

Mesh Decoder: Converts latents into 3D mesh

STL Exporter: Uses trimesh for STL

UI: Built with ipywidgets for prompt input and button handling



🛠️ Troubleshooting

Corrupt Clone?

Delete with !rm -rf shap-e and try cloning again.

No requirements.txt?

That’s normal-just use pip install -e . in the shap-e folder.



🖥️ UI Components

text_input: Enter prompt

generate_button: Triggers model generation

output: Displays logs, errors, download links



📦 File Outputs

/content/output_model.obj - Standard 3D object file.

/content/output_model.stl - Ready for 3D printing.
