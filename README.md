





Expected Directory Structure


/path/to/your/CrisisMMD_v2.0/
├── crisismmd_datasplit_with_LLaVA_generated_text/
│   ├── task_informative_text_img_train.tsv
│   ├── task_informative_text_img_dev.tsv
│   ├── task_informative_text_img_test.tsv
│   ├── task_humanitarian_text_img_train.tsv
│   ├── task_humanitarian_text_img_dev.tsv
│   ├── task_humanitarian_text_img_test.tsv
│   ├── task_damage_text_img_train.tsv
│   ├── task_damage_text_img_dev.tsv
│   └── task_damage_text_img_test.tsv
├── <image_folders>/  # Referenced by 'image' column in TSVs
│   └── *.jpg / *.png
└── experiment_results/  # Created automatically
    ├── results_20250101_120000.csv
    └── results_20250101_120000_summary.csv
