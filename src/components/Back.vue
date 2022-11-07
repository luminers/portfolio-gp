<template>
  <div class="div-content back">
    <div class="icon-label">
      <img
        class="icon"
        src="https://seeklogo.com/images/C/c-sharp-c-logo-02F17714BA-seeklogo.com.png"
        alt="C#"
      />
      <p>C#</p>
    </div>
    <div class="icon-label">
      <img
        class="icon"
        src="https://mvpcluster.com/wp-content/uploads/2016/04/sql-server-1.png"
        alt="SQL server"
      />
      <p>SQL Server</p>
    </div>
    <div class="icon-label">
      <img
        class="icon"
        src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ee/.NET_Core_Logo.svg/1200px-.NET_Core_Logo.svg.png"
        alt="SQL server"
      />
      <p>.NET CORE</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "BackComponente",
};
</script>

<style>
.back {
  width: 30%;
  margin: 0px 10px 0 0;
}
</style>

<style scoped>
.div-content {
  justify-content: space-evenly;
}
</style>
