<template>
	<div>
		<div class="nv-navbar">
			<ul class="nav">
				<font face="Arial, sans-serif">
            <li><router-link :to="{name: 'items'}"> รายละเอียดอัลบัมเพลง</router-link></li>  
            <li><router-link :to="{name: 'blogs'}"> การสั่งซื้ออัลบัมเพลง</router-link></li>
            <li><router-link :to="{name: 'comments'}"> Comment เพลง</router-link></li>
            <li><router-link :to="{name: 'users'}"> ผู้ใช้งาน</router-link></li>
            <li><router-link :to="{name: 'login'}"><i class="fa fa-user-o" aria-hidden="true"></i> Login</router-link></li>
            <li><a v-on:cick.prevent="logout" href="login"><i class="fa fa-sign-in" aria-hidden="true"></i> Logout</a></a></li>
            </font>
			</ul>
			<div class="clearfix" />
		</div>
	</div>
</template>
<script>
export default {};
</script>
<style scoped>
.nv-navbar {
	background-color: rgb(62, 12, 110);
	width: 100%;
	padding: 10px 0px 10px 0px;
}
.nv-navbar .nav {
	list-style: none;
	margin: 0;
	padding: 0;
	float: left;
}
.nv-navbar .nav li {
	float: left;
}
.nv-navbar .nav li a {
	padding: 10px;
	text-decoration: none;
	color: grey;
	font-weight: bold;
}
.nv-navbar .nav li a:hover {
	padding: 10px;
	text-decoration: none;
	color: darkslategrey;
}
.nv-navbar .nav li a.router-link-active {
	background-color: rgb(109, 109, 4);
	color: rgb(4, 26, 26);
}
.clearfix {
	clear: left;
}
</style>


<!-- <template>

    <div>
    
        <div class="nv-navbar"> 
            <div class="nva">
              
  
            </div>
            <font face="Arial, sans-serif">
            <a><router-link :to="{name: 'items'}"> รายละเอียดอัลบัมเพลง</router-link></a>  
            <a><router-link :to="{name: 'blogs'}"> การสั่งซื้ออัลบัมเพลง</router-link></a>
            <a><router-link :to="{name: 'comments'}"> Comment เพลง</router-link></a>
            <a><router-link :to="{name: 'users'}"> ผู้ใช้งาน</router-link></a>
            <a><router-link :to="{name: 'login'}"><i class="fa fa-user-o" aria-hidden="true"></i> Login</router-link></a>
            <a><a v-on:cick.prevent="logout" href="login"><i class="fa fa-sign-in" aria-hidden="true"></i> Logout</a></a>
            </font>
          
        </div>
      
    </div>
  
</template>

<script>
export default {
  methods: {
    logout () {
      this.$store.dispatch('setToken', null)
      this.$store.dispatch('setUser', null)
      this.$router.push({
        name: 'login'
      })
    }
  }
};
</script>

<script>
export default {};
</script>
<style scoped>
.nv-navbar {
	background-color: rgb(213, 20, 20);
	width: 100%;
	padding: 110px 0px 10px 0px;
}
.nv-navbar .nav {
	list-style: none;
	margin: 0;
	padding: 0;
	float: left;
}
.nv-navbar .nav li {
	float: left;
}
.nv-navbar .nav li a {
	padding: 10px;
	text-decoration: none;
	color: grey;
	font-weight: bold;
}
.nv-navbar .nav li a:hover {
	padding: 10px;
	text-decoration: none;
	color: darkslategrey;
}
.nv-navbar .nav li a.router-link-active {
	background-color: gold;
	color: darkslategrey;
}
.clearfix {
	clear: left;
}-->