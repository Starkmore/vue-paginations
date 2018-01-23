# paginations

> 分页组件
#
##
``` bash
功能点：
# 1.点击页面序号可以跳转到相应页面。\<br>
# 2.点击上一页或者下一页可以跳转页面，当页面在第一页时上一页无法点击，页面在最后一页时下一页无法点击。\<br>
# 3.一次显示当前页面的前两页和后两页\<br>
# 4.当当前页面的序号和第一页与最后一页相差三个以上时出现省略号\<br>
# 5.始终显示第一页和最后一页，只有一页的时候显示一页\<br>
# 在父组件中使用\<br>
# 1.引入子组件
import MoPaging  from '../../components/pagination.vue' \<br>
export default { \<br>
  components:{ \<br>
    MoPaging  \<br>
  },
# 2.在模板（template）中插入子组件，使用时参数是从子组件props \<br>
<div align="right" style="margin-top: 30px"> \<br>
  <mo-paging     \<br>
    :page-index="currentPage"   \<br>
    :total="count"     \<br>
    :page-size="pageSize"   \<br>
    @change="pageChange">   \<br>
  </mo-paging>  \<br>
</div>
```

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
