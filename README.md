# spam-comment-detection-project
 AI-based spam detection for social media comments
Instagram & Social Media Spam Detector using ALBERT
An end-to-end Natural Language Processing (NLP) project that identifies and filters out automated spam comments from social media platforms using advanced Deep Learning transformer architectures.

## 🚀 Project Overview
Social media platforms are flooded with automated bots promoting scams, knockoff brands, and engagement bait. While traditional keyword filtering methods fail to understand the nuance of human text,
this project implements a state-of-the-art **ALBERT (A Lite BERT)** model to capture sentence context and structure, achieving near-perfect detection rates.

## 📊 Performance Comparison
We built a lightweight traditional baseline model and compared it directly against our fine-tuned Deep Learning transformer model using the **YouTube Spam Collection Dataset**:
| Model Architecture | Approach Type | Accuracy | Key Advantage |
| :--- | :--- | :--- | :--- |
| **Cosine Similarity** | Keyword / TF-IDF Vectorization | **86.21%** | Fast, lightweight, zero training time. |
| **ALBERT (A Lite BERT)** | Contextual Transformer Network | **98.98%** | Understands sentence intent, sarcasm, and context. |

## 🛠️ Tech Stack & Tools
* **Language:** Python 3.x
* **Environment:** Kaggle Notebooks (GPU T4 Accelerated)
* **Core Libraries:** Hugging Face (`transformers`, `datasets`), PyTorch, Scikit-Learn, Pandas, NumPy

## 📈 Key Insights
Traditional distance-based matching algorithms struggle with polysemy (words with multiple meanings).
For example, a baseline model might flag a legitimate comment like *"I clicked the link to your video and loved it!"* as spam simply because it contains the word "link". ALBERT successfully analyzes the surrounding context, eliminating false positives while catching sophisticated bots.
