# Aditya Kumar's Portfolio

Welcome to my personal portfolio! I'm Aditya Kumar, a Lead ML Engineer with over 6 years of experience in machine learning, deep learning, and AI systems. This GitHub Pages site (adi-iitd.github.io) showcases my professional journey, projects, publications, and more.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/adi-iitd/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=flat&logo=github)](https://github.com/adi-iitd)
[![Medium](https://img.shields.io/badge/Medium-Read-brightgreen?style=flat&logo=medium)](https://medium.com/@adi.gupta)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=flat&logo=gmail)](mailto:adi.ee1iitd@gmail.com)

## About Me

Aditya is a Machine Learning Engineer with over 6 years of experience designing and deploying scalable ML systems across diverse domains — including Classical Machine Learning (e.g., Linear and Logistic Regression, SVMs, XGBoost), Deep Learning, NLP, Reinforcement Learning, Computer Vision, and Recommendation Systems. He is proficient in frameworks like PyTorch, PyTorch Lightning, vLLM, LangChain, Keras, and FastAPI, enabling seamless end-to-end ML development and deployment.

At Posha, a food robotics startup, Aditya leads the full-stack ML pipeline — spanning data collection, foundational model development, and deployment on both cloud and edge devices. His work powers robotic cooking through intelligent perception and adaptive control, while also enabling a rich user experience via personalized recipe generation and multilingual search tailored for diverse communities.

Previously, he worked as an Applied Scientist II at Flipkart, where he built a Competitive Intelligence Platform (CIP) from the ground up to ingest large-scale social media data and perform targeted sentiment analysis for product and brand monitoring. It was adopted by CXOs to track Flipkart’s market positioning and sentiment dynamics on a weekly basis. He began his career as a MLE at Samsung Research, where he contributed to hand gesture recognition systems for human-computer interaction in AR/VR environments.

Aditya graduated in 2019 with a Bachelor's degree in Electrical Engineering from the Indian Institute of Technology Delhi (IIT Delhi).

## Education

- **Indian Institute of Technology Delhi (IIT Delhi)**  
  B.Tech in Electrical Engineering (2015 – 2019)

![IIT Delhi Logo](assets/iitd_logo.png)

## Experience

### Lead AI Engineer @ Posha (Oct 2023 – Present)
- **Search and Recommendation System**: Built a hybrid search engine combining BM25 with domain-specific semantic embeddings (GIST-Embedding) to support 700+ daily queries across 1,000 recipes and 200 ingredients. Trained multilingual models using LLM-augmented synthetic data to resolve fuzzy queries and enable Hindi-English code-mixed retrieval. Deployed FAISS-based retrieval optimized for sub-100ms latency. Achieved a 30% gain in NDCG@5, a 20% lift in recipe conversions, and 70% success on previously unsupported queries.
- **Universal Frying Model (UFM)**: Fine-tuned a Swin Transformer-based doneness predictor for real-time frying, leveraging visual cues to eliminate fixed-timer failures. Generated training data using bucketed doneness intervals and area-weighted label mixing. Achieved 0.025 MAE with ~30ms cloud latency, enabling consistent, adaptive cooking across varied ingredients, preparation styles, and lighting conditions.
- **Food Segmentation & Dispense Localization**: Fine-tuned a SegFormer-based real-time segmentation system for pan, food, robotic arms, and background in cluttered kitchen environments, achieving 97% mIoU. Integrated a dispense-localization module to isolate newly added ingredients with 90% IoU, and improved ingredient classification by applying a Swin Transformer to localized regions, reaching 82% F1 score.
- **Vision-Based Quality Auditors**: Adapted YOLOv8-based image quality validators to detect blur (steam, oil/gravy splatter), glare, human obstructions, and occlusions from external utensils, achieving 99% F1. Enabled automated cooking pause & recovery. Integrated splatter detection (to prevent wall contamination) and lump identification (for food safety) using SegFormer, improving recipe reliability under messy, real-world conditions.
- **Recipe Customisation**: Designed a recipe customization pipeline that adapts user-specified ingredient edits into instruction-level rewrites, grounded in device constraints and a knowledge base of machine, ingredient, and recipe semantics. Curated high-quality data using LLM-as-a-judge and DeepSeek-R1 with human-in-the-loop validation, and fine-tuned a Qwen-3 model in two stages (SFT + GRPO) to enable structured, traceable outputs and self-reflective reasoning, allowing the model to think through adaptations autonomously.

### Applied Scientist II @ Flipkart (Jan 2020 - Sep 2023)
- **Competitive Intelligence Platform (CIP)**: Built an NLP-driven analytics system to track Flipkart’s brand performance across five major social platforms by ingesting organization-level feedback and tagging it by sentiment, business unit, and aspect for marketplace-level benchmarking. Partnered with business teams to define high-level (L1) aspects (e.g., Delivery, Cancellation), and applied topic modeling with few-shot learning to discover granular L2 sub-aspects (e.g., delivery SLA). These insights powered CXO dashboards with VoC (Voice of Customer) metrics, enabling weekly Net Promoter Score (NPS) forecasts with ~1% MAPE and business unit–level market share predictions across 8 verticals with 1.5% MAE using regression ensembles.
- **FashionAI (Generative Design)**: Fine-tuned a diffusion model with full attribute control for high-fidelity fashion generation tailored to seller needs. Used Masked Textual Inversion to learn isolated attribute embeddings by masking irrelevant regions, outperforming DreamBooth and improving over baseline 'stability-ai' Stable Diffusion by 50%. Enabled precise attribute-conditioned synthesis with reliable generalization up to 4 attribute combinations, unlocking guided design and generative catalog monetization.

### Engineer I @ Samsung Research Institute (Jun 2019 - Dec 2019)
- **Gesture Recognition**: Developed a sensor-free hand gesture recognition system for Latin characters and emojis, enabling real-time interaction in AR/VR environments. Achieved 98% IoU for hand segmentation using a MobileNet + DenseASPP architecture with curriculum learning, and 90% classification accuracy with a DenseNet-based gesture recognizer.
- **Photorealistic Image Compositing**: Trained a CNN in an unsupervised setting to model human perception of realism and filter out low-quality composites. Built a synthetic dataset by pasting segmented COCO objects onto random backgrounds using instance masks, with learnable color transfer for visual coherence. Trained a Conditional GAN (Pix2Pix) to generate realistic composites conditioned on background and target object pairs.

### Undergraduate Researcher @ Biomedical Imaging Lab, IIT Delhi (Aug 2018 - May 2019)
- **Liver & Lesion Segmentation (LiTS)**: Collaborated with Medanta Hospital to automate liver and lesion segmentation from abdominal CT volumes using H-DenseUNet (3D-CNN), achieving Dice scores of 0.96 for liver and 0.85 for lesions. Enhanced patient-level classification across Healthy, Cirrhosis, and HCC categories by 20% by integrating radiologist-supervised handcrafted features with SVM-based analysis.

## Publications

1. **Data adaptive compressed sensing using deep neural network for image recognition**  
   R. Gupta, A. Kumar, S. Chaudhury, B. Lall, and V. Kaushik  
   IEEE: 2020 National Conference on Communications, 2020  
   This paper proposes a privacy-preserving, data-adaptive compressive sensing framework for image recognition, enabling inference directly from compressed measurements without reconstructing full images. It replaces block-based random sampling with a learned, global-context-aware encoder that focuses on semantically informative regions. The approach reduces data by ~50% while preserving recognition accuracy, and eliminates the need to store or transmit raw visual data. Its strong generalization across large-scale datasets makes it well-suited for privacy-sensitive applications like elderly fall detection.

2. **Deriving Customer Experience Implicitly from Social Media Data**  
   A. Kumar, S. Gupta, A. Sahu, and M. Kant  
   ACM Web Conference, 2022  
   This work presents a system for implicitly estimating customer experience from social media mentions across platforms such as Twitter, Instagram, LinkedIn, and Facebook. Using advanced NLP techniques, it tags feedback by marketplace, aspect, and sentiment to surface actionable pain points. The platform enables CXOs to track market share, detect emerging trends, and benchmark against competitors in real time, while accurately predicting NPS to drive proactive, data-informed brand strategy.

3. **SMT5: Leveraging Social Media and T5 to Understand Online Shopping Experience**  
   A. Kumar  
   Flipkart Data Science Conference, 2022  
   This paper introduces a multi-stage deep learning pipeline for extracting actionable Voice of Customer (VoC) insights from social media posts in English, Hindi, and Hinglish. Leveraging real-time, large-scale feedback from platforms like Twitter and Instagram, it addresses the limitations of traditional surveys by identifying customer pain points and product-specific experiences across various journey stages. The approach provides organizations with a scalable, cost-effective solution for understanding and enhancing customer satisfaction.

## Projects

### 🔍 Search and Recommendation System (Posha)
Hybrid search engine and Recommendation System with semantic understanding  
- Users frequently entered misspelled recipe names, fuzzy spellings, Hindi-English code-mixed text, or vague descriptions—challenges amplified by the diversity of the user base. Traditional keyword search (BM25) failed to handle such noise effectively. To address this, deployed a hybrid search engine combining BM25 for exact matches with a fine-tuned **GIST-Embedding** model for semantic similarity. The system handled **700–800 daily queries** across **~1,000 recipes** and **~200 ingredients**, bridging the gap between precise matching and contextual understanding to improve discoverability for both structured filters and free-form queries.
- Adapted a pre-trained **GIST-Embedding** model for two distinct tasks: (1) a **query correction** model trained using synthetic data generated via LLM-based augmentation and NLP techniques (e.g., character swaps, Levenshtein ≤**3**) to handle fuzzy spellings and Hindi-English code-mixed queries, and (2) a **semantic retrieval** model adapted using domain-specific Q/A pairs with hard negatives from related recipes to improve fine-grained semantic separation.
- Built a **4-stage** search pipeline: (1) corrected each query token by matching it to its closest token in a binary-quantized embedding space using the query correction model, (2) expanded non-English tokens with language-specific synonyms, (3) retrieved **~100** candidates from the binary embedding space, and (4) re-ranked results using the full-precision semantic embedding model and business logic. FAISS-powered retrieval and re-ranking kept end-to-end latency under **90ms**. Improved search performance across key metrics: NDCG@5 lifted by **30%**, recipe-to-click conversion rate increased by **20%**, and fuzzy/transliterated query success rose to **70%** from a **0%** baseline.
- Built a personalized recipe recommender using semantic embeddings with hybrid filtering that combined user preferences, dietary tags, and past cooking history with collaborative signals. Solved the cold-start problem by introducing an onboarding flow where users specify allergens, cooking habits, and select **3+** preferred recipes—similar to recommendation flows used by Netflix and Spotify.

### 🍲 Universal Frying Model (UFM) (Posha)
Regression model for real-time doneness prediction  
- Replaced fixed frying timers in robotic cooking systems with a Swin Transformer-based regression model that predicts ingredient doneness on a continuous 0–1 scale using real-time visual cues. This dynamic control eliminates under- and overcooking errors, delivering consistent results across diverse ingredients and preparation styles.
- Addressed limited labeled data by collecting bucketed doneness annotations in the 0–0.75 range for individual ingredients under varied lighting conditions (dark, ambient, and bright). Each ingredient was cooked in isolation, and its region was localized using a food segmentation model to capture precise per-ingredient doneness masks. During training, synthetic multi-ingredient scenes were generated by blending up to 3 segmented ingredients into one frame. Labels were computed via area-weighted averaging of individual doneness scores, constrained to adjacent label buckets to preserve semantic consistency in the regression target space. This augmentation strategy substantially diversified and expanded the dataset.
- Exported the model to ONNX and deployed a CPU-optimized inference pipeline that processes raw camera frames every 10 seconds without preprocessing. Achieved low-latency inference with ~30ms on cloud and ~80ms on edge devices, generalizing well across lighting and ingredient variations with a validation MAE of 0.025.

### 🥘 Food and Ingredient Segmentation with Dispense Localization (Posha)
Real-time SegFormer pipeline for ingredient detection and classification  
- **Food Segmentation**: Annotated 1,500 real-world images captured under occlusion, glare, and low-light conditions in cluttered kitchen environments to train a SegFormer model for segmenting pan, food, robotic arms (fixed and rotating), and background. To scale the dataset, generated pseudo-labels on ~10,000 unlabeled frames using the trained model and selected 2,000 high-confidence samples (≥95% confidence) for self-distillation. Fine-tuned the model for a few additional epochs using both annotated and pseudo-labeled data, achieving 97% mean IoU—a +1% improvement from distillation. The final model supports multiple downstream tasks, such as detecting pan state transitions for dynamic control in liquid-heavy recipes (e.g., cooking gravy, frying onion purée). Deployed via ONNX for CPU inference with 120ms latency on edge device and 70ms on cloud.
- **Ingredient Localization and Classification**: Developed a pipeline to detect and classify newly dispensed ingredients after each macro-dispense instruction (up to 4 times per session). Used a SegFormer model for localization, achieving 90% IoU with a +3.5% gain from self-distillation. Cropped the localized regions and classified them using a Swin Transformer, reaching 85% accuracy and 82% F1 score—significantly outperforming full-pan classification (<50% accuracy). This system enables automated recipe debugging by comparing user-executed recipes with ground-truth references to identify ingredient mismatches and compute step-level similarity scores. Deployed end-to-end via ONNX on CPU with 200ms per-frame latency.

### 🕵 Vision-Based Quality Auditors for Robotic Cooking (Posha)
YOLOv8 and SegFormer for automated quality control  
- **Image Auditor**: Vision failures caused by blur, poor lighting, or occlusions can derail automated cooking. To preempt such failures, fine-tuned a YOLOv8 model to serve as a real-time image quality auditor using 5,000 hand-annotated frames. Achieved 92.5% IoU at the bounding box level and 99.2% F1 score in binary classification (good vs. bad frames). The system pauses recipe execution after 5 consecutive bad frames and prompts users to clean the camera, preventing downstream vision breakdowns. Deployed via ONNX on CPU with ~50ms latency on edge and ~70ms on cloud.
- **Splatter Detector**: Oil and gravy splatter during cooking—especially in gravy-rich recipes—can contaminate the robot's surroundings and nearby walls. To address this, fine-tuned a SegFormer model on 500 annotated frames, achieving 69.8% IoU. After each macro-dispense, the system resets its baseline using the previous frame to account for food falling on the main arm during dispensing. If splatter exceeds 2% of the image area relative to the baseline, stirrer speed is increased to 90% to minimize residue buildup and prevent cross-contamination. Deployed via ONNX on CPU with ~120ms latency on edge and ~70ms on cloud.
- **Lump Detector**: Undissolved lumps in meat or noodle dishes can affect health. To ensure a consistent and safe meal, implemented lump detection using a SegFormer model trained on end-of-session frames. Achieved 69.8% IoU for meat and 88% IoU for noodles. If lump area exceeds 2% of the frame, the system adds 100ml water and re-stirs for noodles, and 50ml water and re-stirs for meat. Deployed via ONNX on CPU with ~100ms latency on edge and ~60ms on cloud.

###  The user wants a nice README.md for their GitHub pages site: adi-iitd.github.io. The content is from the provided DOCUMENT, which is Aditya Kumar's portfolio or resume in HTML format, but extracted as text.

First, understand what a README.md for GitHub Pages should include. Typically, for a personal site, it might include:

- Introduction to the site/person.

- How to set up or run the site locally.

- Technologies used.

- Contact info.

- Maybe a screenshot or link to the live site.

Since it's GitHub Pages, the README should describe the repository, which hosts the personal website.

The site seems to be a personal portfolio showcasing experience, education, projects, etc.

To make it "nice", use Markdown formatting: headers, lists, badges if applicable, emojis, etc.

Structure:

1. **Header**: Name and brief bio.

2. **About**: More detailed about the person.

3. **Live Site**: Link to the GitHub Pages site.

4. **Setup**: How to run locally.

5. **Technologies**: HTML, CSS, JS.

6. **Contact**: Links from the document.

The current date is July 28, 2025, but not sure if relevant.

Tools are available, but for writing a README, I might not need them unless verifying something.

The question is to write a README.md based on the document.

I need to generate the Markdown content.

Key sections from document:

- Bio

- Education

- Experience with details

- Publications

- Projects

- Patents

- Interests

In README, summarize or link to the site, don't duplicate everything.

Since it's for the repo hosting the site, README can be a overview.

Make it engaging.# Aditya Kumar's Portfolio

[![GitHub](https://img.shields.io/github/license/adi-iitd/adi-iitd.github.io?style=flat-square)](https://github.com/adi-iitd/adi-iitd.github.io/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/adi-iitd/adi-iitd.github.io?style=flat-square)](https://github.com/adi-iitd/adi-iitd.github.io/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/adi-iitd/adi-iitd.github.io?style=flat-square)](https://github.com/adi-iitd/adi-iitd.github.io/network)

Welcome to my personal portfolio website hosted on GitHub Pages! This site showcases my professional journey as a Lead ML Engineer with over 6 years of experience in machine learning, deep learning, and AI applications across domains like NLP, Computer Vision, Reinforcement Learning, and Recommendation Systems.

[🌐 Visit the Live Site](https://adi-iitd.github.io)

## 👨‍💻 About Me

I'm Aditya Kumar, a Machine Learning Engineer specializing in scalable ML systems. Proficient in frameworks like PyTorch, PyTorch Lightning, vLLM, LangChain, Keras, and FastAPI, I focus on end-to-end ML development and deployment.

- **Current Role**: Lead ML Engineer at [Posha](https://posha.com), a food robotics startup, where I lead the full-stack ML pipeline for robotic cooking, perception, and user personalization.
- **Previous Roles**:
  - Applied Scientist II at Flipkart (2020–2023): Built the Competitive Intelligence Platform (CIP) for social media sentiment analysis and market benchmarking.
  - Engineer I at Samsung Research Institute (2019): Developed hand gesture recognition for AR/VR.
  - Undergraduate Researcher at IIT Delhi (2018–2019): Worked on biomedical imaging for liver lesion segmentation.
- **Education**: B.Tech in Electrical Engineering from Indian Institute of Technology Delhi (IIT Delhi), 2015–2019.
- **Interests**: Coding impactful solutions, writing tech blogs, and playing cricket, table-tennis, and golf!

For more details on my experience, projects, publications, and patents, check out the [live site](https://adi-iitd.github.io).

## 📂 Repository Overview

This repository contains the source code for my personal portfolio website built with HTML, CSS, and JavaScript. It's deployed automatically via GitHub Pages.

### Key Features
- **Responsive Design**: Adapts to all screen sizes, from mobile to desktop.
- **Sections**: About, Education, Experience, Publications, Projects, Patents, and Interests.
- **Interactive Elements**: Tabbed navigation for projects and patents.
- **Assets**: Images and PDF CV included in the `assets/` folder.

## 🛠️ Setup and Local Development

To run the site locally:

1. **Clone the Repository**:
   ```
   git clone https://github.com/adi-iitd/adi-iitd.github.io.git
   cd adi-iitd.github.io
   ```

2. **Open the Site**:
   - Simply open `index.html` in your browser (no server needed for static site).
   - For a live server (optional, for hot-reloading):
     - Install a simple HTTP server if needed: `npm install -g http-server`
     - Run: `http-server .`
     - Visit: `http://localhost:8080`

3. **Dependencies**:
   - No build tools required; pure HTML/CSS/JS.
   - Uses Font Awesome via CDN for icons.

## 🚀 Deployment

This site is deployed on GitHub Pages. To deploy your own fork:
- Go to repository Settings > Pages.
- Set Source to `main` branch and root directory.
- Your site will be live at `https://<username>.github.io`.

## 📫 Contact

- **Email**: [adi.ee1iitd@gmail.com](mailto:adi.ee1iitd@gmail.com)
- **Phone**: +91 9818495273
- **GitHub**: [adi-iitd](https://github.com/adi-iitd)
- **LinkedIn**: [adi-iitd](https://www.linkedin.com/in/adi-iitd/)
- **Medium**: [@adi.gupta](https://medium.com/@adi.gupta)

Feel free to reach out for collaborations, discussions, or just to connect!

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Thanks for visiting! ⭐ If you find this useful, star the repo!
