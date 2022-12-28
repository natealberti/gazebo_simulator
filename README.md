# gazebo_simulator
![gazebo image](https://gazebosim.org/assets/images/gazebo_horz_pos_topbar.svg)
## Step 1
[Install gazebo classic](https://classic.gazebosim.org/tutorials?tut=install_ubuntu#Defaultinstallation:one-liner)
```
curl -sSL http://get.gazebosim.org | sh`
```

## Step 2
Clone repository using [git](https://kbroman.org/github_tutorial/pages/first_time.html) 
```
cd ~/Documents
git clone https://github.com/DevilFishRobotics/gazebo_simulator.git
```

## Step 3 
Open the `.bashrc` file.
```
sudo nano ~/.bashrc
```
Add the `gazebo_models` folder to your `.bashrc` file.
```
#custom gazebo models for gazebo to access
export GAZEBO_MODEL_PATH=~/Documents/gazebo_simulator/gazebo_models
```
**SAVE FILE & RESTART OS**

## Step 4 
Run the program with debugging info
```
gazebo -u Documents/gazebo_simulator/NURC_v0.world --verbose
```
