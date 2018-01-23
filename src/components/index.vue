<template>
  <div>
    <div align="right" style="margin-top: 30px">
      <mo-pagination
        :page-index="currentPage"
        :total="count"
        :page-size="pageSize"
        @change="pageChange">
      </mo-pagination>
    </div>
  </div>
</template>
<script>
import moPagination from './pagination.vue'
export default {
  components: {moPagination},
  data () {
    return {
      pageSize: 3, // 每页显示20条数据
      currentPage: 1, // 当前页码
      count: 10 // 总记录数,
    }
  },
  methods: {
    getList () {},
    pageChange (index) {
      this.currentPage = index
      this.getList()
    }
  }
}
</script>
<style scoped></style>
