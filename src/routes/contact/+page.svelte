<script>
    import ExpandingHr from "../../lib/common/ExpandingHR.svelte";
    import Header from "../../lib/layout/Header.svelte";
    import PageWrapper from "../../lib/common/PageWrapper.svelte";
    import animateTyping from "../lib/common/animateTyping";

</script>
<Header/>

<style>
  @keyframes rainbow {
    0%   { filter: hue-rotate(0deg); }
    100% { filter: hue-rotate(360deg); }
  }

  .rainbow {
    display: inline-block;      /* needed for filter */
    animation: rainbow 3s linear infinite;
  }
</style>

<PageWrapper>
    <h1 class = "text-4xl font-bold">
        Contact Us!
    </h1>
    <ExpandingHr --width=10em/>
    <ul>
        <li>Email: <a href="mailto:escapevelocityweb@gmail.com" class="text-evyellow underline">escapevelocityweb@gmail.com</a></li>
        <li>Instagram: <a href="https://www.instagram.com/ftcescapevelocity14343/" class="text-evyellow underline">@ftcescapevelocity14343</a></li>
        <p> Phone: (425)-324-7617</p>
    </ul>
    
</PageWrapper>
