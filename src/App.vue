<script>
export default {
    name: "App",
    data() {
        return {
            api_key: "30ccec678e579ca698bc043babf9ed4d"
        };
    },
    methods: {

    }
};
</script>

<template>
    <div id="app">
        <main>
            <div class="search-box">
                <input type="text" class="search-bar" placeholder="Enter location"/>
            </div>
        </main>
    </div>
</template>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: "montserrat", sans-serif;
}

#app {
    background-image: url("./assets/cold-bg.jpg");
    background-size: cover;
    background-position: center;
    transition: 0.4s;
}

main {
    min-height: 100vh;
    background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25), rgba(0, 0, 0 , 0.75));
}
</style>
