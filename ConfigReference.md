# Dependencies #
Omegalib libraries and basic can be compiled out of the box without needing any external libraries. Optionally, support for external graphic libraries and toolkits can be added by enabling the specific options inside CMake, and configuring the libraries accordingly.
## Python ##
Omegalib has been tested with Python 2.7
## Open Scene Graph ##
**todo**
## The Visualization Toolkit ##
**todo**
## Qt ##

# CMake variables #
  * `OMEGA_USE_DISPLAY` Enable if you want to write applications that use omegalib to handle graphics.
  * `OMEGA_BUILD_APPS` Enable to build applications, demos and examples included with the omegalib distribution
  * `OMEGA_BUILD_STATIC` (**Experimental**) When selected, omegalib will be built as a static library.
  * `OMEGA_USE_PYTHON` Enable python support inside omegalib. You need a python library distribution installed
  * `OMEGA_BUILD_VTK_LIB` Enable to build the vtk support library. Vtk applications will be built as well if `OMEGA_BUILD_APPS` is enabled
  * `OMEGA_BUILD_OSG_LIB` Enable to build the Open Scene Graph support library. Osg applications will be built as well if `OMEGA_BUILD_APPS` is enabled
  * `OMEGA_BUILD_QT_LIB` Enable to build the Qt support library. Qt applications will be built as well if `OMEGA_BUILD_APPS` is enabled

# Compiler definitions #
The following preprocessor definitions are generated by cmake for all the projects that are part of the omegalib distribution.
Definitions identifying the operating system
  * `OMEGA_OS_WIN`
  * `OMEGA_OS_OSX`
  * `OMEGA_OS_LINUX`
Definitions identifying 64 bit builds
  * `OMEGA_ARCH_WIN32`
  * `OMEGA_ARCH_WIN64`
  * `OMEGA_ARCH_I386`
  * `OMEGA_ARCH_AMD64`
> (**Note: this may be changed in the future to a simpler system**)
Definitions identifying the build toolset
  * `OMEGA_TOOL_VS9`
  * `OMEGA_TOOL_VS10`
  * `OMEGA_TOOL_XCODE`
  * `OMEGA_TOOL_GCC`