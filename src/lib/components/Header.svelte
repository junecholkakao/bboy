<header>
  <div class="logo">
    <a href="/">
      <img src="images/logo.png" alt="logo">
    </a>
  </div>
  <nav>
    <ul>
      <li><a href="#/">home</a></li>
      <li><a href="#/about">about</a></li>
      <li><a href="#/news">news</a></li>
      <li><a href="#/contact">contact</a></li>
    </ul>
  </nav>
</header>

<style lang="scss">
  header {
    text-align: center;
    padding: 25px;
    .logo {
      margin-bottom: 15px;
    }
    nav ul {
      list-style-type: none;
      li {
        display: inline-block;
        margin: 0 1em;
        a {
          text-decoration: none;
          color: #333;
          &:hover {
            opacity: 0.7;
          }
        }
      }
    }
  }
</style>