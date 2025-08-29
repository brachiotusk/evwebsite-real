<script>
    import { base } from "$app/paths";
    import ExpandingHr from "../../lib/common/ExpandingHR.svelte";
    import PageWrapper from "../../lib/common/PageWrapper.svelte";
    import StatBox from "../../lib/common/StatBox.svelte";
    import Header from "../../lib/layout/Header.svelte";
</script>
<Header/>
<PageWrapper>
    <h1 class="text-3xl font-semibold">INTO THE DEEP</h1>
    <ExpandingHr --width=10em/>

    <h2 class="text-xl">Season Statistics</h2><br>
    <div class="flex flex-col md:flex-row w-full h-full md:w-2/3 justify-evenly align-middle content-center items-center">
      <StatBox number=176.87 truncateDecimals=2 duration=3000 statisticName="<small>(Top 1.5% Globally)</small>">OPR</StatBox>
        <div class="md:hidden"><ExpandingHr --width=15em/></div>
        <div class="w-0 h-16 hidden md:block border-white border-l-[2px]"></div>
        <StatBox number=200 truncateDecimals=0 duration=3000 statisticName="<small>teams in the world at the World Championship</small>">One of</StatBox>
        <div class="md:hidden"><ExpandingHr --width=15em/></div>
        <div class="w-0 h-16 hidden md:block border-white border-l-[2px]"></div>
          <StatBox number=42.66 truncateDecimals=0 duration=3000 statisticName="<small>(Top 1.5% Globally)</small>">Autonomous</StatBox>
    </div><br>
    <p>Our 2024-2025 INTO THE DEEP campaign went through two major robot builds, dozens of subsystem iterations, and many different minor tweaks and
     changes before becoming the robot you see today.</p><br>
    <h2 class="text-2xl font-semibold">Version 1</h2>
    <img src="{base}/itd1.jpg" class="max-h-[30em] mt-4" alt="The first iteration of the EV robot."><br>
    <p>Version 1: Our first robot utilized linkage driven pivoting slides, which allowed us to have precise control over the angle of the linear slides. We also used an active claw that was very effective at intaking samples with varying tolerance, depending on how open the claw was. This made it very good for reliably picking samples up from the ground while also selecting samples in the submersible. Combined with a camera, our robot was able to hit the first 6 sample autonomous in the world. We also used a power take off to power our level 3 climbing mechanism, leading to one of the fastest L3 ascents in the world (when it worked).</p>
    <h2 class="text-2xl font-semibold mt-4">Version 2</h2>
    <img src="{base}/itd2.jpg" class="max-h-[30em] mt-4" alt="The second iteration of the EV robot.">
    <p>Version 2: Upon our qualification for the World Championships, we began debating about the future of our robot and eventually we decided to bring V2 also known as Cosmic Crisp into this world. We decided to build V2 after experiencing many issues with our V1 robot, including the load on the pivot being too great for the linear slides, causing them to wear very quickly. Our power takeoff also suffered from reliability issues as the micro servos powering it literally started melting the plastic around it. Our V2 featured similar mechanisms to our V1, but with a much more robust linear rail for our pivot, and an active claw that could pick up from either the top or the side of the sample. However, with our limited time before worlds, the robot lacked testing and driver practice. Our autonomous was also absolutely chopped and we literally rewrote half of it the day before flying out to worlds. </p>
</PageWrapper>
