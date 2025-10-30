# 🖼️ Text-to-Image Generation with Stable Diffusion

This project demonstrates how to generate images from text prompts using **Stable Diffusion** and the **Diffusers** library in **Google Colab**.

---

## 🚀 Project Overview

The notebook explores different **text-to-image generation settings** and demonstrates how changes in parameters affect the **style, realism, and composition** of the resulting image.

During the experiments, several configurations were tested:
- Different models: `Stable Diffusion v1.5` and `Stable Diffusion XL`
- Varying the number of diffusion steps (`num_inference_steps`)
- Adjusting the text-to-image adherence (`guidance_scale`)
- Using GPU acceleration (`torch.autocast`, `float16`)
- Comparing rendering modes — from **photorealistic** to **artistic (watercolor)**

---

## 🎨 Current Version

The current notebook version reflects one of the experimental setups —  
a **watercolor-style** generation using `Stable Diffusion v1.5` with default parameters.

This choice demonstrates how **model defaults** and **simplified settings** (e.g., fewer inference steps and moderate guidance scale) can lead to a softer, more artistic rendering of the prompt.

**Prompt Example:**
"watercolor style, the landscape is rural, summer, village, horses are grazing in the field, early morning"

**Result:**

![example](generated_image.png)

*(Example output from the current experiment)*

---

## 🧠 Key Takeaways

- Even small changes in generation parameters can significantly alter artistic results.
- Higher `num_inference_steps` and `guidance_scale` tend to produce more detailed, realistic outputs.
- Reducing these values or using default settings results in a looser, more painterly effect.
- GPU acceleration with `torch.autocast` improves performance and enables larger model variants (e.g., SDXL).

---

## 🧰 Tech Stack
- Python, Google Colab, PyTorch  
- Hugging Face Diffusers  
- Stable Diffusion v1.5 / SDXL  

---

## 🧾 Author
**Ekaterina Luoto**  
Prompt Engineer / AI Developer  
📍 Saint Petersburg, Russia

