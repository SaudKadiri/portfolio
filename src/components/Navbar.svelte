<script>
    export let fields
</script>

<body>
    <nav class="navbar">
      <!-- LOGO -->
      <div class="logo">saud kadiri</div>
      <!-- NAVIGATION MENU -->
      <ul class="nav-links">
        <!-- USING CHECKBOX HACK -->
        <input type="checkbox" id="checkbox_toggle" />
        <label for="checkbox_toggle" class="hamburger">&#9776;</label>
        <!-- NAVIGATION MENUS -->
        <div class="menu">
            {#each fields as field}
                <li><a href="#{field.id}">{field.title}</a></li>
            {/each}
        </div>
      </ul>
    </nav>
</body>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Splash&display=swap');
    body>nav {
        font-family: cursive;
    }
    a {
        text-decoration: none;
    }
    li {
        list-style: none;
    }

    /* NAVBAR STYLING STARTS */
    .navbar {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 20px;
        background-image: linear-gradient(to left top, #780044, #5b1247, #3f1842, #261836, #151425, #121424, #0f1323, #0c1321, #0b1a32, #082144, #042856, #002e69);
        color: #fff;
    }
    .nav-links a {
        font-weight: bolder;
        color: white;
    }
    a:hover {
        color: lavender;
    }
    /* LOGO */
    .logo {
        color:royalblue;
        text-shadow: 1px 1px khaki;
        font-size: 34px;
        font-weight: 900;
        font-family: 'Splash', cursive;
    }
    /* NAVBAR MENU */
    .menu {
        display: flex;
        gap: 1em;
        font-size: 1.5vmax;
    }
    .menu li:hover {
        box-shadow: 1px 1px lavender;
        background-color:#0b1a32;
        background-image: linear-gradient(to right top, #d16ba5, #c777b9, #ba83ca, #aa8fd8, #9a9ae1, #8aa7ec, #79b3f4, #69bff8, #52cffe, #41dfff, #46eefa, #5ffbf1);
        border-radius: 5px;
        transition: 0.3s ease;
    }
    .menu li {
        padding: 5px 14px;
    }

    /*RESPONSIVE NAVBAR MENU STARTS*/
    /* CHECKBOX HACK */
    input[type=checkbox]{
        display: none;
    } 
    /*HAMBURGER MENU*/
    .hamburger {
        display: none;
        font-size: 24px;
        user-select: none;
    }
    /* APPLYING MEDIA QUERIES */
    @media (max-width: 768px) {
        .menu { 
            display:none;
            right: 0;
            left: 0;
            text-align: center;
            padding: 16px 0;
        }
        .menu li + li {
            margin-top: 12px;
        }
        input[type=checkbox]:checked ~ .menu{
            display: block;
        }
        .hamburger {
            display: block;
        }
    }
</style>
