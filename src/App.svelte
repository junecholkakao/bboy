<script>
  import Router, {location, link} from 'svelte-spa-router'
  import About from "./lib/components/About.svelte";
  import Home from "./lib/components/Home.svelte";
  import News from './lib/components/News.svelte';
  import Detail from './lib/components/Detail.svelte';
  import Contact from './lib/components/Contact.svelte';


</script>

<Router routes= {{
  '/': Home,
  '/about': About,
  '/news':News,
  '/detail/:id':Detail,
  '/contact': Contact
}}

/>
<style>

</style>
