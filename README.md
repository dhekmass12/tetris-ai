# tetris-ai

A bot that plays [Tetris](https://en.wikipedia.org/wiki/Tetris) using deep reinforcement learning.

## Demo

First 10000 points, after some training.
![Demo - First 10000 points](./demo.gif)

## Requirements

1. 
```shell
conda env create -f environment.yml
```
2. 
```shell
conda activate tetris-ai
```
3. You are good to go :)

## Run

- Train/execute:
```shell
# hyper parameters can be changed in the run.py script
python3 run.py
```

- View logs with `tensorboard`:
```shell
tensorboard --logdir ./logs
```

- Play a game with an existing model (`sample.keras` is a previously trained model that achieved more than 800k points, using 3 Relu layers with 32 neurons each):
```shell
python3 run_model.py sample.keras
```