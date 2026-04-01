

The pipeline executes a large-scale multimodal architecture for crisis response.

Requirements
Python 3.9+
CUDA-enabled GPU (16GB+ VRAM recommended)
Dependencies: torch, torchvision, transformers, pandas, scikit-learn, pillow, tqdm, accelerate
📁 Dataset Setup
Download CrisisMMD v2.0.
Update BASE_DIR in the script to your local path.
Ensure your TSV splits include tweet_text and LLaVA_text for multimodal input.
🧪 Key Features
Efficient Tuning: Uses LoRA (Low-Rank Adaptation) to train models with minimal VRAM.
Advanced Fusion: Implements Canonical Correlation Analysis (CCA), Gated Cross-Modal attention, and Bidirectional Cross-Attention.
Imbalance Handling: Utilizes Focal Loss and Class-Weighted Cross-Entropy for skewed disaster data.
Robustness: 5-seed statistical validation with automated hyperparameter search.
Execution
Bash

python Crisis-FusioLIP_main.py





Expected Directory Structure
CrisisMMD_v2.0/
- crisismmd_datasplit_with_LLaVA_generated_text/
  - task_informative_text_img_train.tsv
  - task_informative_text_img_dev.tsv
  - task_informative_text_img_test.tsv
  - task_humanitarian_text_img_train.tsv
  - task_humanitarian_text_img_dev.tsv
  - task_humanitarian_text_img_test.tsv
  - task_damage_text_img_train.tsv
  - task_damage_text_img_dev.tsv
  - task_damage_text_img_test.tsv
- <image_folders>/  
  - *.jpg / *.png   (images referenced in TSV files)
- experiment_results/  
  - results_YYYYMMDD_HHMMSS.csv
  - results_YYYYMMDD_HHMMSS_summary.csv
