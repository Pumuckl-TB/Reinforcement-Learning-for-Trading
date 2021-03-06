# An Application of Deep Reinforcement Learning to Algorithmic Trading
This code is largely based on following research paper. 
> Thibaut Théate and Damien Ernst. "An Application of Deep Reinforcement Learning to Algorithmic Trading." (2020).
> [[arxiv]](https://arxiv.org/abs/2004.06627)
The link to their original github: https://github.com/ThibautTheate/An-Application-of-Deep-Reinforcement-Learning-to-Algorithmic-Trading

# Contributions
I used their model and added the Differential Downside Deviation Return Reward Function introduced by Moody and Saffell 2001 as an evaluation metric as well as the sharpe ratio. 

> Moody, J. and M. Saffell (2001). ‘Learning to trade via direct reinforcement’. In: IEEE Transactions
> on Neural Networks 12.4, pp. 875–889. doi: 10.1109/72.935097.

These are the two added evaluation metrics. 
Sharpe ratio:
![image](https://github.com/Pumuckl-TB/Reinforcement-Learning-for-Trading/blob/main/SR.png)

Differential Downside Deviation Return
![image](https://github.com/Pumuckl-TB/Reinforcement-Learning-for-Trading/blob/main/DDR1.png)
![image](https://github.com/Pumuckl-TB/Reinforcement-Learning-for-Trading/blob/main/DDR2.png)



# Dependencies

The dependencies are listed in the text file "requirements.txt":
* Python 3.7.4
* Pytorch 1.5.0
* Tensorboard
* Gym
* Numpy
* Pandas
* Matplotlib
* Scipy
* Seaborn
* Statsmodels
* Requests
* Pandas-datareader
* TQDM
* Tabulate




# Usage

Simulating (training and testing) a chosen supported algorithmic trading strategy on a chosen supported stock is performed by running the following command:

```bash
python main.py -strategy STRATEGY -stock STOCK
```

with:
* STRATEGY being the name of the trading strategy (by default TDQN),
* STOCK being the name of the stock (by default Apple).

The performance of this algorithmic trading policy will be automatically displayed in the terminal, and some graphs will be generated and stored in the folder named "Figures".



