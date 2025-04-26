<script>
  import Footer from "./Footer.svelte";
  import Header from "./Header.svelte";
  import news, {getNews} from "../../assets/news";

  export let params = {}

  let newsItem = getNews(Number(params.id))
</script>

<Header />
<main class="container">
  <div class="main-header">
    <h2>{newsItem.title}</h2>
    <p class="date">{newsItem.date}</p>
    <img src={newsItem.detailImgUrl} alt="" />
  </div>
  <article>
    {@html newsItem.desc}
  </article>
</main>
<Footer />

<style lang="scss">
  .main-header {
    h2 {
      margin-bottom: 10px;
    }
    .date {
      margin-bottom: 20px;
      font-size: 15px;
      color: #666;
    }
  }
  article {
    margin-top: 50px;
  }
</style>
