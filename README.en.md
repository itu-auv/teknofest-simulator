# Teknofest Simulator
Bu dosyayı Türkçe görüntüleyin [Turkish](README.md).

`teknofest_simulator` is a simulator environment for Teknofest 2021 Underwater Competition based on `uuv_simulator`.

## Dependencies
- `uuv_simulator`
  ```sh
  sudo apt install ros-melodic-uuv-simulator
  ```

## Install & Building
```sh
# Create workspace if you haven't already.
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
git clone git@github.com:itu-auv/teknofest-simulator.git
cd ~/catkin_ws

# Build the package
catkin build -- teknofest_simulator
```

## Running
The simulator environment can be started with
```sh
roslaunch teknofest_simulator start.launch
```


## License
See [LICENSE](LICENSE)

## Author
Sencer Yazıcı - [senceryazici@gmail.com](mailto:senceryazici@gmail.com)