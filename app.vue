


<template>
    <div>

        <div class="headera">
            <div class="logo">
                logo
            </div>
            <div class="menu">
                <div class="menu0  activa">menu0</div>
                <div class="menu0 activa">menu1</div>
                <div class="menu0 activa">menu2</div>
                <div class="menu0 activa">menu3</div>
            </div>
            <div class="searcha"><input type="text" name="searcha" id="searcha"></div>
            <div class="logina">Log In</div>
            <div class="menuburger">burger</div>
            
        </div>
        <div class="menu-burger">
            <div class="fermer-carda-mini">fermer</div>

            <div class="menu-menu">
                <div class="menu-menu0  activa">menu0</div>
                <div class="menu-menu0 activa">menu1</div>
                <div class="menu-menu0 activa">menu2</div>
                <div class="menu-menu0 activa">menu3</div>
            </div>
        </div>
    </div>
</template>

<style>
.headera {
    padding: 12px 0 12px 0;
    margin: 0 5% 0 5%;

    display: grid;
    grid-template-columns: 1fr 1fr max-content max-content;
}

.menu {

    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(max-content, 1fr));
    grid-auto-flow: column;
    justify-items: center;
}

.logina {
    margin-left: 16px;
}

.menu0 {
    position: relative;
    opacity: 0.6;
    transition: all 0.2s ease-in-out;
    display: grid;
    justify-content: center;
    justify-items: center;
}

.menu0,
.logina,
.logo,
.menu-burger {
    cursor: pointer;

}

.menu0:hover {
    opacity: 1;

}

.searcha {
    display: grid;
}

#searcha {
    display: grid;
    width: 70%;
    justify-self: center;
}

.activa {
    padding: 0px;
}

.activa:hover {}

.activa::before {
    content: "";
    position: absolute;
    height: 2px;
    width: 0px;
    background-color: saddlebrown;
    transform: translateY(5px);
    bottom: 0;
    transform-origin: center center;
    transition: all 0.4s cubic-bezier(1, 0.01, 0.2, 1.01);
}

.activa:hover::before {

    height: 2px;
    width: 100%;

}

.menu-burger {
    display: none;
    position: relative;

}

.menu-burger {
    border: 1px solid black;
    padding: 16px;
    justify-content: center;
    display: grid;
    justify-items: center;
    display: grid;


}

.menu-menu {
    position: relative;
    margin-bottom: 0px;
    display: grid;
    justify-items: center;
    justify-self: center;

}

.menu-menu0 {

    position: relative;
    margin: 8px;
}

.fermer-carda-mini {
    position: absolute;
    top: 0;
    right: 0;
}

.menuburger {
    display: none;
    cursor: pointer;
    margin-left: 8px;
}
.menu-burger {
    display: none;

}

/*****responsive xD */

@media screen and (max-width: 870px) {
    .menu {
        display: none;
    }
    .menuburger{
        display: initial;
    }
    .menu-burger {
        display: initial;
        position: absolute;
        border: 1px solid black;
        padding: 16px;
        top: 0;
        right: 0;
        background: white;
        width: 100%;
        justify-content: center;
        display: grid;
        justify-items: center;
        display: grid;
    }
}


/*******fin respo xD */
</style>
