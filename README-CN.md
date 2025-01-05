<div align="center">
  <h1>Vue Color Avatar</h1>

  <p>🧑‍🦱 一个纯前端实现的头像生成网站 🧑‍🦳</p>

[Read in English](./README.md)

</div>

<a href="https://color-avatar.acmsz.top/">
  <img src="./images/social-preview-1.png" alt="website-cover" />
</a>

## 在线预览

[`https://color-avatar.acmsz.top`](https://color-avatar.acmsz.top/)

## 介绍

**这是一款矢量风格头像的生成器，你可以搭配不同的素材组件，生成自己的个性化头像。**

你可能感兴趣的功能：

- 可视化组件配置栏
- 随机生成头像，有一定概率触发彩蛋
- 撤销/还原*更改*
- 国际化多语言
- 批量生成多个头像

## 设计资源

- 设计师：[@Micah](https://www.figma.com/@Micah) on Figma
- 素材来源：[Avatar Illustration System](https://www.figma.com/community/file/829741575478342595)

> **Note**  
> 虽然该项目是 MIT 协议，但是素材资源基于 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 协议。如果你有好的创意素材，欢迎补充！

## 项目开发

该项目使用 `Vue3` + `Vite` 进行开发。

```sh
# 1. 克隆项目至本地
git clone https://github.com/CMSZ001/vue-color-avatar.git

# 2. 安装项目依赖
yarn install

# 3. 运行项目
yarn dev
```

### Docker 快速部署

你可以直接使用我已经构建好的镜像来运行。

```sh
docker run -d -t -p 5173:8080 \
--name=vue-color-avatar \
--restart=always \
docker.io/wenyang0/vue-color-avatar:latest

```

或者，如果您愿意，也可以自己手动编译。

```sh
#下载代码
git clone https://github.com/CMSZ001/vue-color-avatar.git

#docker 编译
cd vue-color-avatar/
docker build -t vue-color-avatar:v1 .

#启动服务
docker run -d -t -p 5173:8080 --name vue-color-avatar --restart=always vue-color-avatar:v1
```

最后，打开你的浏览器访问服务的地址 http://serverIP:5173 即可。
