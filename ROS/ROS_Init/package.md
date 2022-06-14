# package

# package文件
    package/  
        CMakeLists.txt  
        package.xml  

# 创建package

    cd ~/catkin_ws/src
    catkin_create_pkg package_name std_msgs rospy roscpp

# catkin_create_pkg命令
    catkin_create_pkg <package_name> [depend1] [depend2] [depend3]