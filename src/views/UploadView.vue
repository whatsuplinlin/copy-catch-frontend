<template>
  <div class="course">
    <div class="coursedetail">{{ GStore.detail.course_id }}</div>
    <div class="coursedetail">{{ GStore.detail.course_name }}</div>
    <div class="coursedetail">{{ GStore.detail.year }}</div>
    <div class="coursedetail">{{ GStore.detail.examination }}</div>
  </div>

  <DragDrop></DragDrop>
</template>
<script>
import DragDrop from '@/components/DragDropZip.vue'
export default {
  inject: ['GStore'],
  components: {
    DragDrop
  }
}
</script>
<style scoped>
.course {
  margin: 30px 0;
}

.coursedetail {
  font-size: 20px;
  display: inline;
  padding: 0 20px;
  font-weight: bold;
}
</style>
