# 第一次发布：LHLVisionDemo 完全自主实现 工业视觉定位  测量  预处理  亚像素  矫正 拟合等算法 
## 一、find模块参数解释
默认全图建模，如果选择roi需要绘制矩形框\
1、find_ncc                    默认参数可以直接使用，subpixel=0 结果无亚像素 subpixel=1 一维插值 subpixel=2 二维插值 \
2、find_shape                  默认参数可以直接使用，subpixel=0 结果无亚像素 subpixel=1 一维插值 subpixel=2 二维插值 subpixel=3 最小二乘拟合\
3、find_scale_shape            默认参数可以直接使用，subpixel=0 结果无亚像素 subpixel=1 一维插值 subpixel=2 二维插值 subpixel=3 最小二乘拟合\
4、find_pat_scale_shape        默认参数可以直接使用，默认执行最小二乘拟合\
5、find_pat_aniso_scale_shape  默认参数可以直接使用，默认执行最小二乘拟合\
6、find_pat_scale_shape        默认参数可以直接使用，subpixel=0 结果无亚像素 subpixel=1 一维插值 subpixel=2 二维插值 subpixel=3 最小二乘拟合\
7、find_planar_deform_shape    默认参数可以直接使用，默认执行最小二乘拟合\
8、find_local_deform           默认参数可以直接使用，内部无最小二乘拟合\
9、find_feat_points_shape      默认参数可以直接使用，默认执行最小二乘拟合\
注意:带pat的，在创建模板的时候Grand选取不同会导致结果差别比较大，内部有自动计算，如果失败需要手动调节\
## 二、blob
    目前只支持threshold  connection
## 八、subpixel
    目前支持多个亚像素操作

## dll里面有很多算法，没有全部做到界面，如果想看效果可以@作者

## QQ交流群 1076120833
