Here’s a version that renders correctly on GitHub:

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
