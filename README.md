# Deep RL Approach to Adaptive Traffic Lights Management
A framework where a deep Q-Learning Reinforcement Learning agent tries to choose the correct traffic light phase at a multi-intersection map to maximize traffic efficiency.

This project is supported by: https://github.com/stuti2403/Traffic-Light-Management-system-using-RL-and-SUMO.git


## Prepare the environment: 
All main packages are included ```requirements.txt```.
```bash
pip install -r requirements.txt
```

## Train command:
```bash
python train.py --train -e 50 -m model_name -s 2000
```

When the training process ends, a file named ```model_name.bin``` will be stored in ```models```.


## Test comand:
```bash
python train.py -m model_name -s 2000
```

When the tesing process ends, a chart and a text file that store waiting time per step will be saved in a folder ```model_name``` which is a subfolder of ```plots_testing```.

## Argument explainations:
- **train**: enable training process if set to *True* otherwise testing mode is enabled (default is False).  
- **e**: the number of epoch for training process (default is 50).
- **m**: name the new model if train or else indicate the model to test.
- **s**: the number of steps in simulation.