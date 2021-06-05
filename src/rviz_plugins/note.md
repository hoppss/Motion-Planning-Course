# plugin 继承关系

Tool  <-  Pose3DTool   <- Goal3DTool


# plugin profile

快捷键 "g"， 和"2D Nav Goal" 相同， 所以同时加载插件，快捷键有问题
类型是Tool， 就是rviz 菜单栏下面的那一排按钮
左侧那种叫panel
名称: "3D Nav Goal"
话题发布接口 /goal，  [geometry_msgs::PoseStamped]

# 使用方法

默认rviz配置，参考 grid_path_searcher/launch/rviz_config/demo.rviz
点击插件
左键按住给出 x,y信息
左键按住不放，右键按下给出z 高度信息
左右键同时放开，发布消息



# 其他

waypoint_generator
接收/goal 目标请求，

random_complex
随机生成复杂的点云地图，用于规划


demo_node
可视化消息