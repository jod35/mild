<template>
    <section class="side-bar">
        <div class="sidebar-contents">
            <a href="#">Create New Record</a>
            <a href="#">Create New Account</a>
            <a href="#">Sign In</a>
        </div>
    </section>
</template>

<script>
export default {
    name:"SideBar"
}
</script>
<style>
  .side-bar{
      width: 20%;
      background-color:rgb(97, 139, 34);
  }
  .sidebar-contents{
      display: block;
      margin-top: 100px;
      position: fixed;
      flex-direction: row;
  }
  .sidebar-contents a{
      display: block;
      padding: 20px;
      width: 100%;
      color: white;
      transition: all 1.2s;
  }
  .sidebar-contents a:hover{
      margin-left: 5px;
      padding: 20px;
      background-color: rgb(54, 80, 15);
      border-top-right-radius: 30px;
      border-bottom-right-radius: 30px;
  }
</style>