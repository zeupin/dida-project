# Dida Project Skeleton

A skeleton for creating projects with Dida Framework.

为您基于 Dida 框架开发的项目自动创建一个标准的官方应用框架。

## Installation 安装

```bash
# 用最新的版本生成一个项目框架
composer create-project --prefer-dist dida/project  您的项目名

# 用指定的2.4.*版本生成一个项目框架（方式1）
composer create-project --prefer-dist dida/project:2.4.*  您的项目名

# 用指定的2.4.*版本生成一个项目框架（方式2）
composer create-project --prefer-dist dida/project  您的项目名  2.4.*
```

### `composer create-project` 可使用的参数说明：

| 参数             | 说明                                                                        |
| ---------------- | --------------------------------------------------------------------------- |
| --repository-url | 提供一个自定义的储存库来搜索包，这将被用来代替 packagist.org(备注 1) 。     |
| --stability (-s) | 资源包的最低稳定版本，默认为 stable。                                       |
| --prefer-source  | 当有可用的包时，从 source 安装。                                            |
| --prefer-dist    | 当有可用的包时，从 dist 安装。                                              |
| --dev            | 安装 require-dev 字段中列出的包。                                           |
| --no-install     | 禁止安装包的依赖。                                                          |
| --no-plugins     | 禁用 plugins。                                                              |
| --no-scripts     | 禁止在根资源包中定义的脚本执行。                                            |
| --no-progress    | 移除进度信息，这可以避免一些不处理换行的终端或脚本出现混乱的显示。          |
| --keep-vcs       | 创建时跳过缺失的 VCS 。如果你在非交互模式下运行创建命令，这将是非常有用的。 |

备注：

1. 可以是一个指向 composer 资源库的 HTTP URL，或者是指向某个 packages.json 文件的本地路径。

## Usage 使用方法

```bash
# 进入项目目录
cd 您的项目路径

# 启动一个本地的服务器，进行项目配置（默认端口6789）
bin/dida server

# 启动一个本地的服务器，进行项目配置（自定义端口）
bin/dida server -p 端口号
```

然后，用 http://localhost:6789 或者 http://localhost:自定义端口号，即可进行配置。