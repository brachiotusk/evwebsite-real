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
    <p>Version 1</p>
    <h2 class="text-2xl font-semibold mt-4">Version 2</h2>
    <img src="{base}/itd2.jpg" class="max-h-[30em] mt-4" alt="The second iteration of the EV robot.">
    <p>Version 2 </p>
</PageWrapper>
