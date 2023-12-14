.vscode目录：
    Visual Studio Code项目配置文件存放目录，常包含c_cpp_properties.json、 launch.json、tasks.json，该文件夹一般不作为项目内容提交至Git仓库
3rd：
    第三方库文件存放目录
build：
    CMake项目编译配置和可执行文件存放目录，该文件夹一般不作为项目内容提交至Git仓库
doc：
    项目文档(说明文档、图片、视频等)存放目录
include：
    头文件(.hpp .h)存放目录
src：
    源文件(.cpp)存放目录
lib：
    生成的库文件存放目录，该文件夹一般不作为项目内容提交至Git仓库
test：
    测试文件存放目录
.clang-format：
    clang-format工具配置文件，该文件一般不作为项目内容提交至Git仓库
main.cpp：项目启动源文件
package.xml：ROS/ROS2项目专属配置文件，非ROS/ROS2项目不需要包含
CMakeLists.txt：CMake项目配置文件，必须包含
Readme.md：
    MarkDown格式的项目说明文档，文档内引用的图片建议存放在doc文件夹下，图片引用路径使用相对路径，方便直接在GitLab网页端展示完整的Readme