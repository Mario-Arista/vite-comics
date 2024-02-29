<script>

export default {
    name: 'AppNav',

    data() {
        return {
            links: [
                "Characters",
                "Comics",
                "Movies",
                "Tv", 
                "Games",
                "Collectibles",
                "Videos",
                "Fans",
                "News", 
                "Shop"
            ],

            activeIndex: 1,

        }
    }
}

</script>

<template>
  
    <nav>

        <img src="../assets/img/dc-logo.png" alt="logo DC">
        <ul>
            <li 
                v-for="(Currentlink, index) in links"
                :class="index == activeIndex ? 'active' : '' "
            >
                {{ Currentlink }}
            </li>
        </ul>

    </nav>
  
</template>

<style lang="scss">

@use '../styles/general.scss' as *;

nav {

    display: flex;
    justify-content: space-between;
    align-items: center;

    max-width: 1200px;

    margin: 0 auto;

    background-color: #FFFFFF;

    img {
        width: 70px;
        height: auto;
    }

    ul {
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        gap: 30px;
        flex-grow: 1;

        list-style-type: none;
        
        margin: 0px;
        padding: 0px;

        color: $sec_color;

        li {
            

            padding-top: 45px;
            padding-bottom: 45px;
            text-transform: uppercase;
            font-size: 0.6em;
            font-weight: 400;
        }

    }

    ul li.active {
        border-bottom: $primary_color 4px solid;
    }
}

</style>