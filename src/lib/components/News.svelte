<script>
  import Footer from "./Footer.svelte";
  import Header from "./Header.svelte";
  import news from "../../assets/news";
</script>

<Header />
<main class="container">
  <h2>비보이 브라더스 활동</h2>

  <div class="news">
    {#each news as item}
    <a href={"#/detail/"+item.id}>

      <div class="news-item">
        <img src={item.imgUrl} alt="1" />
        <div class="text-info">
          <h3>{item.title}</h3>
          <p class="date">{item.date}</p>
          <div class="hashtag">
            {#each item.hashtag as tag}
            <span>#{tag}&nbsp;</span>
            {/each}
          </div>
        </div>
      </div>
    </a>
    {/each}
  </div>
</main>
<Footer />

<style lang="scss">
  .news {
    display: flex;
    gap: 20px;
    .news-item {
      
      img {
        width: 100%;
      }
      h3 {margin-bottom: 10px;}
      p {margin-bottom: 4px;}
      .date, .hashtag {
        font-size: 15px;
        color: #666;
      }
      box-shadow: 4px 4px 10px rgba(0,0,0,0.2);
      .text-info {
        padding: 20px;
      }
    }
    a {
      color: inherit;
      text-decoration: none;
      width: calc(100%/3);
    }
  }
</style>
