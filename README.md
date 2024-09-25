# The Go Programming Language

Go is an open source programming language that makes it easy to build simple,
reliable, and efficient software.

![Gopher image](https://golang.org/doc/gopher/fiveyears.jpg)
*Gopher image by [Renee French][rf], licensed under [Creative Commons 4.0 Attribution license][cc4-by].*

Our canonical Git repository is located at https://go.googlesource.com/go.
There is a mirror of the repository at https://github.com/golang/go.

Unless otherwise noted, the Go source files are distributed under the
BSD-style license found in the LICENSE file.

### Download and Install

#### Binary Distributions

Official binary distributions are available at https://go.dev/dl/.

After downloading a binary release, visit https://go.dev/doc/install
for installation instructions.

#### Install From Source

If a binary distribution is not available for your combination of
operating system and architecture, visit
https://go.dev/doc/install/source
for source installation instructions.

### Contributing

Go is the work of thousands of contributors. We appreciate your help!

To contribute, please read the contribution guidelines at https://go.dev/doc/contribute.

Note that the Go project uses the issue tracker for bug reports and
proposals only. See https://go.dev/wiki/Questions for a list of
places to ask questions about the Go language.

[rf]: https://reneefrench.blogspot.com/
[cc4-by]: https://creativecommons.org/licenses/by/4.0/

# 使用vscode编译golang源码
### 1.安装golang开发环境
### 2.下载golang源码
### 3.运行src目录下的make.bash，此时golang源码将安装于src目录同级下的bin目录
### 4.修改vscode插件的配置，新增 "go.goroot": "/data/code/go/src/go" 指向golang源码路径，此处以该路径/data/code/go/src/go为例
### 5.重启vscode，此时源码中提示错误的internal调用会消失，单元测试也可以正常运行
### 6.需要使用修改的golang源码同理，编译后将go env下的go root指向编译后的位置即可以使用