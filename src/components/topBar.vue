<template>
    <div>
        <nav class="topbar">
            <div class="topbar-center">
                <ul>
                    <li>
                        <a href="#home" class="link">
                            <span class="text">Home</span>
                        </a>
                    </li>
                    <li>
                        <a href="#who" class="link">
                            <span class="text">Our Program</span>
                        </a>
                    </li>
                    <li>
                        <a href="#location" class="link">
                            <span class="text">Location</span>
                        </a>
                    </li>
                </ul>
            </div>
        </nav>
    </div>
</template>

<style scoped>
.topbar {
    display: flex;
    justify-content: center;
    background: rgba(0, 0, 60, 0.3);
    width: 100%;
    text-align: center;
    position: fixed;
    top: 0;
    z-index: 100;
    padding: 1rem 0;
    border-bottom-left-radius: 15px;
    border-bottom-right-radius: 15px;
    backdrop-filter: blur(5px);
    -webkit-backdrop-filter: blur(10px);
}

.topbar-center {
    padding: 1rem;
    flex: 1;
    display: flex;
    justify-content: center;
}

.topbar-center ul {
    list-style: none;
    display: flex;
    justify-content: center;
    margin: 0;
    padding: 0;
}

.topbar-center ul li {
    margin: 0 1rem;
}

.topbar-center ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
    font-size: 20px;
    transition: color 0.3s ease;
}

.topbar-center ul li a:hover {
    color: #a10d04;
}


@media (max-width: 780px) {
    .topbar-center ul li a {
        font-size: 16px;
    }
}
</style>