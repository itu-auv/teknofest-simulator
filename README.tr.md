# Teknofest Sualtı Yarışması Simülatörü
View this file in [English](README.md).

`teknofest_simulator`, `uuv_simulator` üzerinde Teknofest 2021 Uluslararası Sualtı Yarışması için geliştirilmiş bir simülasyon ortamıdır.

## Dependencies
- `uuv_simulator`
  ```sh
  sudo apt install ros-melodic-uuv-simulator
  ```

## Kurulum & Derleme
```sh
# Workspace klasörü oluşturulur
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
git clone git@github.com:itu-auv/teknofest-simulator.git
cd ~/catkin_ws

# Paket derlenir
catkin build -- teknofest_simulator
```

## Çalıştırma
Simülasyon ortamı aşağıdaki komut ile çalıştırılabilir.
```sh
roslaunch teknofest_simulator start.launch
```

## Lisans
Detay için [LICENSE](LICENSE).

## Yazar
Sencer Yazıcı - [senceryazici@gmail.com](mailto:senceryazici@gmail.com)