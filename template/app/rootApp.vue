<template>
    <div id="root">
        <ul class="header">
            <li>
                <router-link :to="{ path: '/home' }" class="nav-link">HOME</router-link>
            </li>
            <li>
                <router-link :to="{ path: '/about' }" class="nav-link">ABOUT</router-link>
            </li>
        </ul>

        <router-view></router-view>
    </div>
</template>

<script>
export default {
}
</script>

<style scoped>
#root{
    font-family: 'Source Sans Pro', 'Helvetica Neue', Arial, sans-serif;
    box-sizing: border-box;
}

a{
    text-decoration: none;
    color: #2E64FE;
}

.header {
    list-style-type: none;
    text-align: center;
    padding: 0;
    margin: 0;
}

.header li {
    display: inline-block;
    line-height: 40px;
}

.nav-link {
    color: #7f8c8d;
    cursor: pointer;
    text-decoration: none;
    padding-bottom: 3px;
    margin: 0 25px;
}

.nav-link.router-link-active {
    color: #000;
}

.nav-link:first-child {
    margin-left: 0;
}

.nav-link:hover {
  border-bottom: 3px solid #42b983;
}
</style>
