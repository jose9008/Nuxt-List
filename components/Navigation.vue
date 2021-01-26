<template>
    <header class="header">
        <h1> Post App</h1>
        <nav>
            <ul>
                <li>
                   <nuxt-link to="/"> Home </nuxt-link>
                </li>
                <li>
                   <nuxt-link to="/posts"> Post </nuxt-link>
                </li> 
                <li>
                   <nuxt-link to="/about"> About </nuxt-link>
                </li> 
            </ul>
        </nav>
    </header>
</template>

<style>
.header {
    background: #2c3e50;
    color: #ffffff;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 3rem;
    border-bottom: 1px solid #2ecc71;
}

.header ul {
    display: flex;
    list-style: none;
}

.header a {
    color: #ffffff;
    background: #2d3436;
    padding: .3rem 1rem;
    text-decoration: none;
    text-transform: uppercase;
}

.header a:hover {
    background: #2c3e50;
    border: 1px solid rgba(118, 233, 11, 0.333);
}


</style>