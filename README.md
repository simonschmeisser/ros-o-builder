```bash
echo "deb [trusted=yes] https://raw.githubusercontent.com/v4hn/ros-o-builder/jammy-one-overlay// ./" | sudo tee /etc/apt/sources.list.d/v4hn_ros-o-builder-jammy-one-overlay.list
sudo apt update
sudo apt install python3-rosdep2
echo "yaml https://raw.githubusercontent.com/v4hn/ros-o-builder/jammy-one-overlay//local.yaml debian" | sudo tee /etc/ros/rosdep/sources.list.d/1-v4hn_ros-o-builder-jammy-one-overlay.list
rosdep update
```
