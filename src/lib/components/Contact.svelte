<script>
  import Footer from "./Footer.svelte";
  import Header from "./Header.svelte";
</script>

<Header />
<main class="container">
<h2>최고의 무대를 선사하겠습니다</h2>
<div class="contact">
  <figure class="map">
    <iframe src="https://www.google.com/maps/embed?pb=!1m17!1m12!1m3!1d12664.442966548211!2d127.00782240000002!3d37.481713!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m2!1m1!2s!5e0!3m2!1sko!2skr!4v1745664005929!5m2!1sko!2skr" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
  </figure>
  <address>
    <p>경기도 의정부시 범골로 123번길 11, 3층<br>빅브라더 스튜디오</p>
    <p>Email: 
      <a href="mailto:bbrother@gmail.com">bbrother@gmail.com</a></p>
    <p>Tel: 
      <a href="tel:031-000-0000">031-000-0000</a> / 
      <a href="tel:010-000-0000">010-000-0000</a>
     </p>
    <p>Fax: 031-000-0000</p>
  </address>
</div>
</main>
<Footer />

<style lang="scss">
  .contact {
    display: flex;
    gap: 75px;
    figure, address { width: 50%; }
    address { 
      font-style: normal; 
      p:not(:first-child) { margin-bottom: 5px; }
    }
    a { color: inherit; }
  }


</style>