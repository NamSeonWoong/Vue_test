<template>
    <div>
        <v-textarea
          outlined
          v-model="memo"
          label="투두리스트를 입력하시오"
          value=""
        ></v-textarea>
        <v-btn @click="listAdd">리스트 추가</v-btn>
    </div>
</template>>

<script>
export default {
    data()  {
        return {
            memo: null
        }
    },
    methods:    {
        listAdd()   {
            console.log("리스트 추가")
        }
    }
}
</script>>