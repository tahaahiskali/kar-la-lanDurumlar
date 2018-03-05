Bu depo altında herhangi bir program,yazılım çalıştırma yükleme sırasında  karşılaşılan problemler ile ilgili çözümler yazılmıştır.

## Python3 opencv ROS hatası 

  **Hata 
  ImportError: /opt/ros/kinetic/lib/python2.7/dist-packages/cv2.so: undefined symbol: PyCObject_Type? )

## _Hatırlatma_ ##

Ros Kurulumu yapıldıktan sonra python2 sürümüne otomatik olarak opencv eklenmiş olacak fakat python3 için aynı durum söz konusu değil. 

 1) `sudo pip3 install opencv-python` komutu ile py3 için kurulum yapıldığı varsayılmıştır.
 2) **python3** komutu ile terminalde python3 arayüzüne geçtiğiniz zaman **import cv** komutunu çalıştırdığınızda **ImportError: /opt/ros/kinetic/lib/python2.7/dist-packages/cv2.so: undefined symbol: PyCObject_Type** hatası alıyorsanız bunun nedeni **/opt/ros/kinetic/setup.bash** bu bash dosyasının şuan aktif olmasıdır. Bu bash dosyası iki türlü aktif hale getirilmiş olabilir birincisi **source /opt/ros/kinetic/setup.bash** komutu ile yada **gedit /home/username/.bashrc** dosyasının en alt kısmında **source /opt/ros/kinetic/setup.bash** bu komutun bulunmasıdır. Çözüm yakında ..
  



