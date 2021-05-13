# Teknofest Sualtı Yarışması Simülatörü
View this file in [English](README.en.md).

`teknofest_simulator`, `uuv_simulator` üzerinde Teknofest 2021 Uluslararası Sualtı Yarışması için geliştirilmiş bir simülasyon ortamıdır.

### Not
`uuv_simulator` ile oluşturmuş olduğunuz aracı spawn etmeniz gerekmektedir. Yakında [İTÜ AUV Takımı GitHub hesabında](https://github.com/itu-auv)
`uuv_simulator` ile sıfırdan araç oluşturma ile ilgili bir kılavuz yayınlayacağız. Bu kılavuz ile tasarladığınız aracı `uuv_simulator` ile 
simülasyon ortamına aktarabilecek, ve bu repository üzerinde paylaşılan yarışma ortamına `spawn` ederek kullanabileceksiniz, takipte kalın.
İletişim, soru, öneri ve simülasyon ortamına katkılarınız için [senceryazici@gmail.com](mailto:senceryazici@gmail.com).

## Dependencies
- [ROS Melodic](http://wiki.ros.org/melodic/Installation/Ubuntu)
  
  `Not: Ubuntu 18.04, ROS Melodic üzerinde test edilmiştir.`

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