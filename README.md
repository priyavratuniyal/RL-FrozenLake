# RL-FrozenLake
For the purpose of making this project platform agnostic, I have used docker.
Also, I wanted to use pyvirtualdisplay with xvfb, so I had to use the jupyter notebook image with a Linux based container, because it's not available in Windows.

So here are the steps to set-up the container:
- Going inside the jupyter-docker directory => running 'docker-compose up'

Feel free to change the docker files according to your needs.

P.S. It took around 8 mins, on my machine to setup the whole jupyter lab, so please be patient with the spin-up.
