# FactHunt: Retrieval-driven Fact Verification for Accurate Conclusions

### File Structure
- data: For Data Files
- outputs: Contains the log files of output
- src: Contains the code

### Data
Download data folder from [here](https://drive.google.com/drive/folders/1p5uxv90HmIwRM3A1GVX2FXik24eFP4jL?usp=drive_link).

### How to Run
- Prepare Data (Includes relevant row retrieval) \
`python prepare_data.py --selector contriever --parse_rows --parse_columns --output_path <path1>`

- Tokenise and pre-process for BERT \
`python tokenise_data.py --input_path <path1> --bert_model xlm-roberta-base`

- Train Model \
`python train_model.py --do_train --scan horizontal --bert_model xlm-roberta-base --input_save_dir <path1>`

### Authors
1. Nishant Gahlaut (19BT30015)
2. Shrinivas Khiste (19CS30043)
3. Ishan Goel (19CS30052)
4. Ankit katewa (19BT3AI05)
