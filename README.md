# Emotion-detection-in-Tweets

## Installation
```
pip install -r requirements.txt
```

## Running the program
Make sure that the dataset and the python notebook are in the same folder. No external commannds are required to run the program. If using colab make sure you are using GPU, otherwise add "use_cuda=False" in the block where BERT is implemented or replace the intialization of the model with the line given below.

```
model = MultiLabelClassificationModel('bert', 'bert-base-uncased', num_labels=11,use_cuda=False, args={'reprocess_input_data': True, 'overwrite_output_dir': True, 'num_train_epochs': 1})
```
