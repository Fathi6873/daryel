 <!doctype html>
<html lang="en" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Daryel App</title>
  <script src="https://cdn.tailwindcss.com/3.4.17"></script>
  <script src="https://cdn.jsdelivr.net/npm/lucide@0.263.0/dist/umd/lucide.min.js"></script>
  <script src="/_sdk/element_sdk.js"></script>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&amp;family=DM+Sans:wght@400;500;600&amp;display=swap" rel="stylesheet">
  <style>
html,body{margin:0;padding:0;height:100%;font-family:'DM Sans',sans-serif}
.font-display{font-family:'Outfit',sans-serif}
.gradient-blob{position:absolute;border-radius:50%;filter:blur(80px);opacity:.35;pointer-events:none}
.card-hover{transition:transform .3s,box-shadow .3s}
.card-hover:hover{transform:translateY(-6px);box-shadow:0 20px 40px rgba(0,0,0,.15)}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-12px)}}
@keyframes fadeUp{from{opacity:0;transform:translateY(30px)}to{opacity:1;transform:translateY(0)}}
.animate-float{animation:float 4s ease-in-out infinite}
.fade-up{animation:fadeUp .7s ease forwards;opacity:0}
.fade-up-1{animation-delay:.1s}.fade-up-2{animation-delay:.2s}.fade-up-3{animation-delay:.3s}.fade-up-4{animation-delay:.4s}.fade-up-5{animation-delay:.5s}
.nav-blur{backdrop-filter:blur(16px);-webkit-backdrop-filter:blur(16px)}
.feature-icon{width:52px;height:52px;border-radius:14px;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.phone-mockup{width:220px;height:440px;border-radius:32px;position:relative;overflow:hidden}
@media(min-width:768px){.phone-mockup{width:260px;height:520px}}
.scroll-section{opacity:0;transform:translateY(40px);transition:opacity .6s ease,transform .6s ease}
.scroll-section.visible{opacity:1;transform:translateY(0)}
</style>
  <style>body { box-sizing: border-box; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
 </head>
 <body class="h-full">
  <div id="app" class="w-full h-full overflow-auto" style="background:#0a0a1a">
   <!-- Nav -->
   <nav class="fixed top-0 left-0 w-full z-50 nav-blur" style="background:rgba(10,10,26,.8)">
    <div class="max-w-6xl mx-auto px-5 py-4 flex items-center justify-between">
     <div class="flex items-center gap-2">
      <div class="w-9 h-9 rounded-xl flex items-center justify-center font-display font-black text-lg" id="nav-logo-bg" style="background:#6c5ce7;color:#fff">
       D
      </div><span class="font-display font-bold text-xl" id="nav-title" style="color:#fff">Daryel</span>
     </div>
     <div class="hidden md:flex items-center gap-8">
      <a href="#features" class="text-sm" style="color:rgba(255,255,255,.7)" onmouseover="this.style.color='#fff'" onmouseout="this.style.color='rgba(255,255,255,.7)'">Features</a> <a href="#menu" class="text-sm" style="color:rgba(255,255,255,.7)" onmouseover="this.style.color='#fff'" onmouseout="this.style.color='rgba(255,255,255,.7)'">Menu</a>
      <div class="relative group">
       <button class="text-sm flex items-center gap-1" style="color:rgba(255,255,255,.7)" onmouseover="this.style.color='#fff'" onmouseout="this.style.color='rgba(255,255,255,.7)'">Explore <i data-lucide="chevron-down" style="width:14px;height:14px"></i></button>
       <div class="absolute left-0 mt-2 w-40 rounded-xl p-2 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all" style="background:rgba(10,10,26,.95);border:1px solid rgba(255,255,255,.06);backdrop-filter:blur(16px)">
        <a href="#community" class="block px-3 py-2 rounded-lg text-sm" style="color:rgba(255,255,255,.7)" onmouseover="this.style.background='rgba(108,92,231,.1)';this.style.color='#fff'" onmouseout="this.style.background='';this.style.color='rgba(255,255,255,.7)'">Community</a> <a href="#creativity" class="block px-3 py-2 rounded-lg text-sm" style="color:rgba(255,255,255,.7)" onmouseover="this.style.background='rgba(108,92,231,.1)';this.style.color='#fff'" onmouseout="this.style.background='';this.style.color='rgba(255,255,255,.7)'">Creativity</a> <a href="#security" class="block px-3 py-2 rounded-lg text-sm" style="color:rgba(255,255,255,.7)" onmouseover="this.style.background='rgba(108,92,231,.1)';this.style.color='#fff'" onmouseout="this.style.background='';this.style.color='rgba(255,255,255,.7)'">Security</a>
       </div>
      </div><a href="#performance" class="text-sm" style="color:rgba(255,255,255,.7)" onmouseover="this.style.color='#fff'" onmouseout="this.style.color='rgba(255,255,255,.7)'">Performance</a>
     </div><button id="cta-nav" class="px-5 py-2 rounded-full text-sm font-semibold text-white transition-all hover:scale-105" style="background:#6c5ce7">Get Started</button>
    </div>
   </nav><!-- Hero -->
   <section class="relative pt-28 pb-20 md:pt-36 md:pb-28 px-5 overflow-hidden">
    <div class="gradient-blob" style="width:500px;height:500px;background:#6c5ce7;top:-100px;left:-100px"></div>
    <div class="gradient-blob" style="width:400px;height:400px;background:#00cec9;top:100px;right:-80px"></div>
    <div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center gap-12">
     <div class="flex-1 text-center md:text-left z-10">
      <div class="fade-up fade-up-1 inline-flex items-center gap-2 px-4 py-1.5 rounded-full text-xs font-medium mb-6" style="background:rgba(108,92,231,.2);color:#a29bfe">
       <i data-lucide="sparkles" style="width:14px;height:14px"></i> Your social world, simplified
      </div>
      <h1 id="hero-title" class="font-display font-800 text-5xl md:text-7xl leading-tight mb-5 fade-up fade-up-2" style="color:#fff">Daryel</h1>
      <p id="hero-subtitle" class="text-lg md:text-xl font-medium mb-4 fade-up fade-up-3" style="color:#a29bfe">Explore, connect and share your interests with real people</p>
      <p id="hero-desc" class="text-base leading-relaxed mb-8 fade-up fade-up-4" style="color:rgba(255,255,255,.6);max-width:480px">It's simple, reliable, and private, so you can easily keep in touch with your friends and family. A lightweight, all-in-one social platform designed for slower networks too.</p>
      <div class="flex flex-col sm:flex-row gap-3 justify-center md:justify-start fade-up fade-up-5">
       <button id="cta-hero" class="px-8 py-3.5 rounded-full font-semibold text-white transition-all hover:scale-105 hover:shadow-lg" style="background:#6c5ce7;box-shadow:0 4px 20px rgba(108,92,231,.4)">Download Now</button> <button class="px-8 py-3.5 rounded-full font-semibold transition-all hover:scale-105" style="background:rgba(255,255,255,.08);color:#fff;border:1px solid rgba(255,255,255,.12)">Learn More</button>
      </div>
     </div>
     <div class="flex-shrink-0 z-10 relative">
      <div class="phone-mockup animate-float" style="background:linear-gradient(135deg,#6c5ce7,#00cec9);box-shadow:0 30px 60px rgba(108,92,231,.3)">
       <div style="position:absolute;inset:3px;border-radius:30px;background:#1a1a2e;display:flex;flex-direction:column;padding:20px">
        <div class="flex items-center gap-2 mb-5">
         <div class="w-8 h-8 rounded-full" style="background:#6c5ce7"></div>
         <div>
          <div class="w-20 h-2 rounded" style="background:rgba(255,255,255,.3)"></div>
          <div class="w-14 h-1.5 rounded mt-1" style="background:rgba(255,255,255,.15)"></div>
         </div>
        </div>
        <div class="rounded-2xl p-3 mb-3" style="background:rgba(108,92,231,.15)">
         <div class="w-full h-2 rounded mb-1.5" style="background:rgba(255,255,255,.2)"></div>
         <div class="w-3/4 h-2 rounded" style="background:rgba(255,255,255,.12)"></div>
        </div>
        <div class="rounded-2xl p-3 mb-3" style="background:rgba(0,206,201,.1)">
         <div class="w-full h-24 rounded-xl mb-2" style="background:linear-gradient(135deg,rgba(108,92,231,.3),rgba(0,206,201,.3))"></div>
         <div class="w-2/3 h-2 rounded" style="background:rgba(255,255,255,.15)"></div>
        </div>
        <div class="rounded-2xl p-3" style="background:rgba(255,255,255,.05)">
         <div class="flex gap-2 items-center">
          <div class="w-6 h-6 rounded-full" style="background:#00cec9"></div>
          <div class="w-full h-2 rounded" style="background:rgba(255,255,255,.15)"></div>
         </div>
        </div>
        <div class="mt-auto flex justify-around pt-4" style="border-top:1px solid rgba(255,255,255,.08)">
         <i data-lucide="home" style="width:18px;height:18px;color:#6c5ce7"></i> <i data-lucide="search" style="width:18px;height:18px;color:rgba(255,255,255,.3)"></i> <i data-lucide="plus-circle" style="width:18px;height:18px;color:rgba(255,255,255,.3)"></i> <i data-lucide="heart" style="width:18px;height:18px;color:rgba(255,255,255,.3)"></i> <i data-lucide="user" style="width:18px;height:18px;color:rgba(255,255,255,.3)"></i>
        </div>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Features Grid -->
   <section id="features" class="px-5 py-20 relative">
    <div class="max-w-6xl mx-auto">
     <div class="text-center mb-14 scroll-section">
      <h2 class="font-display font-bold text-3xl md:text-4xl mb-3" style="color:#fff">Everything You Need</h2>
      <p style="color:rgba(255,255,255,.5);max-width:500px;margin:0 auto">One app for messaging, sharing, creating and connecting with the people who matter most.</p>
     </div>
     <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-5">
      <!-- Profile & Identity -->
      <div class="scroll-section rounded-2xl card-hover feature-card cursor-pointer" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-main p-6">
        <div class="feature-icon mb-4" id="fi-profile" style="background:rgba(108,92,231,.15)"><i data-lucide="user-circle" style="width:26px;height:26px;color:#a29bfe"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Profile &amp; Identity</h3>
        <p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.5)">Full control over your digital identity and privacy settings.</p>
        <p class="text-xs mt-3" style="color:rgba(162,155,254,.6)">Click to expand →</p>
       </div>
       <div class="feature-sub hidden p-6">
        <div class="flex items-center gap-2 mb-4">
         <i data-lucide="chevron-left" style="width:20px;height:20px;color:#a29bfe;cursor:pointer" class="back-btn"></i>
         <h3 class="font-display font-semibold text-lg" style="color:#fff">Profile Details</h3>
        </div>
        <ul class="space-y-3">
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Complete profile setup with name, gender, age</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Verified email address</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Upload profile picture and bio</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Privacy level selection</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Block &amp; report features</span></li>
        </ul>
       </div>
      </div><!-- Secure Access -->
      <div class="scroll-section rounded-2xl card-hover feature-card cursor-pointer" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-main p-6">
        <div class="feature-icon mb-4" style="background:rgba(0,206,201,.15)"><i data-lucide="lock" style="width:26px;height:26px;color:#00cec9"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Secure Access</h3>
        <p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.5)">Password remember, change and recovery features.</p>
        <p class="text-xs mt-3" style="color:rgba(0,206,201,.6)">Click to expand →</p>
       </div>
       <div class="feature-sub hidden p-6">
        <div class="flex items-center gap-2 mb-4">
         <i data-lucide="chevron-left" style="width:20px;height:20px;color:#00cec9;cursor:pointer" class="back-btn"></i>
         <h3 class="font-display font-semibold text-lg" style="color:#fff">Security Features</h3>
        </div>
        <ul class="space-y-3">
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Secure password encryption</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Password reset via email</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Two-factor authentication</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Session management &amp; logout</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Login activity tracking</span></li>
        </ul>
       </div>
      </div><!-- Feed & Stories -->
      <div class="scroll-section rounded-2xl card-hover feature-card cursor-pointer" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-main p-6">
        <div class="feature-icon mb-4" style="background:rgba(253,203,110,.15)"><i data-lucide="rss" style="width:26px;height:26px;color:#fdcb6e"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Feed &amp; Stories</h3>
        <p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.5)">Personalized feed and immersive Stories from friends.</p>
        <p class="text-xs mt-3" style="color:rgba(253,203,110,.6)">Click to expand →</p>
       </div>
       <div class="feature-sub hidden p-6">
        <div class="flex items-center gap-2 mb-4">
         <i data-lucide="chevron-left" style="width:20px;height:20px;color:#fdcb6e;cursor:pointer" class="back-btn"></i>
         <h3 class="font-display font-semibold text-lg" style="color:#fff">Feed Options</h3>
        </div>
        <ul class="space-y-3">
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#fdcb6e;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">AI-powered personalized feed</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#fdcb6e;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">24-hour Stories from contacts</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#fdcb6e;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Like, comment &amp; share posts</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#fdcb6e;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Story reactions &amp; replies</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#fdcb6e;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Archive &amp; highlight Stories</span></li>
        </ul>
       </div>
      </div><!-- Creative Reels -->
      <div class="scroll-section rounded-2xl card-hover feature-card cursor-pointer" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-main p-6">
        <div class="feature-icon mb-4" style="background:rgba(255,118,117,.15)"><i data-lucide="video" style="width:26px;height:26px;color:#ff7675"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Creative Reels</h3>
        <p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.5)">Show your creative side with trending audio and editing tools.</p>
        <p class="text-xs mt-3" style="color:rgba(255,118,117,.6)">Click to expand →</p>
       </div>
       <div class="feature-sub hidden p-6">
        <div class="flex items-center gap-2 mb-4">
         <i data-lucide="chevron-left" style="width:20px;height:20px;color:#ff7675;cursor:pointer" class="back-btn"></i>
         <h3 class="font-display font-semibold text-lg" style="color:#fff">Reel Tools</h3>
        </div>
        <ul class="space-y-3">
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#ff7675;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Record &amp; edit 15-60 sec videos</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#ff7675;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Access to trending music &amp; audio</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#ff7675;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Filters, effects &amp; transitions</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#ff7675;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Speed control &amp; slow motion</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#ff7675;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Reach new audiences via Reels feed</span></li>
        </ul>
       </div>
      </div><!-- Messenger -->
      <div class="scroll-section rounded-2xl card-hover feature-card cursor-pointer" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-main p-6">
        <div class="feature-icon mb-4" style="background:rgba(108,92,231,.15)"><i data-lucide="message-circle" style="width:26px;height:26px;color:#a29bfe"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Messenger</h3>
        <p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.5)">Integrated chats, voice notes and crystal-clear calls.</p>
        <p class="text-xs mt-3" style="color:rgba(162,155,254,.6)">Click to expand →</p>
       </div>
       <div class="feature-sub hidden p-6">
        <div class="flex items-center gap-2 mb-4">
         <i data-lucide="chevron-left" style="width:20px;height:20px;color:#a29bfe;cursor:pointer" class="back-btn"></i>
         <h3 class="font-display font-semibold text-lg" style="color:#fff">Messaging Features</h3>
        </div>
        <ul class="space-y-3">
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Real-time text messaging</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Voice messages &amp; audio clips</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Crystal-clear HD voice calls</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Group chats &amp; calls</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Shared media &amp; files</span></li>
        </ul>
       </div>
      </div><!-- Live Location -->
      <div class="scroll-section rounded-2xl card-hover feature-card cursor-pointer" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-main p-6">
        <div class="feature-icon mb-4" style="background:rgba(0,206,201,.15)"><i data-lucide="map-pin" style="width:26px;height:26px;color:#00cec9"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Live Location</h3>
        <p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.5)">Share real-time location with the ability to stop anytime.</p>
        <p class="text-xs mt-3" style="color:rgba(0,206,201,.6)">Click to expand →</p>
       </div>
       <div class="feature-sub hidden p-6">
        <div class="flex items-center gap-2 mb-4">
         <i data-lucide="chevron-left" style="width:20px;height:20px;color:#00cec9;cursor:pointer" class="back-btn"></i>
         <h3 class="font-display font-semibold text-lg" style="color:#fff">Location Sharing</h3>
        </div>
        <ul class="space-y-3">
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Real-time location sharing in chats</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Set sharing duration (15 min - 1 hour)</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Stop sharing anytime instantly</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Privacy-first design</span></li>
         <li class="flex gap-2"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i><span class="text-sm" style="color:rgba(255,255,255,.7)">Only in 1-to-1 or group chats</span></li>
        </ul>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Menu Section -->
   <section id="menu" class="px-5 py-20 relative">
    <div class="max-w-6xl mx-auto">
     <div class="text-center mb-14 scroll-section">
      <h2 class="font-display font-bold text-3xl md:text-4xl mb-3" style="color:#fff">Navigation &amp; Controls</h2>
      <p style="color:rgba(255,255,255,.5);max-width:500px;margin:0 auto">Access all your app features and tools from one intuitive menu system.</p>
     </div>
     <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div class="scroll-section rounded-2xl p-8 card-hover" style="background:linear-gradient(135deg,rgba(108,92,231,.08),rgba(162,155,254,.06));border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mb-5" style="background:rgba(108,92,231,.15)"><i data-lucide="menu" style="width:26px;height:26px;color:#a29bfe"></i>
       </div>
       <h3 class="font-display font-semibold text-xl mb-4" style="color:#fff">Main Navigation Menu</h3>
       <ul class="space-y-3">
        <li class="flex gap-3 items-start"><i data-lucide="home" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Home</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Your personalized feed and updates</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="search" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Discover</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Find people, communities &amp; content</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="plus-circle" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Create</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Post stories, reels &amp; messages</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="heart" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Notifications</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Likes, comments &amp; interactions</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="message-circle" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Messages</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Direct chats &amp; conversations</p>
         </div></li>
       </ul>
      </div>
      <div class="scroll-section rounded-2xl p-8 card-hover" style="background:linear-gradient(135deg,rgba(0,206,201,.08),rgba(0,206,201,.05));border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mb-5" style="background:rgba(0,206,201,.15)"><i data-lucide="layout-grid" style="width:26px;height:26px;color:#00cec9"></i>
       </div>
       <h3 class="font-display font-semibold text-xl mb-4" style="color:#fff">Quick Access</h3>
       <ul class="space-y-3">
        <li class="flex gap-3 items-start"><i data-lucide="bell" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Activity</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Real-time updates &amp; alerts</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="bookmark" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Saved</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Your bookmarks &amp; favorites</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="users" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Friends</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Manage your connections</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="play-circle" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Reels</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Video content &amp; entertainment</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="radio" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Stories</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Ephemeral content from friends</p>
         </div></li>
       </ul>
      </div>
     </div>
    </div>
   </section><!-- Settings &amp; Profile Section -->
   <section id="settings" class="px-5 py-20 relative">
    <div class="gradient-blob" style="width:350px;height:350px;background:#6c5ce7;top:0;left:-80px"></div>
    <div class="max-w-6xl mx-auto">
     <div class="text-center mb-14 scroll-section">
      <h2 class="font-display font-bold text-3xl md:text-4xl mb-3" style="color:#fff">Settings &amp; Profile Management</h2>
      <p style="color:rgba(255,255,255,.5);max-width:500px;margin:0 auto">Customize your account, privacy settings, and preferences all in one place.</p>
     </div>
     <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
      <div class="scroll-section rounded-2xl p-8 card-hover" style="background:linear-gradient(135deg,rgba(253,203,110,.08),rgba(255,118,117,.06));border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mb-5" style="background:rgba(253,203,110,.15)"><i data-lucide="user-cog" style="width:26px;height:26px;color:#fdcb6e"></i>
       </div>
       <h3 class="font-display font-semibold text-xl mb-4" style="color:#fff">Profile Settings</h3>
       <ul class="space-y-3">
        <li class="flex gap-3 items-start"><i data-lucide="image" style="width:18px;height:18px;color:#fdcb6e;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Profile Picture</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Upload or change your avatar</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="edit-2" style="width:18px;height:18px;color:#fdcb6e;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Edit Profile</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Update bio, name &amp; info</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="link" style="width:18px;height:18px;color:#fdcb6e;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Social Links</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Connect your other profiles</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="palette" style="width:18px;height:18px;color:#fdcb6e;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Themes</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Customize profile appearance</p>
         </div></li>
       </ul>
      </div>
      <div class="scroll-section rounded-2xl p-8 card-hover" style="background:linear-gradient(135deg,rgba(255,118,117,.08),rgba(255,173,173,.06));border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mb-5" style="background:rgba(255,118,117,.15)"><i data-lucide="shield-alert" style="width:26px;height:26px;color:#ff7675"></i>
       </div>
       <h3 class="font-display font-semibold text-xl mb-4" style="color:#fff">Privacy &amp; Security</h3>
       <ul class="space-y-3">
        <li class="flex gap-3 items-start"><i data-lucide="lock" style="width:18px;height:18px;color:#ff7675;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Change Password</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Update your account password</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="smartphone" style="width:18px;height:18px;color:#ff7675;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Two-Factor Auth</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Enable 2FA for extra security</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="eye-off" style="width:18px;height:18px;color:#ff7675;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Privacy Controls</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Manage who sees your content</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="activity" style="width:18px;height:18px;color:#ff7675;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Active Sessions</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Manage login locations</p>
         </div></li>
       </ul>
      </div>
      <div class="scroll-section rounded-2xl p-8 card-hover" style="background:linear-gradient(135deg,rgba(108,92,231,.08),rgba(162,155,254,.06));border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mb-5" style="background:rgba(108,92,231,.15)"><i data-lucide="bell" style="width:26px;height:26px;color:#a29bfe"></i>
       </div>
       <h3 class="font-display font-semibold text-xl mb-4" style="color:#fff">Notifications</h3>
       <ul class="space-y-3">
        <li class="flex gap-3 items-start"><i data-lucide="mail" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Email Alerts</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Control email notifications</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="bell-ring" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Push Notifications</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">App push notification settings</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="message-square" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Message Alerts</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">New message notifications</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="volume-2" style="width:18px;height:18px;color:#a29bfe;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Sound &amp; Vibration</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Customize alert sounds</p>
         </div></li>
       </ul>
      </div>
      <div class="scroll-section rounded-2xl p-8 card-hover" style="background:linear-gradient(135deg,rgba(0,206,201,.08),rgba(0,206,201,.05));border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mb-5" style="background:rgba(0,206,201,.15)"><i data-lucide="settings" style="width:26px;height:26px;color:#00cec9"></i>
       </div>
       <h3 class="font-display font-semibold text-xl mb-4" style="color:#fff">General Settings</h3>
       <ul class="space-y-3">
        <li class="flex gap-3 items-start"><i data-lucide="globe" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Language</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Choose your preferred language</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="moon" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Dark Mode</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Display and theme options</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="database" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">Storage</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">Manage app cache &amp; data</p>
         </div></li>
        <li class="flex gap-3 items-start"><i data-lucide="info" style="width:18px;height:18px;color:#00cec9;flex-shrink:0;margin-top:2px"></i>
         <div>
          <p class="text-sm font-medium" style="color:#fff">About</p>
          <p class="text-xs" style="color:rgba(255,255,255,.5)">App version &amp; information</p>
         </div></li>
       </ul>
      </div>
     </div>
    </div>
   </section>
   <section id="community" class="px-5 py-20 relative">
    <div class="gradient-blob" style="width:400px;height:400px;background:#00cec9;bottom:0;left:-100px"></div>
    <div class="max-w-6xl mx-auto">
     <div class="scroll-section flex flex-col md:flex-row items-center gap-12 rounded-3xl p-8 md:p-12" style="background:linear-gradient(135deg,rgba(108,92,231,.1),rgba(0,206,201,.08));border:1px solid rgba(255,255,255,.06)">
      <div class="flex-1">
       <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full text-xs font-medium mb-4" style="background:rgba(0,206,201,.15);color:#00cec9"><i data-lucide="users" style="width:12px;height:12px"></i> Community
       </div>
       <h2 id="community-heading" class="font-display font-bold text-3xl md:text-4xl mb-4" style="color:#fff">Build Your Community</h2>
       <ul class="space-y-4">
        <li class="flex gap-3 items-start">
         <div class="w-6 h-6 rounded-full flex items-center justify-center flex-shrink-0 mt-0.5" style="background:rgba(108,92,231,.2)"><i data-lucide="check" style="width:14px;height:14px;color:#a29bfe"></i>
         </div><p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.6)"><strong style="color:#fff">Connect with People &amp; Groups</strong> — Join communities to exchange tips and learn from real-world experiences.</p></li>
        <li class="flex gap-3 items-start">
         <div class="w-6 h-6 rounded-full flex items-center justify-center flex-shrink-0 mt-0.5" style="background:rgba(108,92,231,.2)"><i data-lucide="check" style="width:14px;height:14px;color:#a29bfe"></i>
         </div><p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.6)"><strong style="color:#fff">Stay Updated</strong> — Personalized Feed and immersive Stories from friends, family and influencers.</p></li>
        <li class="flex gap-3 items-start">
         <div class="w-6 h-6 rounded-full flex items-center justify-center flex-shrink-0 mt-0.5" style="background:rgba(108,92,231,.2)"><i data-lucide="check" style="width:14px;height:14px;color:#a29bfe"></i>
         </div><p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.6)"><strong style="color:#fff">Seamless Communication</strong> — Integrated Messenger chats right where you need them.</p></li>
       </ul>
      </div>
      <div class="flex-shrink-0 grid grid-cols-2 gap-3">
       <div class="w-28 h-28 rounded-2xl flex flex-col items-center justify-center" style="background:rgba(108,92,231,.12)"><i data-lucide="users" style="width:28px;height:28px;color:#a29bfe"></i><span class="text-xs mt-2 font-medium" style="color:rgba(255,255,255,.6)">Groups</span>
       </div>
       <div class="w-28 h-28 rounded-2xl flex flex-col items-center justify-center" style="background:rgba(0,206,201,.12)"><i data-lucide="radio" style="width:28px;height:28px;color:#00cec9"></i><span class="text-xs mt-2 font-medium" style="color:rgba(255,255,255,.6)">Stories</span>
       </div>
       <div class="w-28 h-28 rounded-2xl flex flex-col items-center justify-center" style="background:rgba(253,203,110,.12)"><i data-lucide="message-circle" style="width:28px;height:28px;color:#fdcb6e"></i><span class="text-xs mt-2 font-medium" style="color:rgba(255,255,255,.6)">Chat</span>
       </div>
       <div class="w-28 h-28 rounded-2xl flex flex-col items-center justify-center" style="background:rgba(255,118,117,.12)"><i data-lucide="heart" style="width:28px;height:28px;color:#ff7675"></i><span class="text-xs mt-2 font-medium" style="color:rgba(255,255,255,.6)">Connect</span>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Creativity Section -->
   <section id="creativity" class="px-5 py-20 relative">
    <div class="max-w-6xl mx-auto scroll-section">
     <div class="text-center mb-10">
      <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full text-xs font-medium mb-4" style="background:rgba(253,203,110,.15);color:#fdcb6e"><i data-lucide="sparkles" style="width:12px;height:12px"></i> Creativity
      </div>
      <h2 id="creativity-heading" class="font-display font-bold text-3xl md:text-4xl mb-3" style="color:#fff">Express Your Creativity</h2>
      <p style="color:rgba(255,255,255,.5);max-width:480px;margin:0 auto">Create engaging Reels with trending audio, and personalize your profile to control who sees your posts.</p>
     </div>
     <div class="grid grid-cols-1 md:grid-cols-2 gap-5">
      <div class="rounded-2xl p-8 card-hover" style="background:linear-gradient(135deg,rgba(253,203,110,.08),rgba(255,118,117,.06));border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mb-5" style="background:rgba(255,118,117,.15)"><i data-lucide="clapperboard" style="width:26px;height:26px;color:#ff7675"></i>
       </div>
       <h3 class="font-display font-semibold text-xl mb-2" style="color:#fff">Engaging Reels</h3>
       <p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.5)">Show your creative side using trending audio and a professional suite of editing tools. Reach new audiences with short-form video.</p>
      </div>
      <div class="rounded-2xl p-8 card-hover" style="background:linear-gradient(135deg,rgba(108,92,231,.08),rgba(162,155,254,.06));border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mb-5" style="background:rgba(108,92,231,.15)"><i data-lucide="palette" style="width:26px;height:26px;color:#a29bfe"></i>
       </div>
       <h3 class="font-display font-semibold text-xl mb-2" style="color:#fff">Personalized Profile</h3>
       <p class="text-sm leading-relaxed" style="color:rgba(255,255,255,.5)">Take full control of your digital presence. Customize how you appear and choose exactly who sees your posts.</p>
      </div>
     </div>
    </div>
   </section><!-- Performance Section --> <!-- Performance Section -->
   <section id="performance" class="px-5 py-20 relative">
    <div class="gradient-blob" style="width:400px;height:400px;background:#00cec9;bottom:0;right:-100px"></div>
    <div class="max-w-6xl mx-auto">
     <div class="scroll-section">
      <div class="text-center mb-12">
       <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full text-xs font-medium mb-4" style="background:rgba(0,206,201,.15);color:#00cec9"><i data-lucide="zap" style="width:12px;height:12px"></i> Performance
       </div>
       <h2 id="performance-heading" class="font-display font-bold text-3xl md:text-4xl mb-3" style="color:#fff">Lightning-Fast Performance</h2>
       <p style="color:rgba(255,255,255,.5);max-width:520px;margin:0 auto">Engineered for speed and efficiency. Built for everyone, everywhere.</p>
      </div><!-- Performance Metrics Grid -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 mb-8">
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="flex items-end justify-between mb-4">
         <div class="feature-icon" style="background:rgba(0,206,201,.15)"><i data-lucide="zap" style="width:24px;height:24px;color:#00cec9"></i>
         </div>
        </div>
        <h3 class="font-display font-semibold text-2xl" style="color:#00cec9">0.8s</h3>
        <p class="text-xs mt-1" style="color:rgba(255,255,255,.5)">Average load time</p>
       </div>
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="flex items-end justify-between mb-4">
         <div class="feature-icon" style="background:rgba(108,92,231,.15)"><i data-lucide="smartphone" style="width:24px;height:24px;color:#a29bfe"></i>
         </div>
        </div>
        <h3 class="font-display font-semibold text-2xl" style="color:#a29bfe">45MB</h3>
        <p class="text-xs mt-1" style="color:rgba(255,255,255,.5)">Total app size</p>
       </div>
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="flex items-end justify-between mb-4">
         <div class="feature-icon" style="background:rgba(253,203,110,.15)"><i data-lucide="battery" style="width:24px;height:24px;color:#fdcb6e"></i>
         </div>
        </div>
        <h3 class="font-display font-semibold text-2xl" style="color:#fdcb6e">60%</h3>
        <p class="text-xs mt-1" style="color:rgba(255,255,255,.5)">Battery usage reduction</p>
       </div>
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="flex items-end justify-between mb-4">
         <div class="feature-icon" style="background:rgba(255,118,117,.15)"><i data-lucide="wifi" style="width:24px;height:24px;color:#ff7675"></i>
         </div>
        </div>
        <h3 class="font-display font-semibold text-2xl" style="color:#ff7675">2G+</h3>
        <p class="text-xs mt-1" style="color:rgba(255,255,255,.5)">Network compatible</p>
       </div>
      </div><!-- Features List -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
       <div class="rounded-2xl p-6 card-hover" style="background:linear-gradient(135deg,rgba(0,206,201,.08),rgba(108,92,231,.06));border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(0,206,201,.15)"><i data-lucide="zap" style="width:26px;height:26px;color:#00cec9"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Ultra-Fast Loading</h3>
        <ul class="space-y-2">
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i> Smart caching system</li>
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i> Image compression</li>
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#00cec9;flex-shrink:0"></i> Progressive loading</li>
        </ul>
       </div>
       <div class="rounded-2xl p-6 card-hover" style="background:linear-gradient(135deg,rgba(108,92,231,.08),rgba(162,155,254,.06));border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(108,92,231,.15)"><i data-lucide="battery" style="width:26px;height:26px;color:#a29bfe"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Battery Efficient</h3>
        <ul class="space-y-2">
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i> Smart power management</li>
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i> Reduced background activity</li>
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#a29bfe;flex-shrink:0"></i> Adaptive refresh rates</li>
        </ul>
       </div>
       <div class="rounded-2xl p-6 card-hover" style="background:linear-gradient(135deg,rgba(253,203,110,.08),rgba(255,118,117,.06));border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(253,203,110,.15)"><i data-lucide="database" style="width:26px;height:26px;color:#fdcb6e"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Offline Access</h3>
        <ul class="space-y-2">
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#fdcb6e;flex-shrink:0"></i> Read messages offline</li>
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#fdcb6e;flex-shrink:0"></i> Auto-sync on reconnect</li>
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#fdcb6e;flex-shrink:0"></i> Core features work anywhere</li>
        </ul>
       </div>
       <div class="rounded-2xl p-6 card-hover" style="background:linear-gradient(135deg,rgba(255,118,117,.08),rgba(255,173,173,.06));border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(255,118,117,.15)"><i data-lucide="hard-drive" style="width:26px;height:26px;color:#ff7675"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Minimal Storage</h3>
        <ul class="space-y-2">
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#ff7675;flex-shrink:0"></i> 45MB app footprint</li>
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#ff7675;flex-shrink:0"></i> Smart cache cleanup</li>
         <li class="text-sm flex gap-2" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:16px;height:16px;color:#ff7675;flex-shrink:0"></i> Compressed media</li>
        </ul>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Friends & Family Chat Section -->
   <section id="chat" class="px-5 py-20 relative">
    <div class="gradient-blob" style="width:400px;height:400px;background:#00cec9;bottom:0;left:-100px;opacity:0.25"></div>
    <div class="max-w-6xl mx-auto">
     <div class="text-center mb-14 scroll-section">
      <h2 class="font-display font-bold text-3xl md:text-4xl mb-3" style="color:#fff">Friends &amp; Family Chat</h2>
      <p style="color:rgba(255,255,255,.5);max-width:500px;margin:0 auto">Stay connected with loved ones through group chats, voice messages, and real-time conversations.</p>
     </div>
     <div class="grid grid-cols-1 lg:grid-cols-3 gap-6"><!-- Chat Preview Card -->
      <div class="scroll-section lg:col-span-1 rounded-2xl p-6 card-hover" style="background:linear-gradient(135deg,rgba(108,92,231,.08),rgba(162,155,254,.06));border:1px solid rgba(255,255,255,.06);min-height:500px;display:flex;flex-direction:column">
       <div class="flex items-center gap-2 mb-6">
        <div class="w-10 h-10 rounded-full" style="background:linear-gradient(135deg,#6c5ce7,#a29bfe)"></div>
        <div>
         <p class="text-sm font-medium" style="color:#fff">Family Group</p>
         <p class="text-xs" style="color:rgba(255,255,255,.5)">3 online</p>
        </div>
       </div>
       <div class="flex-1 space-y-4 mb-6 overflow-y-auto" style="scrollbar-width:thin;scrollbar-color:rgba(255,255,255,.1) transparent">
        <div class="flex gap-2">
         <div class="w-8 h-8 rounded-full flex-shrink-0" style="background:rgba(108,92,231,.2)"></div>
         <div class="rounded-2xl p-3 max-w-xs" style="background:rgba(108,92,231,.15)">
          <p class="text-xs" style="color:rgba(255,255,255,.7)">Hey everyone! Just arrived at grandma's place</p>
         </div>
        </div>
        <div class="flex gap-2 justify-end">
         <div class="rounded-2xl p-3 max-w-xs text-right" style="background:rgba(0,206,201,.2)">
          <p class="text-xs" style="color:rgba(255,255,255,.7)">That's awesome! We're leaving now 😊</p>
         </div>
         <div class="w-8 h-8 rounded-full flex-shrink-0" style="background:rgba(0,206,201,.2)"></div>
        </div>
        <div class="flex gap-2">
         <div class="w-8 h-8 rounded-full flex-shrink-0" style="background:rgba(253,203,110,.2)"></div>
         <div class="rounded-2xl p-3 max-w-xs" style="background:rgba(253,203,110,.15)">
          <p class="text-xs" style="color:rgba(255,255,255,.7)">🎉 See you soon!</p>
         </div>
        </div>
       </div>
       <div class="flex gap-2 pt-4" style="border-top:1px solid rgba(255,255,255,.06)"><input type="text" placeholder="Type a message..." class="flex-1 bg-transparent text-xs text-white placeholder-opacity-40 focus:outline-none" style="color:rgba(255,255,255,.7)"> <button style="background:rgba(108,92,231,.3);color:#a29bfe;border-radius:8px;padding:6px 12px;border:none;cursor:pointer"> <i data-lucide="send" style="width:16px;height:16px"></i> </button>
       </div>
      </div><!-- Features Grid -->
      <div class="scroll-section lg:col-span-2 grid grid-cols-1 sm:grid-cols-2 gap-5"><!-- Group Chats -->
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(108,92,231,.15)"><i data-lucide="users" style="width:26px;height:26px;color:#a29bfe"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Group Chats</h3>
        <p class="text-sm leading-relaxed mb-4" style="color:rgba(255,255,255,.5)">Create group conversations with family and friends.</p>
        <ul class="space-y-2">
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#a29bfe;flex-shrink:0"></i> Unlimited members</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#a29bfe;flex-shrink:0"></i> Admin controls</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#a29bfe;flex-shrink:0"></i> Custom group names</li>
        </ul>
       </div><!-- Voice Messages -->
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(0,206,201,.15)"><i data-lucide="mic-2" style="width:26px;height:26px;color:#00cec9"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Voice Messages</h3>
        <p class="text-sm leading-relaxed mb-4" style="color:rgba(255,255,255,.5)">Send quick voice clips instead of typing.</p>
        <ul class="space-y-2">
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#00cec9;flex-shrink:0"></i> One-tap recording</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#00cec9;flex-shrink:0"></i> Auto-transcription</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#00cec9;flex-shrink:0"></i> Play at any speed</li>
        </ul>
       </div><!-- Media Sharing -->
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(253,203,110,.15)"><i data-lucide="image" style="width:26px;height:26px;color:#fdcb6e"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Share Photos &amp; Videos</h3>
        <p class="text-sm leading-relaxed mb-4" style="color:rgba(255,255,255,.5)">Instantly share memories with your loved ones.</p>
        <ul class="space-y-2">
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#fdcb6e;flex-shrink:0"></i> Gallery access</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#fdcb6e;flex-shrink:0"></i> Quick compression</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#fdcb6e;flex-shrink:0"></i> Instant sharing</li>
        </ul>
       </div><!-- Pinned Messages -->
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(255,118,117,.15)"><i data-lucide="bookmark" style="width:26px;height:26px;color:#ff7675"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Pinned Messages</h3>
        <p class="text-sm leading-relaxed mb-4" style="color:rgba(255,255,255,.5)">Keep important info at the top of chats.</p>
        <ul class="space-y-2">
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#ff7675;flex-shrink:0"></i> Pin important messages</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#ff7675;flex-shrink:0"></i> Easy reference</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#ff7675;flex-shrink:0"></i> Unpin anytime</li>
        </ul>
       </div><!-- Read Receipts -->
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(0,206,201,.15)"><i data-lucide="check-double" style="width:26px;height:26px;color:#00cec9"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Read Receipts</h3>
        <p class="text-sm leading-relaxed mb-4" style="color:rgba(255,255,255,.5)">Know when messages have been seen.</p>
        <ul class="space-y-2">
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#00cec9;flex-shrink:0"></i> Delivery status</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#00cec9;flex-shrink:0"></i> Read timestamps</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#00cec9;flex-shrink:0"></i> Typing indicators</li>
        </ul>
       </div><!-- Reactions & Emojis -->
       <div class="rounded-2xl p-6 card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
        <div class="feature-icon mb-4" style="background:rgba(108,92,231,.15)"><i data-lucide="smile" style="width:26px;height:26px;color:#a29bfe"></i>
        </div>
        <h3 class="font-display font-semibold text-lg mb-2" style="color:#fff">Reactions &amp; Emojis</h3>
        <p class="text-sm leading-relaxed mb-4" style="color:rgba(255,255,255,.5)">Express yourself with reactions and stickers.</p>
        <ul class="space-y-2">
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#a29bfe;flex-shrink:0"></i> Message reactions</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#a29bfe;flex-shrink:0"></i> Sticker packs</li>
         <li class="flex gap-2 text-xs" style="color:rgba(255,255,255,.6)"><i data-lucide="check-circle-2" style="width:14px;height:14px;color:#a29bfe;flex-shrink:0"></i> Emoji search</li>
        </ul>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Security Section -->
   <section id="security" class="px-5 py-20 relative">
    <div class="gradient-blob" style="width:350px;height:350px;background:#6c5ce7;top:0;right:-80px"></div>
    <div class="max-w-6xl mx-auto scroll-section">
     <div class="text-center mb-10">
      <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full text-xs font-medium mb-4" style="background:rgba(0,206,201,.15);color:#00cec9"><i data-lucide="shield" style="width:12px;height:12px"></i> Security
      </div>
      <h2 id="security-heading" class="font-display font-bold text-3xl md:text-4xl mb-3" style="color:#fff">Secure &amp; Instant Connection</h2>
     </div>
     <div class="grid grid-cols-1 md:grid-cols-3 gap-5">
      <div class="rounded-2xl p-6 text-center card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mx-auto mb-4" style="background:rgba(0,206,201,.15)"><i data-lucide="phone-call" style="width:26px;height:26px;color:#00cec9"></i>
       </div>
       <h3 class="font-display font-semibold mb-2" style="color:#fff">HD Calls</h3>
       <p class="text-sm" style="color:rgba(255,255,255,.5)">Crystal-clear voice calls with secure connections. Sync contacts to start instantly.</p>
      </div>
      <div class="rounded-2xl p-6 text-center card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mx-auto mb-4" style="background:rgba(108,92,231,.15)"><i data-lucide="map-pin" style="width:26px;height:26px;color:#a29bfe"></i>
       </div>
       <h3 class="font-display font-semibold mb-2" style="color:#fff">Privacy Sharing</h3>
       <p class="text-sm" style="color:rgba(255,255,255,.5)">Share real-time location in chats with the ability to stop sharing at any time.</p>
      </div>
      <div class="rounded-2xl p-6 text-center card-hover" style="background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.06)">
       <div class="feature-icon mx-auto mb-4" style="background:rgba(253,203,110,.15)"><i data-lucide="mic" style="width:26px;height:26px;color:#fdcb6e"></i>
       </div>
       <h3 class="font-display font-semibold mb-2" style="color:#fff">Voice Notes</h3>
       <p class="text-sm" style="color:rgba(255,255,255,.5)">Record and send voice messages for a faster, more personal way to stay in touch.</p>
      </div>
     </div>
    </div>
   </section><!-- CTA -->
   <section class="px-5 py-20">
    <div class="max-w-3xl mx-auto text-center scroll-section rounded-3xl p-10 md:p-14 relative overflow-hidden" style="background:linear-gradient(135deg,#6c5ce7,#00cec9)">
     <h2 class="font-display font-bold text-3xl md:text-4xl mb-4" style="color:#fff">Ready to Connect?</h2>
     <p class="mb-8" style="color:rgba(255,255,255,.8);max-width:400px;margin-left:auto;margin-right:auto">Join millions already on Daryel. Your community is waiting.</p><button id="cta-bottom" class="px-10 py-4 rounded-full font-semibold text-lg transition-all hover:scale-105" style="background:#fff;color:#6c5ce7;box-shadow:0 4px 20px rgba(0,0,0,.2)">Download Now</button>
    </div>
   </section><!-- Footer -->
   <footer class="px-5 py-10" style="border-top:1px solid rgba(255,255,255,.06)">
    <div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center justify-between gap-4">
     <div class="flex items-center gap-2">
      <div class="w-7 h-7 rounded-lg flex items-center justify-center font-display font-black text-sm" style="background:#6c5ce7;color:#fff">
       D
      </div><span class="font-display font-semibold" style="color:rgba(255,255,255,.7)">Daryel</span>
     </div>
     <p class="text-xs" style="color:rgba(255,255,255,.3)">© 2025 Daryel. All rights reserved.</p>
    </div>
   </footer>
  </div>
  <script>
const defaultConfig = {
  background_color: '#0a0a1a',
  surface_color: 'rgba(255,255,255,0.04)',
  text_color: '#ffffff',
  primary_action: '#6c5ce7',
  secondary_action: '#00cec9',
  font_family: 'Outfit',
  font_size: 16,
  hero_title: 'Daryel',
  hero_subtitle: 'Explore, connect and share your interests with real people',
  hero_description: "It's simple, reliable, and private, so you can easily keep in touch with your friends and family. A lightweight, all-in-one social platform designed for slower networks too.",
  community_title: 'Build Your Community',
  creativity_title: 'Express Your Creativity',
  security_title: 'Secure & Instant Connection',
  performance_title: 'Lightning-Fast Performance',
  cta_button_text: 'Download Now'
};

function applyConfig(config) {
  const c = {...defaultConfig, ...config};
  const app = document.getElementById('app');
  app.style.background = c.background_color;

  const font = c.font_family || defaultConfig.font_family;
  const base = c.font_size || defaultConfig.font_size;
  document.querySelectorAll('.font-display').forEach(el => { el.style.fontFamily = `${font}, DM Sans, sans-serif`; });

  document.getElementById('hero-title').textContent = c.hero_title;
  document.getElementById('hero-title').style.color = c.text_color;
  document.getElementById('hero-title').style.fontSize = `${base * 3.5}px`;

  document.getElementById('hero-subtitle').textContent = c.hero_subtitle;
  document.getElementById('hero-subtitle').style.color = c.primary_action ? lighten(c.primary_action) : '#a29bfe';

  document.getElementById('hero-desc').textContent = c.hero_description;

  document.getElementById('community-heading').textContent = c.community_title;
  document.getElementById('community-heading').style.color = c.text_color;

  document.getElementById('creativity-heading').textContent = c.creativity_title;
  document.getElementById('creativity-heading').style.color = c.text_color;

  document.getElementById('security-heading').textContent = c.security_title;
  document.getElementById('security-heading').style.color = c.text_color;

  document.getElementById('performance-heading').textContent = c.performance_title;
  document.getElementById('performance-heading').style.color = c.text_color;

  document.querySelectorAll('#cta-nav, #cta-hero').forEach(b => { b.style.background = c.primary_action; });
  document.getElementById('cta-bottom').textContent = c.cta_button_text;
  document.getElementById('cta-bottom').style.color = c.primary_action;
  document.getElementById('nav-logo-bg').style.background = c.primary_action;
}

function lighten(hex) {
  try {
    let r = parseInt(hex.slice(1,3),16), g = parseInt(hex.slice(3,5),16), b = parseInt(hex.slice(5,7),16);
    r = Math.min(255, r + 50); g = Math.min(255, g + 50); b = Math.min(255, b + 50);
    return `rgb(${r},${g},${b})`;
  } catch(e) { return '#a29bfe'; }
}

if(window.elementSdk) {
  window.elementSdk.init({
    defaultConfig,
    onConfigChange: async (config) => applyConfig(config),
    mapToCapabilities: (config) => ({
      recolorables: [
        { get:()=>config.background_color||defaultConfig.background_color, set:(v)=>{config.background_color=v;window.elementSdk.setConfig({background_color:v})} },
        { get:()=>config.surface_color||defaultConfig.surface_color, set:(v)=>{config.surface_color=v;window.elementSdk.setConfig({surface_color:v})} },
        { get:()=>config.text_color||defaultConfig.text_color, set:(v)=>{config.text_color=v;window.elementSdk.setConfig({text_color:v})} },
        { get:()=>config.primary_action||defaultConfig.primary_action, set:(v)=>{config.primary_action=v;window.elementSdk.setConfig({primary_action:v})} },
        { get:()=>config.secondary_action||defaultConfig.secondary_action, set:(v)=>{config.secondary_action=v;window.elementSdk.setConfig({secondary_action:v})} }
      ],
      borderables: [],
      fontEditable: { get:()=>config.font_family||defaultConfig.font_family, set:(v)=>{config.font_family=v;window.elementSdk.setConfig({font_family:v})} },
      fontSizeable: { get:()=>config.font_size||defaultConfig.font_size, set:(v)=>{config.font_size=v;window.elementSdk.setConfig({font_size:v})} }
    }),
    mapToEditPanelValues: (config) => new Map([
      ['hero_title', config.hero_title||defaultConfig.hero_title],
      ['hero_subtitle', config.hero_subtitle||defaultConfig.hero_subtitle],
      ['hero_description', config.hero_description||defaultConfig.hero_description],
      ['community_title', config.community_title||defaultConfig.community_title],
      ['creativity_title', config.creativity_title||defaultConfig.creativity_title],
      ['security_title', config.security_title||defaultConfig.security_title],
      ['performance_title', config.performance_title||defaultConfig.performance_title],
      ['cta_button_text', config.cta_button_text||defaultConfig.cta_button_text]
    ])
  });
}

// Scroll reveal
const observer = new IntersectionObserver((entries) => {
  entries.forEach(e => { if(e.isIntersecting) { e.target.classList.add('visible'); observer.unobserve(e.target); }});
}, {threshold:0.15});
document.querySelectorAll('.scroll-section').forEach(el => observer.observe(el));

// Feature card expand/collapse functionality
document.querySelectorAll('.feature-card').forEach(card => {
  const main = card.querySelector('.feature-main');
  const sub = card.querySelector('.feature-sub');
  
  // Click main area to expand
  main.addEventListener('click', function(e) {
    e.stopPropagation();
    if(sub) {
      sub.classList.remove('hidden');
      main.style.display = 'none';
    }
  });
  
  // Click back button to collapse
  const backBtn = sub ? sub.querySelector('.back-btn') : null;
  if(backBtn) {
    backBtn.addEventListener('click', function(e) {
      e.stopPropagation();
      sub.classList.add('hidden');
      main.style.display = 'block';
    });
  }
});

lucide.createIcons();
</script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9f281c13b068545a',t:'MTc3NzIzMjk1NS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html># daryel
Social media
