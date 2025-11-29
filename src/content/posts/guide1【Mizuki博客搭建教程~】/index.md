---
title: Mizuki博客搭建教程~
published: 2025-11-29
description: 这是一篇H-CAT主题博客搭建的教程~
tags: [教程, 通知]
image: "./cover.png"
category: 教程
draft: false
---

# 博客搭建【基于Mizuki模板】

![Mizuki](https://docs.mizuki.mysqil.com/image.png)

**官方教程：[Mizuki Next Theme](https://docs.mizuki.mysqil.com/)https://docs.mizuki.mysqil.com/**

## 下载项目文件

>前往仓库下载项目文件
>
>H-CAT V1.0主题使用MizukiV7.5版本

::github{repo="halei0v0/H-CAT"}

::github{repo="matsuzaka-yuki/Mizuki"}

自行下载想要的版本解压即可。

# 1.安装使用

1. 环境依赖安装

    在开始使用 Mizuki 之前，您需要确保系统满足以下要求：

    - **Node.js >= 20**

      访问 [Node.js 官网](https://nodejs.org/) 下载并安装最新版本的 Node.js。建议使用 LTS 版本。

      安装完成后，打开终端或命令提示符，运行以下命令验证 Node.js 是否安装成功：

      ```
      node -v
      npm -v
      ```

      如果显示版本号，则表示安装成功。

    - **pnpm >= 9**

      如果您尚未安装 pnpm，可以通过 npm 安装：

      ```
      npm install -g pnpm
      ```

      安装完成后，打开终端或命令提示符，运行以下命令验证 pnpm 是否安装成功：

      ```
      pnpm -v
      ```

      如果显示版本号，则表示安装成功。

    - **Github Desktop**/ **Git**（可选）

      - 下载[Github Desktop](https://desktop.github.com/download/)

      :::note

      已安装**Github Desktop**无需再安装git

      :::

      - （可选）安装git

      访问 [Git 官网](https://git-scm.com/downloads) 下载并安装适合您操作系统的 Git 版本。

      安装完成后，打开终端或命令提示符，运行以下命令验证 Git 是否安装成功：

      ```
      git --version
      ```

      如果显示版本号，则表示安装成功。

2. 启动项目

    > 我们这里不选择直接克隆【国内环境克隆较慢，对小白不友好】

- 打开解压好的文件夹

- `cmd`以管理员身份运行【地址栏输入`cmd`然后`ctrl`+`shifi`+`enter`】

  - 安装依赖（使用pnpm）

  - ```
    pnpm install
    ```

- 配置博客
  - 在启动项目之前，您需要根据自己的需求进行配置【将在配置说明处进行详细说明，这里先进行部署】：
    - 编辑 `src/config.ts` 文件来自定义博客设置
    - 更新站点信息、主题颜色、横幅图片和社交链接
    - 配置翻译设置和特殊页面功能

- 启动开发服务器

  - 运行以下命令启动开发服务器：

  - ```
    pnpm dev
    ```

    启动成功后，您可以在浏览器中访问 `http://localhost:4321` 查看您的博客。



# 2.部署

> 综合所有方案，这里选择免费方案：`Vercel`、`Github Pages`部署

## Vercel部署（推荐）

1. 注册[Vercel](https://vercel.com/)
2. 选择H-CAT仓库
3. 绑定自定义域名
4. 部署成功~~

## Github Pages部署（不推荐）

1. Github Pages

如果您希望将博客托管在 GitHub Pages 上，Mizuki 项目通常会包含一个 GitHub Actions 工作流，可以帮助您自动化部署过程。您需要确保在配置正确的 `base` 路径。

2. 请以`<Github用户名>.github.io`命名仓库

   在 GitHub 上，跳转到存储库的 Settings 选项卡并找到设置的 Pages 部分。


- 选择 GitHub Actions 作为你网站的 Source，然后按 Save。

- 删除.github文件夹工作流文件中除了deploy以外的两个配置文件（不删除会报错）

  :::note

  你的网站现在应该已完成发布了！当你将更改推送到 Astro 项目的存储库时，GitHub Action 将自动为你部署它们。

  :::

# 3.软件推荐

[markdown编辑工具下载（Typora1.3.6）](https://kevinwu06.lanzout.com/iXkq30icv1ha)：https://kevinwu06.lanzout.com/iXkq30icv1ha

