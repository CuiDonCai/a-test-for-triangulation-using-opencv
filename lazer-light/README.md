由于购买的摄像头不合适, 没办法及时调试

原计划自己照书上算法写程序暂时搁置

查遍了opencv的module, 包括额外的包opencv_contrib, 没有关于线激光扫描的模块以及例程.

目前Google不到相关的源码, 而线激光扫描到现在仍是重要的应用, 应该是太简单而用不到opencv吧.

哪怕弄不到源码, 只有录像和相机参数这个项目也能继续下去.

接下来还是照下面的程序走

      捕获图像->灰度化->滤波降噪->二值化->找光线重心(算数或加权平均值)  (细化光线)
      
      立体标定->remap->计算视差->reprojectto3d->三维重建得到点云