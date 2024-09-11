<script setup lang="ts">
import { ref, toRefs } from 'vue'

interface IGroupDetail {
    created_at: string;
}
const props = defineProps<{
    groupDetail: Partial<IGroupDetail>
}>()

// const { groupDetail } = toRefs(props) // Comment this code，groupDetail in template will unknown 

</script>

<template>
  <div>  {{ groupDetail.created_at }}</div>
   <div>  {{ props.groupDetail.created_at }}</div>
</template>
