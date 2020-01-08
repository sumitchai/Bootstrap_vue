<template>
  <div id="app">
    <div id="nav">      
      
      <div>
        <b-navbar>
          <router-link to="/">
            <b-nav class="navbar navbar-expand beta-menu navbar-dropdown align-items-center navbar-fixed-top navbar-toggleable-sm">
              <img src="./assets/up-122x122.png" style="height: 5.8rem;">
            </b-nav>
          </router-link> 
          

          <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

          <b-collapse id="nav-collapse" is-nav>
            
            <!-- Right aligned nav items -->
            <b-navbar-nav class="ml-auto">
              <b-nav>
                <router-link to="/">
                  <b-nav-item active>หน้าแรก</b-nav-item>
                </router-link>
              </b-nav>


              <b-nav-item-dropdown text="Lang" right>
                <b-dropdown-item href="#">EN</b-dropdown-item>
                <b-dropdown-item href="#">ES</b-dropdown-item>
                <b-dropdown-item href="#">RU</b-dropdown-item>
                <b-dropdown-item href="#">FA</b-dropdown-item>
              </b-nav-item-dropdown>

              <div>
                <b-button v-b-modal.modal-1>ติดต่อเรา</b-button>

                <b-modal id="modal-1" title="กองบริการการศึกษา : มหาวิทยาลัยพะเยา">
                  <a class="my-4"><b>งานทะเบียนนิสิตและประมวลผล</b></a><br>
                  <a> 19 หมู่ 2 ตำบลแ่กา อำเภอเมือง จังหวัดพะเยา รหัสไปรษณีย์ 56000</a><br>
                  <a>โทรศัพท์:  054466666 </a>
                </b-modal>
              </div>
            </b-navbar-nav>
          </b-collapse>
        </b-navbar>
      </div>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
