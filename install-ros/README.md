# Playbook for installing Robot Operating System

See (http://ros.org)

## Installation

`ansible-playbook -i hosts install-ros.yml`

## Post-install steps

(Taken from (http://wiki.ros.org/indigo/Installation/Ubuntu))

- Ssh to the machine
- Execute the following commands

### Initialize rosdep

```
sudo rosdep init
rosdep update
```

### Environment setup

```
echo "source /opt/ros/indigo/setup.bash" >> ~/.bashrc
source ~/.bashrc
```