# 3DReconstruction_facial-reconstruction
3D facial reconstruction based on structured light camera

1、依赖环境

opencv、opencv_contrib、dlib、OpenNI2 orbbec

2、编译流程

cd .\infinitam_face\InfiniTAM\build （目录内包含cmakeCache.txt，可查看cmake配置）

cmake 

make -j20

3、运行

编译完成后，连接可正常读取RGB和深度图数据的Astra 摄像头，输入：

cd .\infinitam_face\InfiniTAM\build\Apps\InfiniTAM\

.\InfiniTAM  ..\..\..\Files\orbbec\calib.txt

即可运行。

在运行窗口打开后，按“b”开始读取摄像头数据，出现重建人脸后，慢慢转动头部，可精细化重建效果。

按“w”可保存重建好的点云，保存路径为 .\infinitam_face\InfiniTAM\build\Apps\InfiniTAM\mesh.stl
