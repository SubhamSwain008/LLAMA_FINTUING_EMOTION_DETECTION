😢 Emotion-Aware Training (Text Classification)
Instead of using off-the-shelf sentiment tools, I fine-tuned LLaMA 3.2 (1B) on a curated dataset of emotional dialogues and annotated text. The goal wasn’t just sentiment polarity (positive/negative) but nuanced categories like anger, joy, sadness, fear, disgust, surprise, and neutral.

🧠 Core Model (LLM Backbone)
LLaMA 3.2 serves as the backbone. Its compact 1B parameter size makes it lightweight and efficient for deployment, while fine-tuning aligns it with the task of recognizing subtle emotional cues in sentences. This ensures the model captures both explicit expressions (“I am furious”) and implicit signals (“I can’t believe this happened again”).

📊 Data Engineering (Emotion Annotations)
The dataset was engineered to balance real-world dialogues, social media text, and scripted conversations. Each text segment was paired with emotion tags. Heavy preprocessing—like removing noise, normalizing slang, and handling code-switching (English + Hindi)—was done to make the model robust in real applications.

⚡ Pipeline Integration
Training loop: Hugging Face transformers + PEFT/LoRA for efficient fine-tuning.


🚀 End Goal
This wasn’t just about detecting “positive vs. negative,” but about teaching an open-source LLM to understand human emotions in text—a key step toward emotionally intelligent conversational agents.
