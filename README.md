# Improved Social LSTM implementation in PyTorch
 
## Documentation
- **generator.py** : Python script for generating artifical datasets
- **helper.py**: Python script includes various helper methods
- **hyperparameter.py**: Pyton script for random best parameter selection for a model
- **make_directories.sh**: Bash script for creation of file structure
- **model.py**: Python file includes Improved Social LSTM model definition
- **slstm_model.py**: Python file includes Social LSTM model definition
- **olstm_model.py**: Python file includes Occupancy LSTM model definition
- **olstm_train.py**: Python script for training Occupancy LSTM model
- **test.py**: Python script for model testing and getting output txt file for submission
- **train.py**: Python script for training Improved Social LSTM model
- **slstm_train.py**: Python script for training Social LSTM model
- **utils.py**: Python script for handling input train/test/validation data and batching it
- **validation.py**: Python script for externally evaluate a trained model by getting validation error
- **visualize.py**: Python script for visualizing predicted trajectories during train/test/validation sessions
- **vlstm_model.py**: Python file includes Vanilla LSTM model definition
- **vlstm_train**: Python script for training Vanilla LSTM model

## How to deploy
1. Fork the repository 
2.  Start train a model >>> **python train/olstm_train/vlstm.train.py/slstm.train.py - -[Parameter set]**
3. If necesarry file structure is not exist (which is the initial situation), train script will run make_directories.sh and this command will automatically create file structure
4. Enjoy!

## Results  

| Model name | Avarage error | Final error | Mean error |
| :---: | :---: | :---: | :---: |
| Improved Social LSTM | 0.5094 | 1.7070 | 0.8693 |
| Social LSTM | 1.3865 | 2.098 | 0.675 |
| Occupancy LSTM | 2.1105 | 3.12 | 1.101 |
| Vanilla LSTM | 2.107 | 3.114 | 1.1 |

**Reference**: http://trajnet.stanford.edu/result.php?cid=1

