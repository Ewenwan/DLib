DLib
====

DLib is a collection of C++ classes to solve common tasks in C++ programs, as well as to offer additional functionality to use OpenCV data and to solve computer vision problems.

I have found myself using these functions very often, so I hope they may be useful to other researchers and developers too.

## Documentation

DLib is divided into 3 libraries for different purposes:

  * `DUtils`: utilities for several common C++ program requirements. It includes these classes:
    * `BinaryFile`: 读写二进制文件 reads/writes binary files
    * `LineFile`:   读写txt文件 reads/writes text files by lines
    * `ConfigFile`: 读写配置文件 reads/writes text files with the format `key = value`
    * `FileFunctions`: 文件夹函数 mkdir, rmdir, dir... functionality
    * `Math`:          数学函数 math functions
    * `Random`:        伪随机数 pseudo-random number functions
    * `STL`:           STL模板容器 functions for STL containers
    * `StringFunctions`: 字符串 functions to manipulae strings
    * `Timestamp`:       时间戳 operates with timestamps
    * `TimeManager`:     时间戳管理器  manages collections of timestamps
    * `Profiler`:        测量代码运行时间 measures execution time of portions of code
    * `DebugFunctions`:  内存消耗的代码测试函数 functions to measure memory consumption


  * `DUtilsCV`: utility functions for OpenCV data types. Classes included:
    * `Drawing`: 画图 关键点等 functions to draw keypoints, data, axes...
    * `GUI`:     界面shows images in windows and allows some user input
    * `IO`:      输入输出函数 I/O functions for storage and printing
    * `Mat`:     矩阵  functions to remove rows from matrices
    * `Transformations`: 空间转换函数 functions to deal with spatial transformations
    * `Types`:           数据类型转换 functions to convert between OpenCV data types


  * `DVision`: functions to solve computer vision tasks. Classes included:
    * `BRIEF`:   二进制描述符implementation of the BRIEF descriptor
    * `FSolver`: 基础矩阵求解 implementation of the RANSAC + 8-point algorithm to compute fundamental matrices between images
    * `HSolver`: 单应矩阵求解 implementation of the RANSAC + DLT algorithm to compute homographies between images
    * `ImageFunctions`: 图像块 functions to get patches from images
    * `BundleCamera`:   读/写由Bundle软件创建的相机文件 reads/writes camera files created by the Bundle software
    * `PMVSCamera`, `PatchFile`, `PLYFile`: read/write data created by the PMVS software
    * `PixelPointFile`, `Matches`: 像素、位姿文件读取 read/write multi-purpose pixel and 3D data files
