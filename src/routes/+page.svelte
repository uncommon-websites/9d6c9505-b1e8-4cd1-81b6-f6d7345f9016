<script lang="ts">
  import Navbar from '$lib/Navbar.svelte';
  import Footer from '$lib/Footer.svelte';
  import Button from '$lib/Button.svelte';
</script>

<div class="min-h-screen font-sans text-dark bg-cream overflow-x-hidden">
  <Navbar />

  <!-- Hero Section -->
  <section class="pt-32 pb-16 px-4 sm:px-6 lg:px-8 max-w-7xl mx-auto text-center">
    <div class="mb-6">
      <span class="text-xs font-bold tracking-widest text-gray-500 uppercase">Tennis Bracket Challenges Reimagined</span>
    </div>
    <h1 class="text-5xl md:text-7xl font-serif mb-6 leading-tight">
      Turn Grand Slam tennis <br class="hidden md:block" /> into competitive brackets
    </h1>
    <p class="text-lg md:text-xl text-gray-600 max-w-2xl mx-auto mb-10 leading-relaxed">
      Create bracket challenges for every Grand Slam tournament. Get AI-powered match predictions, 
      compete with friends on group leaderboards, and track live updates throughout the tournament.
    </p>
    <div class="flex flex-col sm:flex-row items-center justify-center gap-4 mb-20">
      <Button href="https://app.brckt.io/group/create" type="primary">Create Your Bracket &rarr;</Button>
      <Button href="https://app.brckt.io/explore" type="outline">Explore Groups</Button>
    </div>

    <!-- Hero Image Placeholder -->
    <div class="relative w-full max-w-5xl mx-auto rounded-2xl overflow-hidden shadow-2xl border border-gray-200 bg-white aspect-[16/9] mb-16 group">
      <!-- Mock Bracket UI -->
      <div class="absolute inset-0 bg-gray-50 p-4">
        <div class="h-full w-full bg-white rounded-xl border border-gray-200 shadow-sm p-6 flex flex-col">
            <!-- Header of Mock UI -->
            <div class="flex items-center justify-between mb-6 border-b border-gray-100 pb-4">
                <div class="flex items-center gap-3">
                    <div class="w-8 h-8 rounded-full bg-primary-brand/20 flex items-center justify-center text-xs font-bold">🎾</div>
                    <div class="h-4 w-32 bg-gray-100 rounded"></div>
                    <span class="text-xs text-gray-400">US Open 2025</span>
                </div>
                <div class="flex gap-2">
                    <div class="h-8 px-3 bg-primary-brand/10 rounded flex items-center text-xs font-medium">Leaderboard</div>
                    <div class="h-8 px-3 bg-gray-100 rounded flex items-center text-xs">My Picks</div>
                </div>
            </div>
            <!-- Bracket Content -->
            <div class="flex-1 flex gap-4 overflow-hidden">
                <!-- Round 1 -->
                <div class="flex-1 space-y-2">
                    <div class="text-[10px] font-bold text-gray-400 mb-2">ROUND 1</div>
                    <div class="bg-gray-50 rounded p-2 text-xs flex justify-between items-center">
                        <span class="font-medium">Djokovic</span>
                        <span class="text-gray-400">1</span>
                    </div>
                    <div class="bg-gray-50 rounded p-2 text-xs flex justify-between items-center opacity-50">
                        <span>Qualifier</span>
                        <span class="text-gray-400">-</span>
                    </div>
                    <div class="bg-gray-50 rounded p-2 text-xs flex justify-between items-center">
                        <span class="font-medium">Alcaraz</span>
                        <span class="text-gray-400">3</span>
                    </div>
                    <div class="bg-gray-50 rounded p-2 text-xs flex justify-between items-center opacity-50">
                        <span>Player</span>
                        <span class="text-gray-400">-</span>
                    </div>
                </div>
                <!-- Round 2 -->
                <div class="flex-1 space-y-2">
                    <div class="text-[10px] font-bold text-gray-400 mb-2">ROUND 2</div>
                    <div class="bg-primary-brand/10 rounded p-2 text-xs flex justify-between items-center border-2 border-primary-brand/30">
                        <span class="font-bold">Djokovic</span>
                        <span class="text-primary-brand">✓</span>
                    </div>
                    <div class="h-8"></div>
                    <div class="bg-gray-50 rounded p-2 text-xs flex justify-between items-center">
                        <span class="font-medium">Alcaraz</span>
                        <span class="text-gray-400">?</span>
                    </div>
                </div>
                <!-- Semifinals -->
                <div class="flex-1 space-y-2">
                    <div class="text-[10px] font-bold text-gray-400 mb-2">SEMIFINALS</div>
                    <div class="bg-gray-50 rounded p-2 text-xs flex justify-between items-center">
                        <span>TBD</span>
                        <span class="text-gray-400">-</span>
                    </div>
                    <div class="h-16"></div>
                    <div class="bg-gray-50 rounded p-2 text-xs flex justify-between items-center">
                        <span>TBD</span>
                        <span class="text-gray-400">-</span>
                    </div>
                </div>
                <!-- Finals -->
                <div class="flex-1 flex items-center">
                    <div class="w-full">
                        <div class="text-[10px] font-bold text-gray-400 mb-2">FINAL</div>
                        <div class="bg-gray-50 rounded p-3 text-xs text-center">
                            <div class="text-2xl mb-1">🏆</div>
                            <div class="text-gray-400">Champion</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
      </div>
      
      <!-- Decorative Elements -->
      <div class="absolute -left-12 bottom-12 w-24 h-24 bg-primary-brand rounded-full blur-2xl opacity-20"></div>
      <div class="absolute -right-12 top-12 w-32 h-32 bg-primary-light rounded-full blur-2xl opacity-20"></div>

      <!-- Tennis Ball Icon -->
      <div class="absolute bottom-[-20px] right-[-20px] w-24 h-24 z-10 hidden md:block">
          <svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="50" cy="50" r="40" fill="#CCFF00" stroke="#333" stroke-width="2"/>
            <path d="M20 35 Q50 50 80 35" stroke="#333" stroke-width="2" fill="none"/>
            <path d="M20 65 Q50 50 80 65" stroke="#333" stroke-width="2" fill="none"/>
          </svg>
      </div>
    </div>

    <!-- Community -->
    <div class="text-center">
      <p class="text-sm text-gray-500 mb-6">Trusted by tennis fans across Reddit, Twitter, and tennis communities worldwide</p>
      <div class="flex flex-wrap justify-center items-center gap-8 md:gap-12 opacity-60">
        <!-- Reddit Tennis -->
        <span class="font-bold text-xl flex items-center gap-2"><div class="w-5 h-5 bg-orange-600 rounded-full"></div> r/tennis</span>
        <!-- ATP -->
        <span class="font-bold text-xl flex items-center gap-2"><div class="w-5 h-5 bg-blue-600 rounded"></div> ATP Tour</span>
        <!-- WTA -->
        <span class="font-bold text-xl flex items-center gap-2"><div class="w-5 h-5 bg-purple-600 rounded-full"></div> WTA</span>
        <!-- Grand Slams -->
        <span class="font-bold text-xl flex items-center gap-2"><div class="w-5 h-5 bg-green-700 rounded"></div> Grand Slams</span>
        <!-- Tennis Twitter -->
        <span class="font-bold text-xl flex items-center gap-2"><div class="w-5 h-5 bg-black rounded-full"></div> Tennis Twitter</span>
      </div>
    </div>
  </section>

  <!-- Stats Section -->
  <section id="tournaments" class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-3xl mx-auto">
        Every Grand Slam tournament, powered by AI predictions and live updates
      </h2>
      
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-16">
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">4 Majors</div>
          <div class="text-xs font-bold text-gray-400 tracking-widest uppercase">Grand Slam Coverage</div>
        </div>
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">128 Players</div>
          <div class="text-xs font-bold text-gray-400 tracking-widest uppercase">Per Tournament Draw</div>
        </div>
        <div class="bg-gray-50 p-8 rounded-2xl text-center">
          <div class="text-4xl font-serif font-medium mb-2">AI-Powered</div>
          <div class="text-xs font-bold text-gray-400 tracking-widest uppercase">Match Analysis</div>
        </div>
      </div>

      <!-- Grand Slam Cards Carousel -->
      <div class="flex gap-4 overflow-hidden relative">
        <div class="absolute inset-y-0 left-0 w-20 bg-gradient-to-r from-white to-transparent z-10"></div>
        <div class="absolute inset-y-0 right-0 w-20 bg-gradient-to-l from-white to-transparent z-10"></div>
        
        <div class="flex gap-4 animate-scroll">
            <!-- Australian Open -->
            <div class="w-64 h-80 bg-blue-100 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold flex items-center gap-1">
                    <div class="w-2 h-2 bg-blue-600 rounded-full"></div> January
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-blue-900/80 to-transparent p-4 text-white">
                    <div class="font-bold text-xl">Australian Open</div>
                    <div class="text-xs opacity-90">Melbourne • Hard Court</div>
                </div>
            </div>
            <!-- French Open -->
            <div class="w-64 h-80 bg-orange-100 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold flex items-center gap-1">
                    <div class="w-2 h-2 bg-orange-600 rounded-full"></div> May
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-orange-900/80 to-transparent p-4 text-white">
                    <div class="font-bold text-xl">French Open</div>
                    <div class="text-xs opacity-90">Paris • Clay Court</div>
                </div>
            </div>
            <!-- Wimbledon -->
            <div class="w-64 h-80 bg-green-100 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold flex items-center gap-1">
                    <div class="w-2 h-2 bg-green-700 rounded-full"></div> June
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-green-900/80 to-transparent p-4 text-white">
                    <div class="font-bold text-xl">Wimbledon</div>
                    <div class="text-xs opacity-90">London • Grass Court</div>
                </div>
            </div>
             <!-- US Open -->
            <div class="w-64 h-80 bg-purple-100 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold flex items-center gap-1">
                    <div class="w-2 h-2 bg-purple-600 rounded-full"></div> August
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-purple-900/80 to-transparent p-4 text-white">
                    <div class="font-bold text-xl">US Open</div>
                    <div class="text-xs opacity-90">New York • Hard Court</div>
                </div>
            </div>
             <!-- Duplicate for seamless scroll -->
            <div class="w-64 h-80 bg-blue-100 rounded-2xl flex-shrink-0 relative overflow-hidden group">
                <div class="absolute top-4 left-4 bg-white/90 backdrop-blur px-2 py-1 rounded-full text-xs font-bold flex items-center gap-1">
                    <div class="w-2 h-2 bg-blue-600 rounded-full"></div> January
                </div>
                <div class="absolute bottom-0 inset-x-0 bg-gradient-to-t from-blue-900/80 to-transparent p-4 text-white">
                    <div class="font-bold text-xl">Australian Open</div>
                    <div class="text-xs opacity-90">Melbourne • Hard Court</div>
                </div>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Comparison Section -->
  <section id="how-it-works" class="bg-dark text-white py-24 overflow-hidden">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-4">Tennis brackets <br /> reimagined with AI</h2>
      <p class="text-center text-gray-400 mb-16">From manual spreadsheets to intelligent predictions</p>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
        <!-- The Old Way -->
        <div>
          <h3 class="text-xl font-serif mb-2">Traditional Brackets</h3>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Fans create brackets in spreadsheets, manually track scores, and struggle to keep groups engaged throughout the tournament.
          </p>
          <div class="bg-gray-800/50 rounded-xl p-6 border border-gray-700 relative">
             <div class="space-y-3">
                <div class="flex items-center gap-2 text-sm">
                    <div class="w-4 h-4 bg-red-500/30 rounded flex items-center justify-center text-red-400 text-xs">✗</div>
                    <span class="text-gray-400">Manual score tracking</span>
                </div>
                <div class="flex items-center gap-2 text-sm">
                    <div class="w-4 h-4 bg-red-500/30 rounded flex items-center justify-center text-red-400 text-xs">✗</div>
                    <span class="text-gray-400">No match insights</span>
                </div>
                <div class="flex items-center gap-2 text-sm">
                    <div class="w-4 h-4 bg-red-500/30 rounded flex items-center justify-center text-red-400 text-xs">✗</div>
                    <span class="text-gray-400">Static spreadsheets</span>
                </div>
                <div class="flex items-center gap-2 text-sm">
                    <div class="w-4 h-4 bg-red-500/30 rounded flex items-center justify-center text-red-400 text-xs">✗</div>
                    <span class="text-gray-400">Bracket fatigue</span>
                </div>
             </div>
             <div class="mt-6 text-center">
                <div class="text-4xl mb-2">📊</div>
                <div class="text-xs text-gray-500">Excel Spreadsheet</div>
             </div>
          </div>
        </div>

        <!-- The Brckt Way -->
        <div>
          <h3 class="text-xl font-serif mb-2">The Brckt Way</h3>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            AI-powered predictions, automatic live updates, group leaderboards, and deep match analysis keep fans engaged all tournament long.
          </p>
          <div class="bg-primary-brand/20 rounded-xl p-6 border border-primary-brand/30 relative">
             <div class="space-y-3">
                <div class="flex items-center gap-2 text-sm">
                    <div class="w-4 h-4 bg-green-500 rounded flex items-center justify-center text-white text-xs">✓</div>
                    <span class="text-white font-medium">Live automatic updates</span>
                </div>
                <div class="flex items-center gap-2 text-sm">
                    <div class="w-4 h-4 bg-green-500 rounded flex items-center justify-center text-white text-xs">✓</div>
                    <span class="text-white font-medium">AI match analysis</span>
                </div>
                <div class="flex items-center gap-2 text-sm">
                    <div class="w-4 h-4 bg-green-500 rounded flex items-center justify-center text-white text-xs">✓</div>
                    <span class="text-white font-medium">Group leaderboards</span>
                </div>
                <div class="flex items-center gap-2 text-sm">
                    <div class="w-4 h-4 bg-green-500 rounded flex items-center justify-center text-white text-xs">✓</div>
                    <span class="text-white font-medium">Player statistics</span>
                </div>
             </div>
             <div class="mt-6 text-center">
                <div class="text-4xl mb-2">🎾</div>
                <div class="text-xs text-primary-brand font-bold">Brckt Platform</div>
             </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Features Section 1 -->
  <section id="features" class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-2xl mx-auto">
        Everything you need for the perfect bracket challenge
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Card 1: AI Analysis -->
        <div class="lg:col-span-2 bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden relative group">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">AI-powered match analysis</h3>
                <p class="text-gray-500 text-sm">Our custom tennis AI analyzes player stats, head-to-head records, recent form, and surface performance to help you make informed picks.</p>
            </div>
            <div class="bg-primary-brand/5 rounded-xl p-6 h-64 relative border border-primary-brand/10">
                <!-- AI Analysis Display -->
                <div class="bg-white rounded-xl p-4 shadow-sm mb-3">
                    <div class="flex items-center justify-between mb-3">
                        <div class="flex items-center gap-2">
                            <div class="w-8 h-8 bg-gray-200 rounded-full"></div>
                            <div>
                                <div class="text-sm font-bold">Djokovic</div>
                                <div class="text-xs text-gray-400">Seed #1</div>
                            </div>
                        </div>
                        <div class="text-primary-brand font-bold text-xl">68%</div>
                    </div>
                    <div class="space-y-1">
                        <div class="flex justify-between text-xs">
                            <span class="text-gray-500">H2H Record</span>
                            <span class="font-medium">5-2</span>
                        </div>
                        <div class="flex justify-between text-xs">
                            <span class="text-gray-500">Hard Court Win %</span>
                            <span class="font-medium">84%</span>
                        </div>
                        <div class="flex justify-between text-xs">
                            <span class="text-gray-500">Recent Form</span>
                            <span class="font-medium text-green-600">W-W-W-L-W</span>
                        </div>
                    </div>
                </div>
                <div class="text-center text-xs text-gray-400">
                    <span class="bg-primary-brand/10 px-2 py-1 rounded-full">✨ AI Prediction</span>
                </div>
            </div>
        </div>

        <!-- Card 2: Live Updates -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">Live tournament updates</h3>
                <p class="text-gray-500 text-sm">Automatic score updates and bracket progression throughout the tournament.</p>
            </div>
            <div class="bg-primary-brand/5 rounded-xl h-48 relative overflow-hidden flex items-center justify-center p-4">
                <div class="space-y-2 w-full">
                    <div class="bg-white p-2 rounded shadow-sm flex items-center justify-between">
                        <span class="text-xs font-medium">Match Complete</span>
                        <span class="text-xs text-green-600 font-bold">✓ LIVE</span>
                    </div>
                    <div class="bg-white p-2 rounded shadow-sm">
                        <div class="text-xs text-gray-500 mb-1">Round 1</div>
                        <div class="flex justify-between items-center">
                            <span class="text-sm font-bold">Djokovic</span>
                            <span class="text-xs text-primary-brand">Winner</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Card 3: Group Leaderboards -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-primary-brand/5 rounded-xl mb-6 p-4 relative">
                <div class="bg-white rounded-xl shadow-sm p-4 h-full w-full">
                    <div class="text-xs font-bold text-gray-400 mb-3">LEADERBOARD</div>
                    <div class="space-y-2">
                        <div class="flex items-center gap-2 bg-primary-brand/10 p-2 rounded">
                            <div class="w-6 h-6 bg-primary-brand text-white rounded-full flex items-center justify-center text-xs font-bold">1</div>
                            <div class="flex-1 text-xs font-medium">Sarah</div>
                            <div class="text-xs font-bold">124 pts</div>
                        </div>
                        <div class="flex items-center gap-2 p-2">
                            <div class="w-6 h-6 bg-gray-200 rounded-full flex items-center justify-center text-xs">2</div>
                            <div class="flex-1 text-xs">Mike</div>
                            <div class="text-xs">118 pts</div>
                        </div>
                        <div class="flex items-center gap-2 p-2">
                            <div class="w-6 h-6 bg-gray-200 rounded-full flex items-center justify-center text-xs">3</div>
                            <div class="flex-1 text-xs">Alex</div>
                            <div class="text-xs">112 pts</div>
                        </div>
                    </div>
                </div>
             </div>
             <h3 class="text-xl font-serif mb-2">Group leaderboards</h3>
             <p class="text-gray-500 text-sm">Compete with friends and see who has the best predictions in real-time.</p>
        </div>

        <!-- Card 4: Player Stats -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-primary-brand/5 rounded-xl mb-6 p-4 flex items-center justify-center">
                <div class="bg-white p-4 rounded-xl shadow-sm w-full">
                    <div class="flex items-center gap-3 mb-3">
                        <div class="w-12 h-12 bg-gray-200 rounded-full"></div>
                        <div>
                            <div class="text-sm font-bold">C. Alcaraz</div>
                            <div class="text-xs text-gray-400">Seed #3</div>
                        </div>
                    </div>
                    <div class="grid grid-cols-3 gap-2 text-center">
                        <div class="bg-gray-50 p-2 rounded">
                            <div class="text-xs font-bold">45-8</div>
                            <div class="text-[10px] text-gray-400">W-L</div>
                        </div>
                        <div class="bg-gray-50 p-2 rounded">
                            <div class="text-xs font-bold">82%</div>
                            <div class="text-[10px] text-gray-400">Win Rate</div>
                        </div>
                        <div class="bg-gray-50 p-2 rounded">
                            <div class="text-xs font-bold">#3</div>
                            <div class="text-[10px] text-gray-400">Rank</div>
                        </div>
                    </div>
                </div>
             </div>
             <h3 class="text-xl font-serif mb-2">Comprehensive player stats</h3>
             <p class="text-gray-500 text-sm">Access detailed statistics, career records, and head-to-head matchups.</p>
        </div>

        <!-- Card 5: Pick Counter -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 overflow-hidden">
             <div class="h-48 bg-primary-brand/5 rounded-xl mb-6 p-4 flex items-center justify-center relative">
                 <div class="bg-white p-6 rounded-xl shadow-sm text-center">
                    <div class="text-4xl font-serif font-bold text-primary-brand mb-2">124/128</div>
                    <div class="text-xs text-gray-500 mb-3">Picks Complete</div>
                    <div class="w-full bg-gray-100 rounded-full h-2">
                        <div class="bg-primary-brand h-2 rounded-full" style="width: 97%"></div>
                    </div>
                 </div>
             </div>
             <h3 class="text-xl font-serif mb-2">Pick counter & validation</h3>
             <p class="text-gray-500 text-sm">Never submit an incomplete bracket with our pick counter and validation system.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonial 1 -->
  <section class="py-16 bg-cream">
    <div class="max-w-4xl mx-auto px-4 text-center">
        <div class="flex justify-center mb-8">
            <div class="flex items-center gap-2 font-bold text-xl opacity-80">
                <div class="w-6 h-6 bg-orange-600 rounded-full"></div> r/tennis
            </div>
        </div>
        <blockquote class="text-2xl md:text-3xl font-serif leading-relaxed mb-8">
            "Brckt has completely changed how we run bracket challenges during Grand Slams. The AI predictions are surprisingly accurate, and the live updates keep everyone engaged throughout the tournament."
        </blockquote>
        <div class="flex items-center justify-center gap-4">
            <div class="w-12 h-12 rounded-full bg-gray-300"></div>
            <div class="text-left">
                <div class="font-bold text-sm">Alex M.</div>
                <div class="text-xs text-gray-500">Tennis Fan & Group Organizer</div>
            </div>
        </div>
    </div>
  </section>

  <!-- Features Section 2 -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16">
        Create, share, and compete <br /> with your tennis community
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Card 1 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-primary-brand/5 rounded-xl h-64 mb-8 p-4 relative overflow-hidden flex items-center justify-center">
                <div class="bg-white rounded-xl shadow-lg p-6 w-full max-w-sm">
                    <div class="text-center mb-4">
                        <div class="text-2xl mb-2">🎾</div>
                        <div class="text-sm font-bold mb-1">US Open 2025</div>
                        <div class="text-xs text-gray-400">Create Your Bracket</div>
                    </div>
                    <div class="space-y-2">
                        <div class="flex items-center gap-2 text-xs">
                            <div class="w-4 h-4 bg-green-500 rounded flex items-center justify-center text-white text-[10px]">✓</div>
                            <span>Men's Draw</span>
                        </div>
                        <div class="flex items-center gap-2 text-xs">
                            <div class="w-4 h-4 bg-green-500 rounded flex items-center justify-center text-white text-[10px]">✓</div>
                            <span>Women's Draw</span>
                        </div>
                        <div class="flex items-center gap-2 text-xs">
                            <div class="w-4 h-4 bg-primary-brand rounded flex items-center justify-center text-white text-[10px]">✓</div>
                            <span>Public & Private Groups</span>
                        </div>
                    </div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Men's & Women's tournaments</h3>
            <p class="text-gray-500 text-sm">Create brackets for both men's and women's draws. Support for all four Grand Slam tournaments throughout the season.</p>
        </div>

        <!-- Card 2 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-primary-brand/5 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                 <div class="bg-white rounded-xl shadow-lg p-4 w-3/4">
                    <div class="flex items-center justify-between mb-4">
                        <div class="text-sm font-bold">Share Group</div>
                        <div class="h-6 px-3 bg-primary-brand rounded text-white text-[10px] flex items-center justify-center">Copy Link</div>
                    </div>
                    <div class="space-y-2">
                        <div class="bg-gray-50 p-2 rounded text-xs">
                            <div class="text-gray-400 mb-1">Group Code</div>
                            <div class="font-mono font-bold">USOPEN2025</div>
                        </div>
                        <div class="flex gap-2">
                            <div class="h-8 w-8 bg-blue-100 rounded flex items-center justify-center text-xs">📱</div>
                            <div class="h-8 w-8 bg-green-100 rounded flex items-center justify-center text-xs">💬</div>
                            <div class="h-8 w-8 bg-purple-100 rounded flex items-center justify-center text-xs">✉️</div>
                        </div>
                    </div>
                 </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Public & private groups</h3>
            <p class="text-gray-500 text-sm">Create private groups for friends or public groups for the entire tennis community. Easy sharing via link or group code.</p>
        </div>

        <!-- Card 3 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-primary-brand/5 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                <div class="bg-white rounded-xl shadow-sm p-4 w-full max-w-sm">
                    <div class="text-xs font-bold text-gray-400 mb-3">MOBILE OPTIMIZED</div>
                    <div class="space-y-2">
                        <div class="bg-gray-50 p-3 rounded flex items-center gap-2">
                            <div class="text-xl">📱</div>
                            <div class="flex-1">
                                <div class="text-xs font-medium">Swipe Navigation</div>
                                <div class="text-[10px] text-gray-400">128-player draws</div>
                            </div>
                        </div>
                        <div class="bg-gray-50 p-3 rounded flex items-center gap-2">
                            <div class="text-xl">📌</div>
                            <div class="flex-1">
                                <div class="text-xs font-medium">Sticky Headers</div>
                                <div class="text-[10px] text-gray-400">Easy tracking</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Mobile-first experience</h3>
            <p class="text-gray-500 text-sm">Seamless mobile navigation with swipe functionality and sticky round headers for easy bracket management on any device.</p>
        </div>

        <!-- Card 4 -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="bg-primary-brand/5 rounded-xl h-64 mb-8 p-4 flex items-center justify-center">
                <div class="w-full max-w-sm">
                    <div class="bg-white rounded-xl shadow-lg p-4 mb-3">
                        <div class="flex items-center justify-between mb-2">
                            <span class="text-xs font-bold">Match Analysis</span>
                            <span class="text-xs text-primary-brand">AI</span>
                        </div>
                        <div class="text-xs text-gray-600 leading-relaxed">
                            "Djokovic holds a 5-2 H2H advantage and has won 84% of hard court matches this season..."
                        </div>
                    </div>
                    <div class="text-center text-[10px] text-gray-400">
                        Powered by custom tennis AI
                    </div>
                </div>
            </div>
            <h3 class="text-xl font-serif mb-2">Deep match insights</h3>
            <p class="text-gray-500 text-sm">Get AI-generated match breakdowns with head-to-head stats, surface performance, and recent form analysis for every matchup.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Join Tournament CTA -->
  <section class="py-24 bg-cream relative overflow-hidden">
    <!-- Floating Tennis Icons Background -->
    <div class="absolute inset-0 opacity-10 pointer-events-none">
        <div class="absolute top-10 left-10 w-12 h-12 text-4xl">🎾</div>
        <div class="absolute top-20 right-20 w-12 h-12 text-4xl">🏆</div>
        <div class="absolute bottom-20 left-1/3 w-12 h-12 text-4xl">🎾</div>
        <div class="absolute bottom-10 right-1/4 w-12 h-12 text-4xl">🏆</div>
    </div>

    <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
        <div class="inline-block bg-primary-brand/10 text-primary-brand px-4 py-1 rounded-full text-xs font-bold mb-6">
            Next Major: Check app.brckt.io
        </div>
        <h2 class="text-4xl md:text-6xl font-serif mb-4">Ready for the next <br /> Grand Slam?</h2>
        <p class="text-gray-500 mb-10">Join thousands of tennis fans competing in bracket challenges</p>
        
        <div class="flex justify-center gap-4">
            <Button href="https://app.brckt.io/group/create" type="primary">Create Your Bracket &rarr;</Button>
            <Button href="https://app.brckt.io/explore" type="white">Explore Groups</Button>
        </div>
    </div>
  </section>

  <!-- Tournament Season Section -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16">
        All four Grand Slams, <br /> one platform
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Left Large Card -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 md:row-span-2 flex flex-col">
            <div class="mb-8">
                <h3 class="text-xl font-serif mb-2">Complete Grand Slam coverage</h3>
                <p class="text-gray-500 text-sm">From Melbourne to New York, create brackets for every major tournament throughout the tennis season.</p>
            </div>
            <div class="flex-1 bg-primary-brand/5 rounded-2xl relative overflow-hidden min-h-[300px] p-6">
                <div class="space-y-4">
                    <div class="bg-white rounded-xl p-4 shadow-sm flex items-center justify-between">
                        <div>
                            <div class="font-bold text-sm mb-1">Australian Open</div>
                            <div class="text-xs text-gray-400">January • Melbourne</div>
                        </div>
                        <div class="text-2xl">🇦🇺</div>
                    </div>
                    <div class="bg-white rounded-xl p-4 shadow-sm flex items-center justify-between">
                        <div>
                            <div class="font-bold text-sm mb-1">French Open</div>
                            <div class="text-xs text-gray-400">May • Paris</div>
                        </div>
                        <div class="text-2xl">🇫🇷</div>
                    </div>
                    <div class="bg-white rounded-xl p-4 shadow-sm flex items-center justify-between">
                        <div>
                            <div class="font-bold text-sm mb-1">Wimbledon</div>
                            <div class="text-xs text-gray-400">June • London</div>
                        </div>
                        <div class="text-2xl">🇬🇧</div>
                    </div>
                    <div class="bg-white rounded-xl p-4 shadow-sm flex items-center justify-between">
                        <div>
                            <div class="font-bold text-sm mb-1">US Open</div>
                            <div class="text-xs text-gray-400">August • New York</div>
                        </div>
                        <div class="text-2xl">🇺🇸</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Right Top Card -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100">
            <div class="flex justify-between items-start mb-4">
                <div>
                     <h3 class="text-xl font-serif mb-2">Growing community</h3>
                     <p class="text-gray-500 text-sm">Join thousands of tennis fans who've discovered a better way to enjoy Grand Slam tournaments.</p>
                </div>
                <span class="bg-primary-brand/10 text-primary-brand px-2 py-1 rounded text-xs font-bold">Active</span>
            </div>
            <div class="bg-primary-brand/5 rounded-xl h-40 flex items-end p-4 gap-2">
                <div class="w-1/5 bg-primary-brand/30 h-[40%] rounded-t"></div>
                <div class="w-1/5 bg-primary-brand/50 h-[60%] rounded-t"></div>
                <div class="w-1/5 bg-primary-brand/70 h-[75%] rounded-t"></div>
                <div class="w-1/5 bg-primary-brand/90 h-[90%] rounded-t"></div>
                <div class="w-1/5 bg-primary-brand h-full rounded-t"></div>
            </div>
        </div>

        <!-- Right Bottom Card (Testimonial) -->
        <div class="bg-white rounded-3xl p-8 shadow-sm border border-gray-100 flex gap-6 items-center">
            <div class="w-24 h-24 bg-gray-200 rounded-full flex-shrink-0 overflow-hidden">
                <svg class="w-full h-full text-gray-400" fill="currentColor" viewBox="0 0 24 24"><path d="M24 24H0V0h24v24z" fill="none"/><path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"/></svg>
            </div>
            <div>
                <div class="text-primary-brand text-4xl font-serif leading-none mb-2">"</div>
                <p class="text-sm text-gray-600 italic mb-4">The AI predictions are surprisingly accurate and the live updates during matches keep our entire group engaged. Best bracket platform I've used.</p>
                <div class="text-xs font-bold">Jordan T.</div>
                <div class="text-[10px] text-gray-400">Tennis Enthusiast</div>
            </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Community Testimonials Grid -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif text-center mb-16 max-w-2xl mx-auto">
        Loved by tennis fans worldwide
      </h2>

      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
         <!-- Testimonial 1 -->
         <div class="bg-white rounded-2xl p-6 shadow-sm border border-gray-100">
            <div class="flex items-center gap-3 mb-4">
                <div class="w-10 h-10 bg-gray-200 rounded-full"></div>
                <div>
                    <div class="font-bold text-sm">Sarah M.</div>
                    <div class="text-xs text-gray-400">Tennis Fan</div>
                </div>
            </div>
            <p class="text-sm text-gray-600 leading-relaxed">"The AI predictions helped me win my group during the Australian Open. The insights are incredibly detailed!"</p>
         </div>

         <!-- Testimonial 2 -->
         <div class="bg-white rounded-2xl p-6 shadow-sm border border-gray-100">
            <div class="flex items-center gap-3 mb-4">
                <div class="w-10 h-10 bg-gray-200 rounded-full"></div>
                <div>
                    <div class="font-bold text-sm">Mike R.</div>
                    <div class="text-xs text-gray-400">Group Organizer</div>
                </div>
            </div>
            <p class="text-sm text-gray-600 leading-relaxed">"Finally, a bracket platform that doesn't require manual score updates. Live tracking is a game-changer."</p>
         </div>

         <!-- Testimonial 3 -->
         <div class="bg-white rounded-2xl p-6 shadow-sm border border-gray-100">
            <div class="flex items-center gap-3 mb-4">
                <div class="w-10 h-10 bg-gray-200 rounded-full"></div>
                <div>
                    <div class="font-bold text-sm">Alex K.</div>
                    <div class="text-xs text-gray-400">r/tennis Member</div>
                </div>
            </div>
            <p class="text-sm text-gray-600 leading-relaxed">"Best tennis bracket platform I've used. The mobile experience is smooth and the leaderboards keep everyone engaged."</p>
         </div>

         <!-- Testimonial 4 -->
         <div class="bg-white rounded-2xl p-6 shadow-sm border border-gray-100">
            <div class="flex items-center gap-3 mb-4">
                <div class="w-10 h-10 bg-gray-200 rounded-full"></div>
                <div>
                    <div class="font-bold text-sm">Emma L.</div>
                    <div class="text-xs text-gray-400">Tennis Enthusiast</div>
                </div>
            </div>
            <p class="text-sm text-gray-600 leading-relaxed">"Love the head-to-head stats and player analysis. Makes picking matches so much more informed and fun."</p>
         </div>

         <!-- Testimonial 5 -->
         <div class="bg-white rounded-2xl p-6 shadow-sm border border-gray-100">
            <div class="flex items-center gap-3 mb-4">
                <div class="w-10 h-10 bg-gray-200 rounded-full"></div>
                <div>
                    <div class="font-bold text-sm">Chris P.</div>
                    <div class="text-xs text-gray-400">Tournament Follower</div>
                </div>
            </div>
            <p class="text-sm text-gray-600 leading-relaxed">"The pick counter saved me from submitting an incomplete bracket. Great attention to detail on this platform."</p>
         </div>

         <!-- Testimonial 6 -->
         <div class="bg-white rounded-2xl p-6 shadow-sm border border-gray-100">
            <div class="flex items-center gap-3 mb-4">
                <div class="w-10 h-10 bg-gray-200 rounded-full"></div>
                <div>
                    <div class="font-bold text-sm">Taylor B.</div>
                    <div class="text-xs text-gray-400">Grand Slam Fan</div>
                </div>
            </div>
            <p class="text-sm text-gray-600 leading-relaxed">"Having both men's and women's brackets in one place is perfect. Can't wait for Wimbledon!"</p>
         </div>
      </div>
    </div>
  </section>

  <!-- Primary CTA Section -->
  <section class="bg-primary-brand py-24 relative overflow-hidden">
    <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
        <h2 class="text-4xl md:text-6xl font-serif mb-8 text-white">Make every Grand Slam <br /> more exciting</h2>
        
        <div class="flex flex-col md:flex-row justify-center gap-6 mb-10 text-sm font-medium text-white/90">
            <div class="flex items-center gap-2">
                <div class="bg-white text-primary-brand rounded-full p-0.5"><svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg></div>
                AI-powered match predictions
            </div>
            <div class="flex items-center gap-2">
                <div class="bg-white text-primary-brand rounded-full p-0.5"><svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg></div>
                Live updates & leaderboards
            </div>
        </div>

        <div class="flex justify-center gap-4">
            <Button href="https://app.brckt.io/group/create" type="white">Create Your Bracket &rarr;</Button>
        </div>
    </div>

    <!-- Bottom Tennis Court Lines -->
    <div class="absolute bottom-0 left-0 right-0 h-32 opacity-10 pointer-events-none flex items-end justify-center overflow-hidden">
        <svg width="1200" height="100" viewBox="0 0 1200 100" fill="none" xmlns="http://www.w3.org/2000/svg">
            <!-- Tennis court lines -->
            <line x1="0" y1="80" x2="1200" y2="80" stroke="white" stroke-width="3"/>
            <line x1="200" y1="60" x2="200" y2="100" stroke="white" stroke-width="2"/>
            <line x1="400" y1="60" x2="400" y2="100" stroke="white" stroke-width="2"/>
            <line x1="600" y1="40" x2="600" y2="100" stroke="white" stroke-width="3"/>
            <line x1="800" y1="60" x2="800" y2="100" stroke="white" stroke-width="2"/>
            <line x1="1000" y1="60" x2="1000" y2="100" stroke="white" stroke-width="2"/>
        </svg>
    </div>
  </section>

  <!-- FAQ -->
  <section class="py-24 bg-cream">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <h2 class="text-3xl md:text-5xl font-serif mb-16">Frequently Asked Questions</h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-x-12 gap-y-6">
        {#each [
            "What is Brckt?",
            "Which tournaments does Brckt cover?",
            "How does the AI prediction system work?",
            "Can I create private groups for friends?",
            "How are brackets scored?",
            "When do groups open for each tournament?",
            "Is there a mobile app?",
            "How do I join an existing group?"
        ] as question}
            <div class="border-b border-gray-200 py-4 flex justify-between items-center group cursor-pointer">
                <span class="font-medium text-lg group-hover:text-primary-brand transition-colors">{question}</span>
                <div class="w-6 h-6 rounded-full bg-dark text-white flex items-center justify-center text-sm group-hover:bg-primary-brand transition-colors">+</div>
            </div>
        {/each}
      </div>
    </div>
  </section>

  <Footer />
</div>

<style>
  /* Custom Scroll Animation */
  @keyframes scroll {
    0% { transform: translateX(0); }
    100% { transform: translateX(-50%); }
  }
  .animate-scroll {
    animation: scroll 20s linear infinite;
  }
  
  @keyframes spin-slow {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }
  .animate-spin-slow {
    animation: spin-slow 20s linear infinite;
  }
</style>

