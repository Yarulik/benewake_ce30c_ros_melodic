# benewake_ce30c_ros_melodic
 
## Инструкция по запуску лидара на ROS Melodic
На других не тестировал, но на Raspbian Buster привер из CE30_sdk_test, работал

#### ROS Melodic уже должен быть установлен
#### в ~/.bashrc должно быть прописан localhost name и т.д.


#### Если при catkin_make выйдет ошибка драйвера:
/usr/bin/ld: skipping incompatible /home/nvidia/Загрузки/SDK/CE30-C_ROS/libbw_ce30v2.0.so when searching for -lbw_ce30v2.0
#### то нужно на откомпилировать этот файл, перейдя в директорию 
cd ~/benewake_ce30c_ros_melodic/benewake_ce30c_sdk_linux/sources и сделать make 
в catkin/src/benewake_c30c libbw_ce30v2.0.so заменяем на новый, теперь пробуем снова catlin_make


#### Возможно потребуется установить 
sensor_msgs, std_msgs и д.р., об этом сообщит компилятор
