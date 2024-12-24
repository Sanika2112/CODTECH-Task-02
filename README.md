# CODTECH-Task-02

**Name**: SANIKA SHINDE<br>
**Company**: CODTECH IT SOLUTIONS<br>
**ID**: CT6WDS2686<br>
**Domain**: Machine Learning<br>
**Duration**: DECEMBER 5th, 2024 to JANUARY 20th, 2025<br>

## Overview of project
### Topic: TEXT-TO-IMAGE GENERATION APPLICATION
This project implements a **Text-to-Image Generation Application** using the **Stable Diffusion** model. The application inputs textual descriptions and generates high-quality visual representations of the described scenes or objects. This showcases the potential of generative AI in creating custom, photorealistic images.

---

## Features
- **Custom Image Generation**: Generates images based on user-defined prompts.
- **High-Quality Outputs**: Produces 4K resolution images with fine details.
- **Interactive Workflow**: Allows users to input prompts, specify the number of images, and save results.
- **Batch Processing**: Supports generating multiple images for multiple prompts.

---

## Requirements
The following libraries are required for the application:

```bash
pip install --upgrade diffusers transformers accelerate torch matplotlib Pillow
```

---

## Configuration
The application is designed with configurable parameters to enhance usability and performance:
- **Device**: Automatically uses CUDA (GPU) if available.
- **Seed**: Ensures reproducibility by setting a random seed.
- **Resolution**: Generates images at 3840x2160 (4K) resolution.
- **Model**: Utilizes `stabilityai/stable-diffusion-2-1` from Hugging Face.
- **Output Directory**: Saves generated images in the `./generated_images` folder.

---

## Setup and Execution

### Step 1: Clone the Repository
```bash
git clone <repository-link>
cd <repository-folder>
```

### Step 2: Install Required Libraries
```bash
pip install --upgrade diffusers transformers accelerate torch matplotlib Pillow
```

### Step 3: Run the Application
1. Open the Python file or notebook containing the code.
2. Execute the script. The main execution loop will prompt you to input:
   - A text description (e.g., *"A sunset over the mountains"*).
   - The number of images to generate.
3. View or save the generated images.

---

## Code Structure

### 1. **Library Installation and Imports**
Installs and imports necessary Python libraries like `torch`, `diffusers`, and `matplotlib`.

### 2. **Configuration Setup**
Defines parameters like device type, seed, model ID, resolution, and output directory.

### 3. **Model Loading**
Loads the Stable Diffusion model from Hugging Face with FP16 precision for faster computation.

### 4. **Image Generation**
Generates images based on textual prompts using the `generate_image()` function. Images are resized to 4K resolution and saved to the output directory.

### 5. **Image Display**
Displays generated images using `matplotlib` for user feedback.

### 6. **Batch Image Generation**
Processes multiple prompts and generates multiple images as required.

### 7. **Main Execution**
Runs an interactive loop for generating images based on user input.

---

## Example Usage
1. Run the script.
2. Input a prompt (e.g., *"A rainy window framing vibrant green plants, their leaves glistening with raindrops."*).
3. Specify the number of images (e.g., `3`).
4. View the generated images or find them saved in the `./generated_images` folder.

---

## Applications
- **Creative Design**: Concept art, visual storytelling, and graphic design.
- **Education**: Generating visual aids for teaching concepts.
- **Marketing**: Creating promotional visuals based on themes.

---

## Future Enhancements
- Integrating additional generative models for diverse styles.
- Allowing for real-time prompt refinement.
- Adding a graphical user interface (GUI) for easier usability.
