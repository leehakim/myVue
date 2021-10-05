<template>
    <div class="sidebar">
        <div class="photo">

        </div>
        <nav>
            <a v-for="menu in menus" :key="menu">{{ menu }}</a>
        </nav>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                menus: ["Welcom", "About", "Works", "Contact Me"],
            }
        }
    }
</script>

<style lang="scss" scoped>
    .sidebar {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width:300px;
    }
    .photo {
        width: 210px;
        height: 210px;
        background-color: #ddd;
        border: 2px solid #000;
        border-radius: 50%;
    }
    nav {
        margin-top: 2rem;
        a {
            display: block;
            width: 210px;
            margin-bottom: 1.5rem;
            background-color: #fff;
            border: 2px solid #000;
            border-radius: 1rem;
            font-size: 1.5rem;
            line-height: 3.75rem;
        }
    }
</style>