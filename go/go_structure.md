# go 结构

- `package`定义包名，即程序属于哪个包
  - `package main`表示一个可独立执行的程序
  - 每个 go 的应用程序必须包含一个 main 包
- `import`表示程序需要使用的包，如 fmt 实现了格式化输入输出函数
- `func func_name(){}`定义了程序的函数
  - main 函数是每一个可执行程序必须包含的，一般来说都是在启动后第一个执行的函数
  - 有 init 函数的时候先执行 init 函数
- `/*...*/`和`//`是注释
- 标识符（常量、变量、类型、函数名、结构字段等）
  - 以大写字母开头，则该对象可以被外部包的代码使用，即导出（类比面向对象的 public）
  - 以小写字母开头，则对外包不可见，只在包内部可见可用（类比面向对象的 protected）
- 执行程序
  - 程序以`.go`结尾
  - 执行`go run filename.go`可允许代码
- Note：go 语言不支持`{`放单独一行，和 C 和 C++ 不一样