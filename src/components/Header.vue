<template>

    <nav>
        <a href="#">
            <img src="../assets/dc-logo.png" alt="#">
        </a>
        
        <ul class="list">
            <li v-for="(link, i) in navLinks">
                <a :href="link.href">{{ link.title }}</a>
            </li>
        </ul>
    </nav>

</template>

<script>

export default {
    data() {
        return {
            navLinks: [
                {
                    title: 'CHARACTERS',
                    href: '#'
                },
                {
                    title: 'COMICS',
                    href: '#'
                },
                {
                    title: 'MOVIES',
                    href: '#'
                },
                {
                    title: 'TV',
                    href: '#'
                },
                {
                    title: 'GAMES',
                    href: '#'
                },
                {
                    title: 'COLLECTIBLES',
                    href: '#'
                },
                {
                    title: 'VIDEOS',
                    href: '#'
                },
                {
                    title: 'FANS',
                    href: '#'
                },
                {
                    title: 'NEWS',
                    href: '#'
                },
                {
                    title: 'SHOP',
                    href: '#'
                },
            ]
        }
    }
}

</script>


<style scoped lang="scss">
@use '../styles/variables';
    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .list {
            display: flex;
            list-style: none;
            li {
                padding: 5px;
            }

            a{
                text-decoration: none;
                color: black;
                &:hover {
                    color: variables.$primary;
                    border-bottom: 3px solid variables.$primary;
                    padding-bottom: 30px;
                }
            }
        }
    }
</style>