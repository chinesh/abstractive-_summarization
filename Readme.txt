Converting dataset into chunked files:
The dataset is converted into the bin files using the following github repository. https://github.com/abisee/cnn-dailymail

Command to train the model:
python run_summarization.py --mode=train --data_path=chunked/train_* --vocab_path=vocab --log_root=hello --exp_name=myexperiment

Command to get the results and save it in the Txt file:
python run_summarization.py --mode=decode --data_path=chunked/val_* --vocab_path=vocab --log_root=hello --exp_name=myexperiment

The results after 14 hours of training are saved in the output.txt.

