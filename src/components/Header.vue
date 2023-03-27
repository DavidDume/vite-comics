<template>

    <nav>
        <ul>
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