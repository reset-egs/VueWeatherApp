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

            <div class="weather-wrap">
                <div class="location-box">
                    <div class="location">
                        Copenhagen, Denmark
                    </div>
                    <div class="date">
                        28 September 2022
                    </div>
                </div>
            </div>

            <div class="weather-box">
                <div class="temp">10°C</div>
                <div class="weather">Overcast</div>
            </div>
        </main>
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@700&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: "Poppins", sans-serif;
}

#app {
    background-image: url("./assets/cold-bg.jpg");
    background-size: cover;
    background-position: center;
    transition: 0.4s;
}

main {
    min-height: 100vh;
    padding: 100px;
    background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25), rgba(0, 0, 0 , 0.75));
}

.search-box {
    width: 100%;
    margin-bottom: 30px;
}

.search-box .search-bar {
    display: block;
    width: 100%;
    padding: 15px;
    color: #313131;
    font-size: 20px;
    appearance: none;
    border: none;
    outline: none;
    background: none;
    background-color: rgba(255, 255, 255, 0.5);
    border-radius: 16px 16px 16px 16px;
}

.search-box .search-bar:focus {
    box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
    background-color: rgba(255, 255, 255, 0.75);
}

.location-box .location {
    color: rgb(218, 214, 214);
    font-size: 30px;
    font-weight: 500;
    text-align: center;
    text-shadow: 2px 2px rgba(0, 0, 0, 0.25);
}

.location-box .date {
    color: rgb(218, 214, 214);
    font-size: 20px;
    font-weight: 300;
    font-style: italic;
    text-align: center;
}

.weather-box {
    text-align: center;
}

.weather-box .temp {
    display: inline-block;
    padding: 10px 25px;
    color: rgb(218, 214, 214);
    font-size: 102px;
    font-weight: 900;
    text-shadow: 3px 6px rgba(0, 0, 0, 0.25);
    background-color: rgba(255, 255, 255, 0.25);
    border-radius: 16px 16px 16px 16px;
    margin: 30px 0px;
    box-shadow: 3px 6px rgba(0, 0, 0, 0.25);
}

.weather-box .weather {
    color: rgb(218, 214, 214);
    font-size: 50px;
    font-weight: 700px;
    text-shadow: 3px 6px rgba(0, 0, 0, 0.25);
}
</style>
