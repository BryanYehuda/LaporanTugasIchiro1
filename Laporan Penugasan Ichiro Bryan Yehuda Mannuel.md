
Nama : Bryan Yehuda Mannuel       
NRP : 05311940000021
Departemen : Teknologi Informasi (IT)       
Divisi : Programming

## Persiapan Sebelum Penugasan
1. Sudah mengikuti pelatihan _Linux_ di Departemen IT di ITS pada tanggal 3 November 2019
2. _ISO Linux Ubuntu 18.04_ sudah terdownload dari [_Linux Ubuntu_]([https://ubuntu.com/download/desktop](https://ubuntu.com/download/desktop))
3. _Rufus_ sudah terdownload dari [_Rufus_]([https://rufus.ie/](https://rufus.ie/))

## Tugas 1 : Install Linux Ubuntu
 
1. Melakukan Partisi pada Harddisk di _Windows_, untuk mengalokasikan storage sebesar 100GB untuk _Linux Ubuntu_ 
(**Selesai pada 7 November 2019, jam 21:23**)
2. Melakukan Format terhadap Flashdisk yang akan digunakan untuk booting _Linux Ubuntu_ 
(**Selesai pada 7 November 2019, jam 21:25**)
3. Melakukan Burning ISO Linux Ubuntu menggunakan Rufus 
(**Selesai pada 7 November 2019, jam 21:33**)
4. Melakukan Restart dalam Safe Mode menggunakan Windows (**Selesai pada 7 November 2019, jam 21:34**)
5. Melakukan Booting _Linux Ubuntu_ dengan bantuan Flashdisk yang sudah terburning _ISO Linux Ubuntu_ didalamnya 
(**Selesai pada 7 November 2019, jam 21:37**)
6. Melakukan Instalasi _Linux Ubuntu_ pada Partisi Hardisk yang sudah disediakan 
(**Selesai pada 7 November 2019, jam 22.00**)
7. Melakukan Update sistem _Linux Ubuntu_ menggunakan _Terminal_ dengan command : 
```
sudo apt update
``` 
(**Selesai pada 7 November 2019, jam 22.05**)  
  
8. Melakukan Upgrade sistem _Linux Ubuntu_ menggunakan _Terminal_ dengan command :
```
sudo apt-get upgrade
```
(**Selesai pada 7 November 2019, jam 22.35**) 
             
9. _OS Linux Ubuntu_ sudah selesai terinstall dan siap untuk digunakan lebih lanjut 
(**Selesai pada 7 November 2019, jam 22.35**)

## Tugas 2 : Install ROS Melodic Morenia
### Sumber : [ROS Wiki Tutorial](http://wiki.ros.org/ROS/Tutorials) dan [Packt](https://subscription.packtpub.com/book/hardware_and_creative/9781783987443/1/ch01lvl1sec11/installing-ros-on-desktop-systems)

1. Mengconfigure _Ubuntu Repositories_ agar memperbolehkan instalasi dari sumber-sumber _"restricted"_, _"universe"_, dan _"multiverse"_ 
(**Selesai pada 8 November 2019, jam 07.15**)        
2.  Melakukan Setup pada _Linux Ubuntu_ agar bisa menerima Software dari [ROS Melodic Morenia](packages.ros.org.) dengan menggunakan _Terminal_ dengan command :
```
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```
(**Selesai pada 8 November 2019, jam 07.17**)    
   
3. Melakukan Set Up Keys pada _Linux Ubuntu_ dengan command :
```
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```
(**Selesai pada 8 November 2019, jam 07.19**) 
      
4. Memastikan sistem _Linux Ubuntu_ sudah terupdate dengan command :
```
sudo apt update
```
(**Selesai pada 8 November 2019, jam 07.22**)  
      
5. Melakukan Instalasi _ROS Melodic Morenia_ dengan command :
```
sudo apt install ros-melodic-desktop-full
``` 
(**Selesai pada 8 November 2019, jam 09.15**)
         
6. Melakukan inisialisasi _rosdep_ agar sistem _ROS_ bisa dengan melakukan instalasi program-program yang dibutuhkan dan diperlukan untuk menjalankan beberapa komponen utama pada _ROS_ dengan command :
```
sudo rosdep init
rosdep update
```
(**Selesai pada 8 November 2019, jam 09.17**)  
       
7. Melakukan Set Up Environment _ROS_ dengan command :
```
echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
source ~/.bashrc
```
(**Selesai pada 8 November 2019, jam 09.19**)  
       
8. Melakukan instalasi program yang dibutuhkan oleh _ROS Melodic Morenia_ yaitu _python_ untuk ROS dengan command :
```
sudo apt install python-rosinstall python-rosinstall-generator python-wstool build-essential
```
(**Selesai pada 8 November 2019, jam 09.25**)      
  
9. Melakukan pengecekkan hasil instalasi _ROS Melodic Morenia_ dengan membuka _Terminal_ baru dan menggetikkan command :
```
roscore
rosrun turtlesim turtlesim_node
```
(**Selesai pada 8 November 2019, jam 09.29**)         
 
10. Dan, setelah dicek, ternyata hasil instalasi _ROS Melodic Morenia_ berhasil dan siap untuk digunakan
(**Selesai pada 8 November 2019, jam 09.30**)          
   
## Tugas 3 : Membuat Laporan Dalam Bentuk Markdown
1. Mempelajari Syntax Markdown dari [Markdown Tutorial]([https://www.markdowntutorial.com/](https://www.markdowntutorial.com/))
(**Selesai pada 8 November 2019, jam 20.00**)          
2. Mendownload Text Editor _Abricotine_ dari [Abricotine]([http://abricotine.brrd.fr/](http://abricotine.brrd.fr/))
(**Selesai pada 8 November 2019, jam 20.05**)          
3. Melakukan pengetikan laporan dalam bentuk _Markdown_ pada Text Editor _Abricotine_ bersumber dari catatan di _Notes_
(**Selesai pada 8 November 2019, jam 21.50**)          
4. Melakukan Update setiap kali ada aktivitas penugasan yang dikerjakan

## Tugas Bonus : Tutorial ROS Melodic Morenia
 
### Sumber : [ROS Wiki Tutorial](http://wiki.ros.org/ROS/Tutorials)

#### 1. Instalasi dan Konfigurasi _Environment ROS_
1. Melakukan Instalasi _ROS Melodic Morenia_ 
(**Selesai pada 8 November 2019, jam 09.30**)      
2. Memeriksa Source _ROS Package_ terinstall pada path apa dengan command :
 ```
 printenv | grep ROS
 ```
 Mengapa kita perlu memanage source dari instalasi _ROS_? Karena _ROS_ mengandalkan environment dari _Shell Linux_ untuk menggabungkan space yang dibutuhkan. Hal ini akan membuat nantinya bekerja dengan lebih dari satu _ROS Package_ menjadi lebih mudah untuk dilakukan
 (**Selesai pada 8 November 2019, jam 11.17**)     
    
 3. Memanage Source awal dari _ROS Package_ yang terinstall pada _Linux Ubuntu_ dengan command :
 ```
 source /opt/ros/melodic/setup.bash
 ```
 kita perlu menuliskan command ini setiap kita ingin mengakses _Command-command ROS_ setiap kita menyalakan _Shell Linux_ baru
  (**Selesai pada 8 November 2019, jam 11.18**)       
   
 4. Membuat _ROS Workspace_ di dalam direktori _catkin_ws/src_ dengan command :
 ```
 mkdir -p ~/catkin_ws/src
 cd ~/catkin_ws/
 catkin_make
 ``` 
 Code _catkin_make_ ini nantinya akan menghasilkan file _CMakeList.txt_ di dalam folder _src_
  (**Selesai pada 8 November 2019, jam 11.20**)         
  
 5. Sekarang jika melihat pada direktori _catkin_ws_ kita akan menemukan 2 folder yaitu _devel_ dan _build_. Di dalam folder _devel_ ada beberapa file _setup.*sh_. Dan kita perlu untuk melakukan sourcing terhadap file-file ini dengan menggunakan command :
 ```
 source devel/setup.bash
 ```
 agar workspace _catkin_ kita bisa teroverlay dengan baik di atas environment yang ada
 (**Selesai pada 8 November 2019, jam 11.22**)       
 
 6. Untuk memastikan workspace kita sudah teroverlay dengan baik, gunakan command : 
```
echo $ROS_PACKAGE_PATH /home/bryan/catkin_ws/src:/opt/ros/melodic/share
```
dan setelah dicek, ternyata workspace _catkin_ sudah berhasil dibuat dengan baik
(**Selesai pada 8 November 2019, jam 11.25**)       

#### 2. Cara menavigasi _filesystem ROS_ dengan _Command-command ROS_
1. Sebelum memulai tutorial ini, kita perlu mendownload file tutorial dengan command :
```
sudo apt-get install ros-melodic-ros-tutorials
```
(**Selesai pada 8 November 2019, jam 12.01**)         

2. Beberapa istilah dalam _ROS_ yang perlu diketahui:
   * Package : Organisasi kode dari Software _ROS_, tiap package bisa berisi libraries, executables, scripts, atau artifact lainnya
   * Manifest (seperti _package.xml_) : manifest adalah deskripsi dari package, berfungsi untuk mendefiniskan dependencies diantara package dan untuk menangkap informasi meta tentang package seperti version, mantainer, license, dll
3. Command `rospack` bisa kita gunakan untuk mencari informasi tentang package
4. Command `rospacfind [package_name]` bisa kita gunakan untuk mencari path menuju ke _package_name_
5. Command `roscd [locationname[/subdir]]` bisa kita gunakan untuk berganti direktori, sama seperti command `cd` pada _Linux_
6. Command `roscd log` bisa kita gunakan untuk mengetahui program _ROS_ apa saja yang pernah kita jalankan, dengan cara membawa kita ke folder log
7. Command `rosls [locationname[/subdir]]` bisa kita gunakan untuk mengetahui list dari apa saja isi dari direktori yang kita inginkan, sama seperi command `ls` pada _Linux_
8. Kita bisa menggunakan _Tab Completion_ untuk auto complete command kita dengan menekan tab 2 kali, sama seperti pada _Linux_
9. Dan itulah semua, command yang bisa kita gunakan untuk menavigasi _filesystem ROS_
(**Selesai pada 8 November 2019, jam 12.30**)          

#### 3. Membuat Package _Catkin_
1. Agar sebuah package bisa disebut sebagai _package catkin_, package tersebut perlu memenuhi:
    * Harus memiliki file _package.xml yang berisi informasi meta tentang package tersebut
    * Harus memiliki file _CMakeList.txt_ yang mengandung catkin
    * Harus memiliki direktori tersendiri tanpa ada nested directory apapun
2. Pertama-tama, masuk ke direktori _src_ dengan command :
```
cd ~/catkin_ws/src
``` 
(**Selesai pada 9 November 2019, jam 20.00**) 
          
3. lalu gunakan script _catkin_create_pkg_ untuk membuat sebuah package dengan nama "beginner_tutorials" yang bergantung pada _std_msgs_ , _roscpp_ , dan _rospy_ dengan command:
```
catkin_create_pkg beginner_tutorials std_msgs rospy roscpp
```
(**Selesai pada 9 November 2019, jam 20.02**)            

4. Command tersebut diatas mempunyai syntax :
``` 
catkin_create_pkg <package_name> [depend1] [depend2] [depend3] 
```
5. Lalu, kita pergi ke direktori _catkin_ws_ untuk membuat package pada _catkin workspace_ dengan command:
```
cd ~/catkin_ws
```
(**Selesai pada 9 November 2019, jam 20.03**)         
 
6. Lalu gunakan command :
``` 
catkin_make
``` 
untuk membuat packagenya
(**Selesai pada 9 November 2019, jam 20.04**)       
   
7. Untuk menambahkan workspace kita ke _Filesystem ROS_ kita perlu melakukan source pada setup file nya dengan command :
``` 
~/catkin_ws/devel/setup.bash
```
(**Selesai pada 9 November 2019, jam 20.05**)         

8. Kita bisa menggunakan command `rospack depends1 beginner_tutorials` untuk melihat pada file apa saja _beginner_tutorials_ ini bergantung (dependensi)
9. lalu kita bisa mengubah isi dari package.xml, pertama-tama kita lihat terlebih dahulu isinya dengan command :
```
cat package.xml
```
 (**Selesai pada 9 November 2019, jam 20.07**)         
 
 10. _Package.xml_ terdiri dari beberapa bagian, yaitu :
     * Description Tag 
      ```
      <description>The beginner_tutorials package</description>
      ```
      yang isinya adalah deskripsi dari apa yang akan kita buat
      * Mantainer Tag
      ```
      <maintainer email="bryanyehuda@gmail.com">Bryan Yehuda</maintainer>
      ```
      yang isinya adalah kontak dari orang yang bertanggung jawab atas package tersebut
      * License Tag
      ```
      <license>BSD</license>
      ```
      yang isinya adalah lisensi dari package tersbut
      * Dependencies Tag
      ```
      <buildtool_depend>catkin</buildtool_depend>
      <build_depend>roscpp</build_depend>
      <build_depend>rospy</build_depend>
      <build_depend>std_msgs</build_depend>
      <exec_depend>roscpp</exec_depend>
      <exec_depend>rospy</exec_depend>
      <exec_depend>std_msgs</exec_depend>
      ```
      yang isinya adalah list dari dependensi package tersebut
11.  Kita akan melakukan editing dari _package.xml_ sehingga hasil akhirnya adalah :
       ```
       <?xml version="1.0"?>
            <package format="2">
                <name>beginner_tutorials</name>
                <version>0.1.0</version>
                <description>The beginner_tutorials package</description>

		<maintainer email="bryanyehuda@gmail.com">Bryan Yehuda Mannuel</maintainer>
                <license>BSD</license>
                <url type="website">http://wiki.ros.org/beginner_tutorials</url>
                <author email="bryanyehuda@gmail.com">Bryan Yehuda Mannuel</author>
                <buildtool_depend>catkin</buildtool_depend>
                <build_depend>roscpp</build_depend>
                <build_depend>rospy</build_depend>
                <build_depend>std_msgs</build_depend>
                <exec_depend>roscpp</exec_depend>
                <exec_depend>rospy</exec_depend>
                <exec_depend>std_msgs</exec_depend>
        </package>
(**Selesai pada 9 November 2019, jam 20.20**)        

#### 4. Membuat Package _Catkin_ Lanjutan
1. Jangan lupa melakukan sourcing pada setup dengan command :
```
source /opt/ros/melodic/setup.bash
```
(**Selesai pada 9 November 2019, jam 20.21**)         

2. masuk ke direktori_catkin_ws_ dengan command :
```
cd ~/catkin_ws/
```
 (**Selesai pada 9 November 2019, jam 20.22**)     
    
 3. Lalu build packagenya dengan command :
 ```
 catkin_make
 ```
 akan keluar log yang panjang sekali di terminal, tanda package sedang dibuild
 (**Selesai pada 9 November 2019, jam 20.24**)         
 
 4. Dan, package _catkin_ sudah selesai dibuat dan siap untuk digunakan
 (**Selesai pada 9 November 2019, jam 20.25**)        

#### 5. Mempelajari Nodes pada _ROS_
1. Sebelum memulai tutorial ini, kita perlu mendownload file tutorial dengan command :
```
sudo apt-get install ros-melodic-ros-tutorials
```
 (**Selesai pada 11 November 2019, jam 19.01**)         
 
2. Beberapa istilah dalam _ROS_ yang perlu diketahui:
   * Nodes : adalah sebuah file yang bisa dijalankan yang membutuhkan _ROS_ untuk berkomunikasi dengan nodes lainnya
   * Messages : tipe data _ROS_ yang digunakan ketika subscribing atau publishing sebuah topic
   * Topic : Nodes bisa subscribe ke topic untuk menerima messages atau publish ke topic untuk mengirim messages
   * Master : nameservice untuk _ROS_ (membantu nodes menemukan satu sama lain)
   * rosout : sama seperti stdout/stderr
   * roscore : master + rosout + parameter service
3. Library client pada _ROS_ terdiri dari 2 bahasa pemrograman yaitu :
   * roscpp : c++
   * rospy : python
4. Command `roscore` adalah hal paling pertama yang harus dijalankan apabila menggunakan _ROS_
5. Buka tab terminal baru, karena `roscore` harus tetap running selama kita menjalankan _ROS_ dan gunakan command :
```
rosnode list
```
untuk melihat nodes apa saja yang sedang berjalan pada saat itu, hanya ada /rosout
(**Selesai pada 11 November 2019, jam 19.02**)       
 
6. Kita bisa menggunakan command `rosnode info /rosout` untuk mendapatkan info lebih tentang nodes rosout
7. Command `rosrun` digunakan untuk menjalankan package tanpa perlu repot-repot mengetik semua path yang ada
8. Jalankan _turtlesim_ dengan command :
```
rosrun turtlesim turtlesim_node
```
(**Selesai pada 11 November 2019, jam 19.03**)     
    
9. Sekarang apabila kita menggunakan command `rosnode list` lagi, kita akan melihat ada 2 aktivitas nodes yaitu /rosout dan /turtlesim
(**Selesai pada 11 November 2019, jam 19.04**)         


#### 6. Mempelajari Topic pada _ROS_
1. Jalankan roscore dengan command :
```
roscore
```
dan buka terminal baru
(**Selesai pada 11 November 2019, jam 19.05**)      
   
2. Jalankan _turtlesim_ dengan command :
```
rosrun turtlesim turtlesim_node
```
(**Selesai pada 11 November 2019, jam 19.06**)       
   
3. Gunakan command :
```
rosrun turtlesim turtle_teleop_key
```
agar kita bisa mengontrol pergerakan kura-kura dengan keyboard
(**Selesai pada 11 November 2019, jam 19.07**)       
  
4. Dari sini bisa terlihat bahwa node _turtlesim_node_ dan node _turtle_teleop_key_ sedang berkomunikasi anatara satu sama lain dengan menggunakan topic, dimana node _turtle_teleop_key_ melakukan publishing lewat keyboard dan node _turtlesim_node_ melakukan subscribe dengan menerima messages tersebut
5. Kita bisa melihat hubungan ini lebih jelas dengan menggunakan bantuan _rqt_graph_ yang harus diinstal terlebih dahulu dengan command :
```
sudo apt-get install ros-melodic-rqt
sudo apt-get install ros-<distro>-rqt-common-plugins
```
dan buka terminal baru dan masukkan command :
```
rosrun rqt_graph rqt_graph
```
Dan, bisa dilihat dari graphic yang keluar, dengan jelas hubungan antara kedua node tersebut
(**Selesai pada 11 November 2019, jam 19.10**)          

6. Command `rostopic` bisa memberi kita info lebih lanjut tentang topic yang ada
7. Command `rostopic -h` bisa memberi tahu kita informasi tentang sub-command bagi rostopic
8. Command `rostopic echo /turtle1/cmd_vel` bisa memberi tahu kita, data apa saja yang terpublish pada suatu topic (agar command ini memberi hasil, kita perlu menggerakkan kura-kura). Dan apabila kita merefresh _rqt_graph_ kita bisa melihat bahwa echo tersubscribe ke topic _turtle1/command_velocity_
9. Command `rostopic list -h` bisa memberi tahu kita informasi tentang sub-command bagi rostopic list
10. Command `rostopic list -v` bisa memberi tahu kita informasi tentang verbose list dari topic dan tipe data mereka
11. Agar node bisa berkomunikasi satu dengan yang lain, maka mereka saling mengirim dan menerima messages. Kita bisa menggunakan command `rostopic type` untuk mendapatkan informasi tentang type messages yang dikirimkan dan diterima antara node yang ada
12. Command `rostopic pub` untuk mempublish data kepada topic yang sedang dijalankan
13. Command ini mempunyai syntax :
```
rostopic pub [topic] [msg_type] [args]
```
dan kita bisa menggunakannya pada kura-kura kita dengan command :
```
rostopic pub -1 /turtle1/cmd_vel geometry_msgs/Twist -- '[2.0, 0.0, 0.0]' '[0.0, 0.0, 1.8]'
```
(**Selesai pada 11 November 2019, jam 19.25**)           
yang nantinya command ini akan menyuruh kura-kura kita bergerak dengan kecepatan liner 2.0 dan kecepatan anguler 1.8 sebanyak sekali

14. Di command ini ada beberapa bagian yaitu:
    * `rostopic pub` mempublish data kepada topic yang sedang dijalankan
    * `-1`mempublish data sebanyak sekali saja
    * `/turtle1/cmd_vel`topic tujuan
    * `geometry_msgs/Twist` type message
    * `--`optional bisa diisi atau tidak, disini kita mengosonginya
    * `'[2.0, 0.0, 0.0]' '[0.0, 0.0, 1.8]'`kecepatan linear dan anguler
15. Kita bisa menggunakan `rostopic pub` untuk mengirim command berkali-kali dengan menambahkan `-r` pada command, sehingga menjadi:
```
rostopic pub /turtle1/cmd_vel geometry_msgs/Twist -r 1 -- '[2.0, 0.0, 0.0]' '[0.0, 0.0, -1.8]'
```
(**Selesai pada 11 November 2019, jam 19.27**)         

16. Command `rostopic hz /turtle1/pose` digunakan untuk memberi tahu seberapa besar data yang dipublish tiap detik oleh suatu node 
(**Selesai pada 11 November 2019, jam 19.28**)          
17. Kita bisa menggunakan command `rosrun rqt_plot rqt_plot` untuk melihat perpindahan kura-kura kita tiap detik pada grafik x dan y
(**Selesai pada 11 November 2019, jam 19.29**)           


#### 7. Mempelajari Service dan Parameter pada _ROS_
1. Service adalah cara lain agar nodes bisa berkomunikasi. Services terdiri dari pengiriman request dan penerimaan response
2. Command `rosservice` akan menampilkan command apa saja yang tersedia bagi rosservice
3. Command `rosservice list`akan menampilkan service apa saja yang disediakan oleh suatu node
4. Command `rosservice type [service]` memberi tahu type apakah suatu service tersebut
5. Command `rosservice call [service] [args]` akan memanggil service yang kita inginkan menurut argumen yang kita set
6. Command `rosservice call /clear` tidak membutuhkan argumen dan membersihkan background dari node
7. Command `rosservice call /spawn 2 2 0.2 ""` akan memanggil kura-kura baru pada posisi 2 2 0.2
8. Parameter Service menyimpan data integers, floats, boolean, dictionaries, dan list pada sistem _ROS_. Seperti semacam acuan baku untuk sistem _ROS_
9. Command `rosparam` memungkinkan kita untuk memanipulasi data tersebut dan akan menampilkan command apa saja yang tersedia bagi rosparam
10. Command `rosparam list`akan menampilkan parameter apa saja yang ada pada suatu node
11. Command `rosparam set /background_r 150` akan mengubah warna backgorund dari turtlesim menjadi merah, namun sebelum perubahan itu terjadi, kita perlu melakukan clear terlebih dahulu dengan command :
```
rosservice call /clear
```
dan bisa dilihat bahwa warna background dari turtlesim berubah menjadi merah
(**Selesai pada 11 November 2019, jam 19.45**)          

#### 8. Menggunakan rqt_console dan roslaunch
1. Sebelum memulai tutorial ini, kita perlu mendownload file tutorial dengan command :
```
sudo apt-get install ros-melodic-rqt ros-melodic-rqt-common-plugins ros-melodic-turtlesim
```
2. Jalankan _rqt_console_ dengan command :
```
rosrun rqt_console rqt_console
```
Pada terminal baru, dan akan muncul tab baru
(**Selesai pada 11 November 2019, jam 19.48**)       
 
3. Jalankan _rqt_logger_level_ dengan command :
```
rosrun rqt_logger_level rqt_logger_level
```
Pada terminal baru, dan akan muncul tab baru
(**Selesai pada 11 November 2019, jam 19.49**)     
   
4. Jalankan _turtlesim_ dengan command :
```
rosrun turtlesim turtlesim_node
```
akan muncul info pada tab _rqt_console_
(**Selesai pada 11 November 2019, jam 19.50**)        

5. Lalu ganti logger level pada _rqt_logger_level_ ke level warn
6. Tabrakkan kura-kura kita ke dinding dengan command :
```
rostopic pub /turtle1/cmd_vel geometry_msgs/Twist -r 1 -- '{linear: {x: 2.0, y: 0.0, z: 0.0}, angular: {x: 0.0,y: 0.0,z: 0.0}}'
```
akan muncul warning yang sangat banyak pada _rqt_console_
(**Selesai pada 11 November 2019, jam 19.52**)         

7. Logging level diurutkan berdasarkan 
```
Fatal
Error
Warn
Info
Debug
```
Yang berarti apabila kita memilih level warn, hanya informasi tentang fatal, error, dan warn saja yang akan ditampilkan, dan apabila kita memilih level debug, maka semua informasi akan ditampilkan
(**Selesai pada 11 November 2019, jam 19.53**)         

8. Menggunakan command `roslaunch` dengan syntax :
```
roslaunch [package] [filename.launch]
``` 
yang akan menjalankan filename.launch yang berbentuk tipe file launch pada package

9. Mari kita kembali ke package beginner_tutorial dengan command:
``` 
cd ~/catkin_ws
source devel/setup.bash
roscd beginner_tutorials
```
(**Selesai pada 11 November 2019, jam 19.55**)        

10. Lalu kita buat direktori launch dengan command :
```
mkdir launch
cd launch
```
(**Selesai pada 11 November 2019, jam 19.56**)           

11. Lalu buat file launch dengan nama turtlemimic.launch yang berisi :
```
<launch>
<group ns="turtlesim1">
<node pkg="turtlesim" name="sim" type="turtlesim_node"/>
</group>
<group ns="turtlesim2">
<node pkg="turtlesim" name="sim" type="turtlesim_node"/>
</group>
<node pkg="turtlesim" name="mimic" type="mimic">
<remap from="input" to="turtlesim1/turtle1"/>
<remap from="output" to="turtlesim2/turtle1"/>
</node>
</launch>
```
yang mana isinya adalah kita membuat 2 kura-kura pada saat bersamaan, dan kemudian menyuruh kura-kura pertama untuk bergerak sesuai command `rostopic pub`, dan menyuruh kura-kura kedua untuk meniru gerakan kura-kura pertama
(**Selesai pada 11 November 2019, jam 20.01**)        

12. Lalu jalankan turtlemimic.launch dengan command :
```
roslaunch beginner_tutorials turtlemimic.launch
```
(**Selesai pada 11 November 2019, jam 20.15**)          

13. Dan masukkan command :
```
rostopic pub /turtlesim1/turtle1/cmd_vel geometry_msgs/Twist -r 1 -- '[2.0, 0.0, 0.0]' '[0.0, 0.0, -1.8]'
```
(**Selesai pada 11 November 2019, jam 20.20**)         


#### 9. Mengedit files pada _ROS_ dengan rosed
1. Melakukan instalasi Vim Editor yang dibutuhkan oleh _ROS_ dengan command :
```
sudo apt-get update
sudo apt-get install vim
```
(**Selesai pada 11 November 2019, jam 20.30**)            

2. Melakukan editing pada file dengan command `rosed` menggunakan syntax :
```
rosed [package_name] [filename]
```
dengan contoh :
```
rosed roscpp Logger.msg
```
(**Selesai pada 11 November 2019, jam 20.32**)           

3. Kita juga bisa menggunakan editor bawaan _Linux Ubuntu_ yaitu nano dengan syntax :
```
nano [filename]
```
(**Selesai pada 11 November 2019, jam 20.33**)

#### 10. Membuat _ROS_ msg dan srv
1.  File msg adalah file sederhana yang mendeskripsikan besar dari suatu Message _ROS_. Mereka digunakan untuk menghasilkan source code dalam berbagai macam bahasa
2. File srv adalah file yang mendeskripsikan service. Terdiri dari 2 bagian, yaitu request dan response
3. Berbagai macam field type yang bisa digunakan untuk msg adalah:
   * int8, int16, int32, int64 (plus uint*)
   * float32, float64
   * string
   * time, duration
   * other msg files
   * variable-length array[] dan fixed-length array[C]
4. Ada juga type spesial bagi msg yaitu Header. Header berisi timestamp dan juga informasi koordinasi fram yang sering digunakan dalam _ROS_, contoh msg yang menggunakan Header adalah :
```
Header header
string child_frame_id
geometry_msgs/PoseWithCovariance pose
geometry_msgs/TwistWithCovariance twist
```
5. File srv sama seperti file msg hanya saja mereka terdiri dari 2 bagian yaitu request dan response, yang mana kedua bagian itu dipisahkan oleh --- seperti pada contoh :
```
int64 A
int64 B
---
int64 Sum
```
6. Mari kita membuat msg di dalam package yang sudah dibuat sebelumnya dengan command :
```
roscd beginner_tutorials
mkdir msg
echo "int64 num" > msg/Num.msg
```
(**Selesai pada 11 November 2019, jam 21.31**)         

7. Dan kemudian copy isi dari Num.msg seperti dibawah :
```
string first_name
string last_name
uint8 age
uint32 score
```
(**Selesai pada 11 November 2019, jam 21.33**)         

8. Lalu tambahkan command ini pada package.xml :
```
<build_depend>message_generation</build_depend>
<exec_depend>message_runtime</exec_depend>
```
agar source code nya bisa diubah ke berbagai macam bahasa yang kita inginkan
(**Selesai pada 11 November 2019, jam 21.34**)        

9. Lalu tambahkan command ini pada CMakeList.txt pada bagian function _find_package_ :
```
message_generation
```
(**Selesai pada 11 November 2019, jam 21.36**)        

10. Lalu tambahkan command ini pada CMakeList.txt pada bagian function _catkin_package_ :
```
CATKIN_DEPENDS message_runtime
```
(**Selesai pada 11 November 2019, jam 21.38**)         

11. Lalu lakukan uncomment pada :
```
# add_message_files(
#   FILES
#   Message1.msg
#   Message2.msg
# )
```
sehingga menjadi :
```
add_message_files(
 FILES
 Num.msg
)
```
(**Selesai pada 11 November 2019, jam 21.39**)           

12. Lalu lakukan uncomment pada :
```
# generate_messages(
#   DEPENDENCIES
#   std_msgs
# )
```
sehingga menjadi :
```
generate_messages(
 DEPENDENCIES
 std_msgs
)
```
(**Selesai pada 11 November 2019, jam 21.40**)          

13. Pastikan _ROS_ bisa melihat msg nya dengan menggunakan command :
```
rosmsg show beginner_tutorials/Num
```
(**Selesai pada 11 November 2019, jam 21.42**)     
  
14. Mari kita membuat srv di dalam package yang sudah dibuat sebelumnya dengan command :
```
roscd beginner_tutorials
mkdir srv
```
(**Selesai pada 11 November 2019, jam 21.44**)        

15. Lakukan copy dengan command :
```
roscp rospy_tutorials AddTwoInts.srv srv/AddTwoInts.srv
```
yang mempunyai syntax :
```
roscp [package_name] [file_to_copy_path] [copy_path]
```
(**Selesai pada 11 November 2019, jam 21.46**)           

16. Lalu lakukan uncomment pada :
```
# add_service_files(
#   FILES
#   Service1.srv
#   Service2.srv
# )
```
sehingga menjadi :
```
add_service_files(
 FILES
 AddTwoInts.srv
)
```
(**Selesai pada 11 November 2019, jam 21.48**)          
 
17. Pastikan _ROS_ bisa melihat srv nya dengan menggunakan command :
```
rossrv show beginner_tutorials/AddTwoInts
```
(**Selesai pada 11 November 2019, jam 21.50**)          

18. Command `rosmsg -h` nisa kita gunakan untuk mencari bantuan pada command rosmsg

#### 11. Membuat Publisher dan Subscriber dalam c++
1. Masuk ke direktori beginner_tutorials dengan command :
```
roscd beginner_tutorials
```
(**Selesai pada 11 November 2019, jam 21.51**)         
 
2. Buat direktori baru dengan command : 
```
mkdir -p src
```
(**Selesai pada 11 November 2019, jam 21.54**)           

3. Buat file src/talker.cpp yang berisi :
```
#include "ros/ros.h"
#include "std_msgs/String.h"
#include <sstream>
/**
 * This tutorial demonstrates simple sending of messages over the ROS system.
 */
int main(int argc, char **argv)
{
 /**
 * The ros::init() function needs to see argc and argv so that it can perform
 * any ROS arguments and name remapping that were provided at the command line.
 * For programmatic remappings you can use a different version of init() which takes
 * remappings directly, but for most command-line programs, passing argc and argv is
 * the easiest way to do it.  The third argument to init() is the name of the node.
 *
 * You must call one of the versions of ros::init() before using any other
 * part of the ROS system.
 */
 ros::init(argc, argv, "talker");
 /**
 * NodeHandle is the main access point to communications with the ROS system.
 * The first NodeHandle constructed will fully initialize this node, and the last
 * NodeHandle destructed will close down the node.
 */
 ros::NodeHandle n;
 /**
 * The advertise() function is how you tell ROS that you want to
 * publish on a given topic name. This invokes a call to the ROS
 * master node, which keeps a registry of who is publishing and who
 * is subscribing. After this advertise() call is made, the master
 * node will notify anyone who is trying to subscribe to this topic name,
 * and they will in turn negotiate a peer-to-peer connection with this
 * node.  advertise() returns a Publisher object which allows you to
 * publish messages on that topic through a call to publish().  Once
 * all copies of the returned Publisher object are destroyed, the topic
 * will be automatically unadvertised.
 *
 * The second parameter to advertise() is the size of the message queue
 * used for publishing messages.  If messages are published more quickly
 * than we can send them, the number here specifies how many messages to
 * buffer up before throwing some away.
 */
 ros::Publisher chatter_pub = n.advertise<std_msgs::String>("chatter", 1000);
 ros::Rate loop_rate(10);
 /**
 * A count of how many messages we have sent. This is used to create
 * a unique string for each message.
 */
 int count = 0;
 while (ros::ok())
 {
 /**
 * This is a message object. You stuff it with data, and then publish it.
 */
 std_msgs::String msg;
 std::stringstream ss;
 ss << "hello world " << count;
 msg.data = ss.str();
 ROS_INFO("%s", msg.data.c_str());
 /**
 * The publish() function is how you send messages. The parameter
 * is the message object. The type of this object must agree with the type
 * given as a template parameter to the advertise<>() call, as was done
 * in the constructor above.
 */
 chatter_pub.publish(msg);
 ros::spinOnce();
 loop_rate.sleep();
 ++count;
 }
 return 0;
}
```
(**Selesai pada 11 November 2019, jam 21.58**)          
 
4. Code di atas berisi command:
   * Inisialisasi system _ROS_
   * Advertise bahwa kita akan mempublish message [std_msgs/String](http://docs.ros.org/api/std_msgs/html/msg/String.html) pada topic Chatter kepada Master
   * Lopp selagi publish message ke topic Chatter sebanyak 10 kali per detik
 5. Buat file src/listener.cpp yang berisi :
 ```
 #include "ros/ros.h"
#include "std_msgs/String.h"
/**
 * This tutorial demonstrates simple receipt of messages over the ROS system.
 */
void chatterCallback(const std_msgs::String::ConstPtr& msg)
{
 ROS_INFO("I heard: [%s]", msg->data.c_str());
}
int main(int argc, char **argv)
{
 /**
 * The ros::init() function needs to see argc and argv so that it can perform
 * any ROS arguments and name remapping that were provided at the command line.
 * For programmatic remappings you can use a different version of init() which takes
 * remappings directly, but for most command-line programs, passing argc and argv is
 * the easiest way to do it.  The third argument to init() is the name of the node.
 *
 * You must call one of the versions of ros::init() before using any other
 * part of the ROS system.
 */
 ros::init(argc, argv, "listener");
 /**
 * NodeHandle is the main access point to communications with the ROS system.
 * The first NodeHandle constructed will fully initialize this node, and the last
 * NodeHandle destructed will close down the node.
 */
 ros::NodeHandle n;
 /**
 * The subscribe() call is how you tell ROS that you want to receive messages
 * on a given topic.  This invokes a call to the ROS
 * master node, which keeps a registry of who is publishing and who
 * is subscribing.  Messages are passed to a callback function, here
 * called chatterCallback.  subscribe() returns a Subscriber object that you
 * must hold on to until you want to unsubscribe.  When all copies of the Subscriber
 * object go out of scope, this callback will automatically be unsubscribed from
 * this topic.
 *
 * The second parameter to the subscribe() function is the size of the message
 * queue.  If messages are arriving faster than they are being processed, this
 * is the number of messages that will be buffered up before beginning to throw
 * away the oldest ones.
 */
 ros::Subscriber sub = n.subscribe("chatter", 1000, chatterCallback);
 /**
 * ros::spin() will enter a loop, pumping callbacks.  With this version, all
 * callbacks will be called from within this thread (the main one).  ros::spin()
 * will exit when Ctrl-C is pressed, or the node is shutdown by the master.
 */
 ros::spin();
 return 0;
}
 ```
  (**Selesai pada 11 November 2019, jam 22.20**)            
  
 6. Code di atas berisi command:
   * Inisialisasi system _ROS_
   * Subscribe ke topic Chatter
   * Spin dan tunggu messages untuk datang
   * Ketika messages dayang, function _chatterCallback()_ dipanggil
 7. Membangun nodes yang ada pada _[CMakeLists.txt](http://wiki.ros.org/catkin/CMakeLists.txt)_ sehingga terbentuk seperti ini :
```
cmake_minimum_required(VERSION 2.8.3)
project(beginner_tutorials)
## Find catkin and any catkin packages
find_package(catkin REQUIRED COMPONENTS roscpp rospy std_msgs genmsg)
## Declare ROS messages and services
add_message_files(FILES Num.msg)
add_service_files(FILES AddTwoInts.srv)
## Generate added messages and services
generate_messages(DEPENDENCIES std_msgs)
## Declare a catkin package
catkin_package()
## Build talker and listener
include_directories(include ${catkin_INCLUDE_DIRS})
add_executable(talker src/talker.cpp)
target_link_libraries(talker ${catkin_LIBRARIES})
add_dependencies(talker beginner_tutorials_generate_messages_cpp)
add_executable(listener src/listener.cpp)
target_link_libraries(listener ${catkin_LIBRARIES})
add_dependencies(listener beginner_tutorials_generate_messages_cpp)
```
(**Selesai pada 11 November 2019, jam 22.30**)          

8. Code di atas berisi command untuk membuat dua executeables yaitu _talker_ dan _listener_ dengan dependensi mereka masing-masing
9. Lalu, jalankan _catkin_make_ dengan command:
 ```
 cd ~/catkin_ws
catkin_make
``` 
(**Selesai pada 11 November 2019, jam 22.32**)          

#### 13. Menjalankan Publisher dan Subscriber dalam c++
1. Jalankan `roscore`
(**Selesai pada 11 November 2019, jam 22.33**)        
2. Jangan lupa melakukan sourcing pada file setup dengan command :
```
cd ~/catkin_ws
source ./devel/setup.bash
```
(**Selesai pada 11 November 2019, jam 22.34**)       
  
3. Jalankan _talker_ dengan command :
```
rosrun beginner_tutorials talker
```
(**Selesai pada 11 November 2019, jam 22.35**)        
    
4. Jalankan _listener_ dengan command :
```
rosrun beginner_tutorials listener
```
(**Selesai pada 11 November 2019, jam 22.35**)        
  
5. Amati bahwa _talker_ dan _listener_ saling bertukar messages satu sama lain
(**Selesai pada 11 November 2019, jam 22.37**)            

