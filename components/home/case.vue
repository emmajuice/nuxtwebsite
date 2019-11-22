<template>
    <div class="case-box">
      <div class="case-items">
        <div class="case-item-l">

        </div>
        <div class="case-item-r">
         <p></p>
        </div>
      </div>
    </div>
</template>

<script>
    export default {
        name: "case"
    }
</script>

<style type="text/css" lang="scss" scoped>
.case-box{
  width: 1200px;
  margin: 5rem auto;
  .case-items{
    display: flex;
    width: 100%;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    .case-item-l{
      width: 40%;
      display: flex;
    }
    .case-item-r{
      width: 60%;
      display: flex;
    }
  }
}
</style>
