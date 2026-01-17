Interactive Fashion Advisor with Virtual Try-On

LLM-powered Conversational Recommendation & Diffusion-based Virtual Try-On

📌 Overview

This project implements an Interactive Fashion Advisor that combines a
Large Language Model–based Conversational Recommendation System (CRS) with a
diffusion-based Virtual Try-On (VTO) module.

The system allows users to:

Interact with an AI assistant through multi-turn natural language dialogue

Receive personalized fashion recommendations

Visually try on recommended garments using virtual try-on technology

The project was developed as a capstone project and focuses on practical applications of LLMs, Computer Vision, and Generative AI.

🧠 System Architecture

The system consists of three main components:

Conversational Recommendation System (CRS)

Handles user dialogue and preference understanding

Uses a fine-tuned Large Language Model for multi-turn conversations

Retrieval Module

Retrieves relevant fashion items based on user intent

Uses FAISS for efficient similarity search

Virtual Try-On Module

Visualizes recommended outfits on user images

Built using diffusion-based models and vision-language representations

🛠️ Technologies

Programming & Frameworks: Python, PyTorch

Large Language Models: Qwen 2.5 3B (fine-tuned), GPT-4o mini

Retrieval: FAISS

Virtual Try-On: CatVTON (diffusion-based model)

Computer Vision:

SegFormer (garment segmentation)

CLIP / BLIP (vision–language representation)

Others: NLP, Computer Vision, Diffusion Models, Generative AI

⚙️ Configuration Notes

Before running the project, please note the following:

Replace API tokens in the following files:

retrieval_service/test_vto_space.py (around line 17)

retrieval_service/vto_service.py (around line 27)

FAISS index file:

Download products.faiss

Place it inside the index_retrieval/ directory

Please contact the author to obtain this file

▶️ How to Run
Step 1: Install dependencies
pip install -r requirements.txt

Step 2: Activate virtual environment

PowerShell (Cursor):

.\.venv\Scripts\Activate.ps1


VS Code:

venv\Scripts\Activate

Step 3: Start the application
pnpm dev
