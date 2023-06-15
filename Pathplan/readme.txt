在windows环境，配置VS2019，使用matplotlib方法：

配置vs2019属性设置python3.9时：
链接器-->输入-->附加依赖项：直接设置为 python39.lib        不要设置为 python39_d.lib


安装Eigen库，导入包含目录：
C:\Program Files\Eigen3\include
C:\Program Files\Eigen3\include\eigen3
导入python及numpy包含目录：
C:\Program Files\Python39\include
C:\Users\zengpiaoyang\AppData\Roaming\Python\Python39\site-packages\numpy\core\include
导入当前工程头文件包含目录：
D:\MyWork\visual_project\Pathplan\include


导入python及numpy，包含库目录：
C:\Program Files\Python39\libs
C:\Users\zengpiaoyang\AppData\Roaming\Python\Python39\site-packages\numpy\lib


Eigen库的安装： CMake3.25.1 编译
git上下载eigen-3.4.0版本：  https://gitlab.com/libeigen/eigen/-/archive/3.4.0/eigen-3.4.0.zip
不要下载eigen-3.3.8版本，因为此版本编译CMake后，不能用vs2019 install到C:\Program Files\Eigen3