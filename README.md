# mypUI

**快速开发nvue页面的组件库与工具集**

- nvue页面，兼容vue页面；
- 纯flex布局，符合weex规范；
- 规范与统一，确保代码质量和开发效率；
- 可配置主题；
- 细节开放到位，在好用和可灵活适配之间把握到位；
- request/router/share...各种工具集；

# TODO
- 统一与规范字段；
- 完善文档；

# 组织结构
- `分享`：开发时的注意事项，以及学习资料；
- `mypUI`：公共组件以及工具库，组件数量不多，都是一些最基础的组件；
- `components`：基于mypUI衍生的组件，落地组件；
- `pages`：页面内容；
- `router`：路由相关的一些工具与`mixin`；
- `service`：常用的一些`mixin`；
- `store`：`vuex`；

# 使用注意

- 直接将`mypUI`放在项目根目录下；
- `loadingSrc`等公用静态资源直接使用了`/static/ui`下面的静态文件，没有使用网络图片，所以需要拷贝到自己的项目下，而且路径保持一致；
- `easycom`开启配置，在`pages.json`下配置：

```json
"easycom": {
	"autoscan": true,
	"custom": {
		"myp-(.*)": "@/mypUI/myp-$1/myp-$1.vue" // 匹配mypUI内的vue文件
	}
}
```

# 说明

- 当时写这套nvue页面的时候，还没有任何一款nvue页面组件在开放或者售卖。
- 第一版的时候，其实是根据weex-ui改的。scroll是根据mescroll改的（当时mescroll还不是mixin的形式）。
- 其实我是想搞一个设计软件，设计即uni-app代码，而且是nvue代码，减少大量的开发时间，甚至直接通过简短的几句描述就实现页面。

希望对你有用。

# 工具

- [免费图片压缩](https://tinypng.com/)
- [免费图片托管](https://img.wenhairu.com/)

# 最后

劝你善良，内心平静，不刻意差评，不恶意差评。
