<template>
    <div>
        <ul class="icons-list">
            <li v-for="icon in icons" class="icon-links">
                <img :src="getImg(icon.path)" alt="">
                <a href="#">{{ icon.name }}</a>
            </li>
        </ul>
    </div>
</template>

<styles scoped lang="scss">
    .icons-list {
        list-style: none;
        display: flex;
        justify-content: center;
        align-items: center;
        img {
            width: 70px;
            height: 70px;
            margin-right: 10px;
        }
        .icon-links {
            display: flex;
            align-items: center;
            margin: 0 10px;
            a {
                color: white;
                text-decoration: none;
            }
        }
    }

</styles>

<script>

export default {

    data() {
        return {
            icons: [
                {
                    path: '../assets/buy-comics-digital-comics.png',
                    name: 'DIGITAL COMICS'
                },
                {
                    path: '../assets/buy-comics-merchandise.png',
                    name: 'DC MERCHANDISE'
                },
                {
                    path: '../assets/buy-comics-subscriptions.png',
                    name: 'SUBSCRIPTION'
                },
                {
                    path: '../assets/buy-comics-shop-locator.png',
                    name: 'COMIC SHOP LOCATION'
                },
                {
                    path: '../assets/buy-dc-power-visa.svg',
                    name: 'DC POWER VISA'
                },
                
            ]
        }
    }, 
    methods: {
        getImg: function(url) {
            return new URL(url, import.meta.url).href;
        }
    }
}

</script>