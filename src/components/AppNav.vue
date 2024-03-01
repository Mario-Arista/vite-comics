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
        <div class="container">
            <img src="/img/dc-logo.png" alt="logo DC">
            <ul>
                <li 
                    v-for="(Currentlink, index) in links"
                    :class="index == activeIndex ? 'active' : '' "
                >
                    {{ Currentlink }}
                </li>
            </ul>
        </div>
    </nav>
  
</template>

<style lang="scss">

@use '../styles/variables.scss' as *;

nav {
    background-color: #FFFFFF;
    width: 100%;

    .container {

        justify-content: space-between;
  
        img {
            width: 70px;
            height: auto;
        }

        ul {
            display: flex;
            flex-direction: row;
            justify-content: flex-end;
            flex-wrap: wrap;
            gap: 30px;
            flex-grow: 1;

            list-style-type: none;
    

            color: $sec_color;

            li {
            

                padding-top: 45px;
                padding-bottom: 45px;
                text-transform: uppercase;
                font-size: 0.7em;
                font-weight: 400;
            }

        }

        ul li.active {
            border-bottom: $primary_color 4px solid;
        }
    }

}

@media screen and (max-width: 992px) {
    nav .container {
        padding: 10px 5px;
        ul {
            gap: 10px;

            li {
            
                padding-top: 10px;
                padding-bottom: 10px;
    
            }

        }
    }    
}

@media screen and (max-width: 576px) {
    nav .container ul {
        display: none;
    }
}

</style>