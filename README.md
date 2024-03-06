The "Stable Bud" project aims to develop a machine learning application for accurately counting the repetitions performed by individuals during deadlift exercises. Leveraging computer vision techniques and the Stable Diffusion model, this project offers a sophisticated solution to track and analyze deadlift movements in real time.

Technical Details:

Graphical User Interface (GUI):

The application utilizes the Tkinter library for creating a GUI.

Components include an entry field for user input, a button for triggering image generation, and a label for displaying the generated images.

Model Initialization:

The application initializes the Stable Diffusion Pipeline using the StableDiffusionPipeline.from_pretrained() method.

The modelid parameter specifies the pre-trained model to be used, which is "CompVis/stable-diffusion-v1-4".

The device parameter indicates the hardware accelerator to be used, with "cuda" referring to NVIDIA GPU acceleration.

The auth_token is used for authentication purposes.

Image Generation:
User inputs are processed through the Stable Diffusion Pipeline to generate corresponding images.
The generate() function processes the input text from the entry field and generates images based on the Stable Diffusion model.
The generated images are displayed in the GUI window using PIL (Python Imaging Library) and ImageTk modules.

Autocasting:
Autocasting is utilized within the generate() function to automatically cast data to the appropriate data type for GPU acceleration.
Output and Interaction:
The generated images are saved as "generatedimage.png" and displayed in the GUI window.
Users can interact with the application by inputting text and clicking the "Generate" button to initiate image generation and display.


The "Stable Bud" project showcases the integration of machine learning models, particularly the Stable Diffusion model, into a user-friendly application for analyzing deadlift movements. By leveraging computer vision and deep learning techniques, this project offers a novel approach to accurately count repetitions during deadlift exercises, catering to fitness enthusiasts and professionals alike.

