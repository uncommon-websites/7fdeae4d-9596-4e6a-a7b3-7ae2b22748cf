<script>
  import { onMount } from 'svelte';

  const images = [
    "/generated/image-passionate-football-fans-celebrating-in--1765987877113-0.webp", // Fans celebrating
    "/generated/image-close-up-of-a-fans-hand-holding-a-smartp-1765987895176-1.webp", // Fan with phone
    "/generated/image-football-player-celebrating-a-goal-with--1765987912989-2.webp", // Player celebrating
    "/generated/image-wide-shot-of-a-modern-football-stadium-a-1765987924169-3.webp", // Stadium at night
    "/generated/image-young-diverse-group-of-friends-watching--1765987941397-4.webp"  // Friends watching
  ];

  let showCookieBanner = $state(true);
</script>

<div class="font-sans text-[#111] antialiased bg-white selection:bg-black selection:text-white">
  <!-- Header -->
  <header class="fixed top-0 left-0 w-full z-50 flex justify-between items-center px-6 py-5 bg-white/90 backdrop-blur-sm">
    <div class="text-xl font-medium tracking-tight">FanLayer</div>
    <nav class="hidden md:flex items-center gap-8 text-sm font-medium">
      <a href="#" class="hover:opacity-70 transition-opacity">Platform</a>
      <a href="#" class="hover:opacity-70 transition-opacity">For Clubs</a>
      <a href="#" class="hover:opacity-70 transition-opacity">For Fans</a>
      <a href="#" class="hover:opacity-70 transition-opacity">Blog</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="pt-40 pb-20 px-6 max-w-[1400px] mx-auto">
    <div class="max-w-4xl mb-24">
      <h1 class="text-6xl md:text-7xl font-medium tracking-tight leading-[1.1] mb-8">
        ChatGPT for Sports.<br>Your AI fan companion.
      </h1>
      <div class="flex flex-col md:flex-row justify-between items-start md:items-end gap-8">
        <p class="text-lg md:text-xl max-w-md leading-relaxed text-gray-800">
          Transform fragmented sports experiences into personalized AI conversations. Monetize fan data while delivering the engagement fans crave.
        </p>
        <button class="bg-black text-white px-6 py-3 text-sm font-medium rounded-sm hover:bg-gray-800 transition-colors">
          Request demo
        </button>
      </div>
    </div>

    <!-- Hero Images Grid -->
    <div class="grid grid-cols-2 md:grid-cols-5 gap-4">
      {#each images as src, i}
        <div class="aspect-[3/4] overflow-hidden bg-gray-100 rounded-sm">
          <img {src} alt="Sports fan experience {i}" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
        </div>
      {/each}
    </div>
  </section>

  <!-- Floating Images Section -->
  <section class="py-32 px-6 max-w-[1400px] mx-auto relative min-h-[800px]">
    <div class="absolute inset-0 flex items-center justify-center pointer-events-none z-10">
      <h2 class="text-2xl md:text-3xl font-medium text-center max-w-2xl leading-snug bg-white/80 backdrop-blur-sm p-4 rounded-xl">
        One AI conversation replaces 10+ apps. Give fans the unified experience they deserve.
      </h2>
    </div>

    <!-- Scattered Images with interactive elements -->
    <div class="relative w-full h-full min-h-[800px]">
      <!-- Image 1: Fan with jersey (Left) -->
      <div class="absolute top-20 left-[10%] w-64 aspect-[3/4]">
        <img src="/generated/image-fan-wearing-team-jersey-using-smartphone-1765987951685-5.webp" alt="Fan with smartphone" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <div class="w-3 h-3 bg-white rounded-full mx-auto mb-2 animate-pulse"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">Ask AI</button>
        </div>
      </div>

      <!-- Image 2: Stadium aerial (Center Top) -->
      <div class="absolute top-0 left-[45%] w-56 aspect-video">
        <img src="/generated/image-aerial-view-of-a-football-stadium-during-1765987956566-6.webp" alt="Stadium aerial view" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/3 left-1/3">
             <div class="w-3 h-3 bg-white rounded-full mb-2 animate-pulse"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">Live Stats</button>
        </div>
      </div>

       <!-- Image 3: Analytics dashboard (Right Top) -->
      <div class="absolute top-40 right-[5%] w-80 aspect-video">
        <img src="/generated/image-sports-analytics-dashboard-on-a-laptop-s-1765987968443-8.webp" alt="Analytics dashboard" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute bottom-1/3 right-1/3">
             <div class="w-3 h-3 bg-white rounded-full mb-2 animate-pulse ml-auto"></div>
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">Get Insights</button>
        </div>
      </div>

      <!-- Image 4: Excited fans (Left Bottom) -->
      <div class="absolute bottom-20 left-[5%] w-56 aspect-[3/4]">
        <img src="/generated/image-close-up-of-excited-fans-faces-painted-i-1765987962997-7.webp" alt="Excited fans" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">Match Updates</button>
        </div>
      </div>

      <!-- Image 5: Fans with phones (Center Bottom) -->
      <div class="absolute bottom-0 left-[35%] w-48 aspect-[3/4]">
        <img src="/generated/image-football-fans-in-stadium-seats-checking--1765987976093-9.webp" alt="Fans checking phones" class="w-full h-full object-cover rounded-sm shadow-lg" />
        <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
             <button class="bg-white/90 backdrop-blur text-xs px-3 py-1.5 rounded-full shadow-sm whitespace-nowrap hover:bg-white transition-colors">Team News</button>
        </div>
      </div>
    </div>
  </section>

  <!-- Dark Section 1: Natural Language -->
  <section class="bg-[#111] text-white py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-8">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight max-w-xl">
          Ask anything.<br>Get instant answers.
        </h2>
        <p class="text-gray-400 text-lg max-w-md leading-relaxed">
          Fans ask questions in their own words. FanLayer delivers real-time insights powered by exclusive rights holder data and AI.
        </p>
      </div>

      <!-- Interactive Box -->
      <div class="w-full aspect-video bg-[#1a1a1a] rounded-sm mb-16 flex items-center justify-center relative overflow-hidden group">
        <div class="text-4xl md:text-6xl font-light tracking-tight text-white/90">
          Who scored in the last<span class="animate-pulse">|</span>
        </div>
        <!-- Subtle grid or gradient could go here -->
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-12 border-t border-white/10 pt-12">
        <div>
          <h3 class="text-lg font-medium mb-3">Natural conversation</h3>
          <p class="text-gray-400 leading-relaxed">Fans ask questions like they would a friend.</p>
        </div>
        <div>
          <h3 class="text-lg font-medium mb-3">Real-time intelligence</h3>
          <p class="text-gray-400 leading-relaxed">Live match insights, injury updates, lineup predictions.</p>
        </div>
        <div>
          <h3 class="text-lg font-medium mb-3">Personalized for each fan</h3>
          <p class="text-gray-400 leading-relaxed">Tailored responses based on team loyalty and preferences.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Dark Section 2: Connect Catalog -->
  <section class="bg-[#111] text-white py-32 px-6 border-t border-white/5">
    <div class="max-w-[1400px] mx-auto">
      <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-8">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight">
          Monetize your<br>fan data goldmine
        </h2>
        <p class="text-gray-400 text-lg max-w-md leading-relaxed">
          Rights holders sit on valuable content and data they can't monetize. FanLayer unlocks digital revenue while deepening fan relationships.
        </p>
      </div>

      <!-- Interactive Box -->
      <div class="w-full aspect-[2/1] bg-[#1a1a1a] rounded-sm flex items-center justify-center">
         <div class="text-4xl md:text-6xl font-light tracking-tight text-white/90">
          Show me team tactic<span class="animate-pulse">|</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Light Gray Section -->
  <section class="bg-[#f5f5f5] py-24 px-6">
    <div class="max-w-[1400px] mx-auto grid grid-cols-1 md:grid-cols-3 gap-12">
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">Own fan relationships</h3>
        <p class="text-gray-600 leading-relaxed">Direct connections instead of relying on social platforms as intermediaries.</p>
      </div>
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">Unlock revenue streams</h3>
        <p class="text-gray-600 leading-relaxed">B2C subscriptions, B2B licensing, and sponsored AI interactions.</p>
      </div>
      <div>
        <h3 class="text-lg font-medium mb-3 text-[#111]">Engage fans 24/7</h3>
        <p class="text-gray-600 leading-relaxed">AI-powered conversations that never sleep, in multiple languages.</p>
      </div>
    </div>
  </section>

  <!-- Built for Sports Fans -->
  <section class="bg-[#f0f0f0] py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <div class="mb-16">
        <h2 class="text-4xl md:text-5xl font-medium tracking-tight mb-6 text-[#111]">
          Built for the AI era of sports
        </h2>
        <p class="text-gray-600 text-lg max-w-2xl leading-relaxed">
          FanLayer combines exclusive rights holder data with AI-native generation to create personalized experiences that transform how fans engage with their favorite teams.
        </p>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
        <!-- Visual -->
        <div class="bg-[#111] aspect-video rounded-xl flex items-center justify-center relative overflow-hidden perspective-1000">
           <!-- Abstract Wireframe Animation -->
           <div class="relative w-64 h-40 flex items-center justify-center transform-style-3d">
              {#each [0, 1, 2, 3, 4] as i}
                <div 
                  class="absolute w-32 h-48 border border-white/30 bg-white/5 backdrop-blur-sm rounded-sm transition-transform duration-500"
                  style="
                    transform: translateX({(i - 2) * 40}px) translateZ({Math.abs(i - 2) * -20}px) rotateY({(i - 2) * 10}deg);
                    z-index: {10 - Math.abs(i - 2)};
                  "
                ></div>
              {/each}
              <!-- Central Highlight -->
              <div class="absolute w-32 h-48 border border-white/60 shadow-[0_0_15px_rgba(255,255,255,0.2)] rounded-sm z-20"></div>
           </div>
        </div>

        <!-- List -->
        <div class="space-y-12 pt-4">
          <div class="group cursor-pointer">
            <h3 class="text-xl font-medium mb-3 text-[#111]">Trained on exclusive data</h3>
            <p class="text-gray-600 leading-relaxed">Historical matches, player performance, tactical analysis from rights holders creates unmatched accuracy.</p>
          </div>
          <div class="group cursor-pointer opacity-40 hover:opacity-100 transition-opacity">
            <h3 class="text-xl font-medium mb-3 text-[#111]">Understand fan intent</h3>
            <p class="text-gray-600 leading-relaxed">Deep insights into what fans want — powered by real conversations and engagement patterns.</p>
          </div>
          <div class="group cursor-pointer opacity-40 hover:opacity-100 transition-opacity">
            <h3 class="text-xl font-medium mb-3 text-[#111]">Integrated commerce layer</h3>
            <p class="text-gray-600 leading-relaxed">Tickets, merchandise, and premium content — all without leaving the conversation.</p>
          </div>

          <div class="flex gap-4 pt-8">
             <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-400 hover:border-gray-800 hover:text-gray-800 transition-colors">←</button>
             <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-400 hover:border-gray-800 hover:text-gray-800 transition-colors">→</button>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Fast to Launch -->
  <section class="bg-[#fffcf8] py-32 px-6">
    <div class="max-w-[1400px] mx-auto">
      <h2 class="text-4xl md:text-5xl font-medium tracking-tight mb-20 text-[#111]">
        From pilot to scale in months
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
        <!-- Card 1 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5 21 12m0 0-7.5 7.5M21 12H3" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Rapid deployment</h3>
          <p class="text-gray-600 leading-relaxed">MVP launch with 3 league partnerships and 100K early adopters in Q1-Q2 2026.</p>
        </div>

        <!-- Card 2 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6A2.25 2.25 0 0 1 6 3.75h2.25A2.25 2.25 0 0 1 10.5 6v2.25a2.25 2.25 0 0 1-2.25 2.25H6a2.25 2.25 0 0 1-2.25-2.25V6ZM3.75 15.75A2.25 2.25 0 0 1 6 13.5h2.25a2.25 2.25 0 0 1 2.25 2.25V18a2.25 2.25 0 0 1-2.25 2.25H6A2.25 2.25 0 0 1 3.75 18v-2.25ZM13.5 6a2.25 2.25 0 0 1 2.25-2.25H18A2.25 2.25 0 0 1 20.25 6v2.25A2.25 2.25 0 0 1 18 10.5h-2.25a2.25 2.25 0 0 1-2.25-2.25V6ZM13.5 15.75a2.25 2.25 0 0 1 2.25-2.25H18a2.25 2.25 0 0 1 2.25 2.25V18A2.25 2.25 0 0 1 18 20.25h-2.25A2.25 2.25 0 0 1 13.5 18v-2.25Z" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Multi-sport expansion</h3>
          <p class="text-gray-600 leading-relaxed">Football first, then e-sports and multi-sport platform by 2027.</p>
        </div>

        <!-- Card 3 -->
        <div>
          <div class="w-14 h-14 bg-[#111] text-white flex items-center justify-center rounded-sm mb-8">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round" d="M12 21a9.004 9.004 0 0 0 8.716-6.747M12 21a9.004 9.004 0 0 1-8.716-6.747M12 21c2.485 0 4.5-4.03 4.5-9S14.485 3 12 3m0 18c-2.485 0-4.5-4.03-4.5-9S9.515 3 12 3m0 0a8.997 8.997 0 0 1 7.843 4.582M12 3a8.997 8.997 0 0 0-7.843 4.582m15.686 0A11.953 11.953 0 0 1 12 10.5c-2.998 0-5.74-1.1-7.843-2.918m15.686 0A8.959 8.959 0 0 1 21 12c0 .778-.099 1.533-.284 2.253m0 0A17.919 17.919 0 0 1 12 16.5c-3.162 0-6.133-.815-8.716-2.247m0 0A9.015 9.015 0 0 1 3 12c0-1.605.42-3.113 1.157-4.418" />
            </svg>
          </div>
          <h3 class="text-lg font-medium mb-3 text-[#111]">Global reach</h3>
          <p class="text-gray-600 leading-relaxed">Multi-language support serving fans worldwide from day one.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Banner -->
  <section class="px-6 py-12">
    <div class="max-w-[1400px] mx-auto border border-gray-100 rounded-xl p-8 md:p-12 flex flex-col md:flex-row justify-between items-center gap-8 bg-white shadow-sm">
      <div class="flex items-center gap-6">
        <div class="flex gap-1 h-8">
           <div class="w-2 bg-black h-full"></div>
           <div class="w-2 bg-black h-full"></div>
           <div class="w-2 bg-black h-full"></div>
           <div class="w-2 bg-black h-full opacity-50"></div>
        </div>
        <h2 class="text-2xl md:text-3xl font-medium tracking-tight">Ready to transform your fan experience?</h2>
      </div>
      <button class="bg-black text-white px-8 py-3 text-sm font-medium rounded-sm hover:bg-gray-800 transition-colors whitespace-nowrap">
        Request demo
      </button>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-white pt-20 pb-10 px-6 border-t border-gray-100">
    <div class="max-w-[1400px] mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-12 md:gap-24 mb-20">
        <div class="col-span-1 md:col-span-2">
          <h3 class="text-xl font-medium mb-1">FanLayer</h3>
          <p class="text-gray-500 text-lg">ChatGPT for Sports</p>
        </div>

        <div>
          <ul class="space-y-4 text-sm font-medium">
            <li><a href="#" class="hover:underline">Get in touch</a></li>
            <li><a href="#" class="hover:underline">For Clubs</a></li>
            <li><a href="#" class="hover:underline">Read our Blog</a></li>
          </ul>
        </div>

        <div>
          <ul class="space-y-4 text-sm font-medium">
            <li><a href="#" class="hover:underline">LinkedIn</a></li>
            <li><a href="#" class="hover:underline">X</a></li>
          </ul>
        </div>
      </div>

      <div class="flex flex-col md:flex-row justify-between items-end text-[10px] text-gray-400 uppercase tracking-wider gap-4">
        <div class="flex gap-8">
          <span>FanLayer 2025</span>
          <span>Backed by Werner Vogels (Amazon CTO)</span>
        </div>
        <div class="flex gap-8">
          <a href="#" class="hover:text-gray-600">Terms of use</a>
          <a href="#" class="hover:text-gray-600">Privacy Policy</a>
        </div>
      </div>
    </div>
  </footer>

  <!-- Cookie Banner -->
  {#if showCookieBanner}
    <div class="fixed bottom-6 right-6 max-w-sm bg-white border border-gray-100 shadow-xl p-6 rounded-sm z-50 text-xs text-gray-600">
      <p class="mb-4 leading-relaxed">
        We use cookies. See our <a href="#" class="underline text-black">Privacy Policy</a> for more information.
      </p>
      <button onclick={() => showCookieBanner = false} class="bg-black text-white px-4 py-2 rounded-sm font-medium hover:bg-gray-800 transition-colors">
        Got it
      </button>
    </div>
  {/if}
</div>

<style>
  :global(body) {
    font-family: 'Inter', sans-serif;
  }
  .perspective-1000 {
    perspective: 1000px;
  }
  .transform-style-3d {
    transform-style: preserve-3d;
  }
</style>

