<template>
    <div class="Sidebar">
        <div class="Sidebar__MenuIcon">
            <div class="Sidebar__MenuIcon_Icon">
                <div class="whiteLine" />
                <div class="whiteLine" />
            </div>
        </div>
        <NuxtLink to="/" class="Sidebar__MenuOptions">
            <img src="/img/home.png" alt="">
        </NuxtLink>
        <div class="Sidebar__NewTaskContainer">
            <NuxtLink to="/newTask" class="Sidebar__NewTaskContainer__Button">
                    <img src="/img/plus.png" alt="">
            </NuxtLink>
        </div>
    </div>
</template>
<style>
.Sidebar {
    background-color: #2e3034;
    width: 5rem;
    height: calc(100vh - 7rem);
    border-radius: 1rem;
}

.Sidebar__MenuIcon {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 6rem;
}

.Sidebar__MenuIcon_Icon {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 70%;
    height: 100%;
    row-gap: 0.5rem;
    border-bottom: 1px solid #bebebe
}

.whiteLine {
    width: 60%;
    height: 0.15rem;
    border-radius: 1rem;
    background-color: white;
}

.Sidebar__MenuOptions {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 6rem;
}

.Sidebar__MenuOptions>img {
    width: 2.5rem;
    height: 2.5rem;
}

.Sidebar__NewTaskContainer {
    width: 100%;
    height: 5rem;
    display: flex;
    justify-content: center;
    align-items: center;
}

.Sidebar__NewTaskContainer__Button {
    width: 70%;
    height: 3.5rem;
    background-color: #2c55dc;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 1rem;
}

.Sidebar__NewTaskContainer__Button>img {
    width: 50%;
    filter: invert(100%);
}
@media screen and (max-height: 800px) {
    .Sidebar{
        height: 43rem;
    }
    
}
</style>
