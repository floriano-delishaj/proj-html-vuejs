<template>
    <nav class="d-flex align-items-center justify-content-between p-5">
        <img src="../../public/img/theme_eduprime_logo.png" alt="">

        <div class="d-flex">
            <ul class="d-flex">
                <li v-for="(item, i) in navList" :key='i'>
                    <a href="#">
                        {{item}}
                    </a>
                </li>
            </ul>

            <div class="btn">
                VIEW COURSES
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    data () {
        return {
            navList: [
                'Home',
                'Courses',
                'About Us',
                'News',
                'Pages',
                'Contact',
                'Purchase',
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/navBar.scss';
</style>