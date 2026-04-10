---
type: PostLayout
title: How to Structure and Organize a Next.js Project 🗂️
colors: colors-a
date: '2024-06-03'
author: content/data/team/doris-soto.json
excerpt: More context that may or may not be helpful
featuredImage:
  type: ImageBlock
  url: /images/featured-Image6.jpg
  altText: Post thumbnail image
bottomSections:
  - elementId: ''
    type: RecentPostsSection
    colors: colors-f
    variant: variant-d
    subtitle: Recent posts
    showDate: true
    showAuthor: false
    showExcerpt: true
    recentCount: 2
    styles:
      self:
        height: auto
        width: wide
        padding:
          - pt-12
          - pb-56
          - pr-4
          - pl-4
        textAlign: left
    showFeaturedImage: true
    showReadMoreLink: true
  - type: ContactSection
    backgroundSize: full
    title: Stay up-to-date with my words ✍️
    colors: colors-f
    form:
      type: FormBlock
      elementId: sign-up-form
      fields:
        - name: firstName
          label: First Name
          hideLabel: true
          placeholder: First Name
          isRequired: true
          width: 1/2
          type: TextFormControl
        - name: lastName
          label: Last Name
          hideLabel: true
          placeholder: Last Name
          isRequired: false
          width: 1/2
          type: TextFormControl
        - name: email
          label: Email
          hideLabel: true
          placeholder: Email
          isRequired: true
          width: full
          type: EmailFormControl
        - name: updatesConsent
          label: Sign me up to recieve my words
          isRequired: false
          width: full
          type: CheckboxFormControl
      submitLabel: Submit 🚀
      styles:
        self:
          textAlign: center
    styles:
      self:
        height: auto
        width: narrow
        padding:
          - pt-24
          - pb-24
          - pr-4
          - pl-4
        flexDirection: row
        textAlign: left
---
<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Geopolitical Intelligence Brief | Hormuz Closure & Helium Crisis</title>
<style>
  \* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

:root {
\--navy: #080E1D;
\--blue: #1B4F8A;
\--teal: #1A7A6E;
\--amber: #D4830A;
\--red: #B22222;
\--grey: #8899BB;
\--lgrey: #E8ECF2;
\--ink: #1A1A2E;
}

body {
font-family: system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif;
background: #F4F6FA;
color: var(--ink);
font-size: 13px;
line-height: 1.5;
}

.page {
max-width: 1080px;
margin: 0 auto;
padding: 24px 16px;
}

.topbar {
display: flex;
justify-content: space-between;
align-items: center;
margin-bottom: 18px;
flex-wrap: wrap;
gap: 8px;
}
.topbar-l {
font-size: 11px;
color: var(--grey);
font-weight: 700;
letter-spacing: 1.5px;
text-transform: uppercase;
}
.topbar-r {
font-size: 11px;
color: var(--amber);
font-weight: 700;
letter-spacing: 1px;
text-transform: uppercase;
}

.cover {
background: var(--navy);
color: #fff;
border-radius: 14px;
padding: 32px 36px;
margin-bottom: 24px;
}
.cover-meta {
font-size: 10px;
color: var(--grey);
letter-spacing: 2px;
font-weight: 700;
text-transform: uppercase;
margin-bottom: 6px;
}
.cover-tag {
font-size: 11px;
color: var(--amber);
font-weight: 700;
letter-spacing: 1px;
text-transform: uppercase;
margin-bottom: 10px;
}
.cover h1 {
font-size: 22px;
font-weight: 800;
line-height: 1.3;
margin-bottom: 16px;
}
.cover-summary {
font-size: 13px;
line-height: 1.75;
color: #B8C8E0;
margin-bottom: 18px;
}
.cover-lens {
background: rgba(255,255,255,0.07);
border-radius: 8px;
padding: 9px 14px;
font-size: 12px;
margin-bottom: 18px;
}
.l-label { color: var(--teal); font-weight: 700; }
.l-name { color: #fff; font-weight: 600; }
.l-why { color: var(--grey); }
.wl-row {
display: flex;
gap: 24px;
flex-wrap: wrap;
}
.wl-title {
font-size: 10px;
color: var(--grey);
letter-spacing: 1px;
text-transform: uppercase;
margin-bottom: 5px;
}
.tags {
display: flex;
gap: 6px;
flex-wrap: wrap;
}
.tag {
display: inline-block;
border-radius: 4px;
padding: 2px 8px;
font-size: 10px;
font-weight: 700;
letter-spacing: 0.5px;
text-transform: uppercase;
color: #fff;
}
.tag-teal { background: var(--teal); }
.tag-red { background: var(--red); }

.sec-title {
font-size: 11px;
font-weight: 800;
text-transform: uppercase;
letter-spacing: 1.2px;
color: var(--navy);
margin-bottom: 12px;
}

.events-grid {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(190px, 1fr));
gap: 10px;
margin-bottom: 24px;
}
.ev {
background: var(--lgrey);
border-radius: 10px;
padding: 11px 13px;
border-left: 4px solid var(--blue);
}
.ev-dom {
font-size: 11px;
font-weight: 700;
color: var(--navy);
margin-bottom: 3px;
}
.ev-dev {
font-size: 12px;
line-height: 1.5;
margin-bottom: 5px;
}
.ev-metric {
font-size: 11px;
color: var(--teal);
font-weight: 700;
}
.ev-src {
font-size: 10px;
color: var(--grey);
margin-top: 3px;
}

hr {
border: none;
border-top: 2px solid var(--lgrey);
margin: 20px 0;
}

.persp {
margin-bottom: 24px;
overflow-x: auto;
}
table {
width: 100%;
border-collapse: collapse;
font-size: 11.5px;
min-width: 680px;
}
thead th {
background: var(--navy);
color: var(--amber);
padding: 8px 11px;
text-align: left;
font-weight: 700;
}
thead th.pc { color: #fff; }
tbody td {
padding: 8px 11px;
line-height: 1.5;
vertical-align: top;
}
tbody tr:nth-child(even) td { background: var(--lgrey); }
tbody tr:nth-child(odd) td { background: #fff; }
.pname {
font-weight: 700;
color: var(--navy);
white-space: nowrap;
}

.two-col {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 24px;
}
@media (max-width: 640px) {
.two-col { grid-template-columns: 1fr; }
}

.quotes {
display: flex;
flex-direction: column;
gap: 9px;
margin-bottom: 24px;
}
.qcard {
background: #F0F4FA;
border-left: 4px solid var(--amber);
border-radius: 8px;
padding: 11px 14px;
}
.qtext {
font-size: 12px;
font-style: italic;
line-height: 1.65;
margin-bottom: 5px;
}
.qattr {
font-size: 11px;
color: var(--grey);
}
.qattr strong { color: var(--navy); }

.media {
display: flex;
flex-direction: column;
gap: 9px;
margin-bottom: 24px;
}
.mcard {
background: #fff;
border: 1px solid var(--lgrey);
border-radius: 10px;
padding: 11px 13px;
display: flex;
gap: 9px;
align-items: flex-start;
}
.mbadge {
border-radius: 4px;
padding: 3px 7px;
font-size: 10px;
font-weight: 700;
color: #fff;
white-space: nowrap;
flex-shrink: 0;
}
.b-read { background: var(--blue); }
.mtitle {
font-size: 12px;
font-weight: 700;
color: var(--navy);
line-height: 1.4;
margin-bottom: 2px;
}
.msrc {
font-size: 10px;
color: var(--teal);
font-weight: 600;
margin-bottom: 3px;
}
.mwhy {
font-size: 11px;
color: var(--grey);
}

.footer {
background: var(--navy);
border-radius: 12px;
padding: 20px 26px;
}
.footer-grid {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 18px;
margin-bottom: 16px;
}
@media (max-width: 520px) {
.footer-grid { grid-template-columns: 1fr; }
}
.flabel {
font-size: 10px;
font-weight: 700;
letter-spacing: 1px;
text-transform: uppercase;
margin-bottom: 5px;
}
.fa { color: var(--amber); }
.ft { color: var(--teal); }
.ftext {
font-size: 12px;
color: #B8C8E0;
line-height: 1.6;
}
.fcred {
border-top: 1px solid rgba(255,255,255,0.1);
padding-top: 12px;
font-size: 10px;
color: var(--grey);
text-align: center;
line-height: 1.8;
}


</head>
<body>
<div class="page">

<div class="topbar">
  <span class="topbar-l">🌐 Geopolitical Intelligence Newsletter</span>
  <span class="topbar-r">Hormuz Closure — Essential Gases & Semiconductors</span>
</div>

<div class="cover">
  <div class="cover-meta">Geopolitical Intelligence Brief · April 8, 2026</div>
  <div class="cover-tag">Hormuz Closure — Essential Gases, Semiconductors & Data Center Costs</div>
  <h1>Qatar's Helium Tap Is Off: The Six-Month Clock Ticking on Chips, AI and Data Centers</h1>
  <p class="cover-summary">Iranian drone strikes on Qatar's Ras Laffan Industrial City on March 2 shut down one of only two plants on Earth producing semiconductor-grade helium, removing 27–30% of global supply overnight. With \~200 cryogenic containers stranded in the Gulf — each capable of keeping helium liquid for only 35–48 days — South Korean and Taiwanese fabs face a hard supply cliff in early April. Spot helium prices have surged 40–100%. Compounding the crisis: European LNG prices rose 60%, directly inflating AI data center energy costs; HDD prices are up 46%; and HP, Dell and Lenovo have warned enterprise clients of 15–20% price hikes for H2 2026. Even if the Strait reopened today, Kornbluth Helium Consulting estimates supply chains need a minimum of 2–4 extra months to normalise.</p>
  <div class="cover-lens">
    <span class="l-label">📐 Lens: </span>
    <span class="l-name">Kindleberger Spiral</span>
    <span class="l-why"> — A single chokepoint failure cascades into overlapping shortages — helium, LNG, aluminium, bromine — each amplifying the next with no single actor able to arrest the spiral alone.</span>
  </div>
  <div class="wl-row">
    <div>
      <div class="wl-title">Net Winners</div>
      <div class="tags"><span class="tag tag-teal">Linde</span><span class="tag tag-teal">Air Products</span><span class="tag tag-teal">N. American Helium</span><span class="tag tag-teal">Pulsar Helium</span></div>
    </div>
    <div>
      <div class="wl-title">Net Losers</div>
      <div class="tags"><span class="tag tag-red">Samsung</span><span class="tag tag-red">SK Hynix</span><span class="tag tag-red">Taiwan Fabs</span><span class="tag tag-red">Data Centers</span><span class="tag tag-red">OEM Buyers</span></div>
    </div>
  </div>
</div>

<div class="sec-title">📋 Key Developments</div>
<div class="events-grid">
  <div class="ev"><div class="ev-dom">💰 Helium Spot Price</div><div class="ev-dev">Spot helium surged 40–100% since war began. Ultra-pure semiconductor-grade helium doubled in price.</div><div class="ev-metric">📊 +40–100% spot; ultra-pure grade ×2</div><div class="ev-src">— IndexBox / Carra Globe / CNBC</div></div>
  <div class="ev"><div class="ev-dom">💰 LNG & Data Center Energy</div><div class="ev-dev">European LNG prices rose 60%. AI data center energy costs rising with a 4–8 week materialisation lag into April–May 2026.</div><div class="ev-metric">📊 LNG +60%; compute cost curve steepening</div><div class="ev-src">— abhs.in / Tom's Hardware</div></div>
  <div class="ev"><div class="ev-dom">🚢 The Container Clock</div><div class="ev-dev">\~200 cryogenic ISO containers stranded near the Strait, each worth $1M. Helium stays liquid for only 35–48 days — the six-week evaporation deadline is now.</div><div class="ev-metric">📊 200 containers; 35–48 day window</div><div class="ev-src">— Fortune / Scientific American / C\&EN</div></div>
  <div class="ev"><div class="ev-dom">🚢 Cape Rerouting Fails Helium</div><div class="ev-dev">Cape of Good Hope adds \~3,500 nautical miles and 10–14 days — helium boils off before arrival, making rerouting physically impossible for cryogenic shipments.</div><div class="ev-metric">📊 +$1M fuel cost; boil-off risk at 14+ days</div><div class="ev-src">— J2 Sourcing AB</div></div>
  <div class="ev"><div class="ev-dom">💻 Ras Laffan Offline</div><div class="ev-dev">QatarEnergy declared force majeure March 4. 33% of global helium supply offline for 3–5 years. One of only two semiconductor-grade helium plants on Earth.</div><div class="ev-metric">📊 33% offline; 3–5 year repair timeline</div><div class="ev-src">— C\&EN / NewsNation / Tom's Hardware</div></div>
  <div class="ev"><div class="ev-dom">💻 HDD & Chip Crisis</div><div class="ev-dev">HDD prices up 46% since Sept 2025. Western Digital sold out all of 2026. TSMC CoWoS packaging for Nvidia Blackwell GPUs fully booked through mid-2026.</div><div class="ev-metric">📊 WD sold out 2026; CoWoS fully booked</div><div class="ev-src">— Tom's Hardware / J2 Sourcing</div></div>
  <div class="ev"><div class="ev-dom">🌐 Data Center Strikes</div><div class="ev-dev">Iran claims strikes on Oracle's Dubai data center and Amazon's Bahrain facility. AWS Bahrain suffered major disruption. Half of planned US data center builds delayed or cancelled.</div><div class="ev-metric">📊 15–20% OEM price hike warnings issued</div><div class="ev-src">— Tom's Hardware / IDC / Medium</div></div>
</div>

<hr>

<div class="persp">
  <div class="sec-title">🌐 Party Perspectives</div>
  <table>
    <thead><tr><th class="pc">Party</th><th>💰 Economics & Energy</th><th>🚢 Trade & Logistics</th><th>💻 Tech & AI</th><th>🌐 Global Development</th></tr></thead>
    <tbody>
      <tr><td class="pname">🇺🇸 US / West</td><td>Linde (+15%) and Air Products (+14%) are 2026's surprise stock winners. JPMorgan upgraded Linde; Wells Fargo upgraded Air Products to overweight. US industrial gas firms are benefiting commercially from the crisis they geopolitically helped trigger.</td><td>North American fabs (GlobalFoundries) insulated by domestic US helium production and long-term contracts. But half of planned US data center builds are delayed or cancelled due to energy costs and parts shortages from China.</td><td>Iran struck AWS Bahrain and Oracle Dubai data centers directly. AI inference costs rising. Cloud hyperscalers on variable-rate compute most exposed; fixed-rate reserved instances provide short-term buffer.</td><td>The SIA warned in 2023 that a helium disruption "would send shocks through global semiconductor manufacturing" — that forecast is now reality. Congressional interest in domestic helium reserve legislation is accelerating.</td></tr>
      <tr><td class="pname">🇨🇳 China</td><td>One-third of China's total LNG use comes through the Strait. Energy costs for Chinese chip fabs rising. China's existing gallium export ban compounds chip material prices — chip materials have doubled.</td><td>China's semiconductor industry lags 5–10 years in AI data center chips — helium crisis hits it less acutely than TSMC/Samsung/SK Hynix. But CATL and BYD face aluminium cost pressures from Gulf smelter disruptions.</td><td>Huawei and SMIC accelerating domestic helium sourcing strategy. China's gallium export ban layered on the helium shortage creates a dual leverage position for any future semiconductor negotiation.</td><td>Xinhua highlights Russia's Amur plant failure leaves the West without an alternative. Chinese state media frames the shortage as proof of Western supply chain fragility.</td></tr>
      <tr><td class="pname">🇷🇺 Russia</td><td>Russia's Amur Gas Processing Plant was projected to supply 25% of global helium but has been plagued by explosions, delays, and sanctions — still well below capacity. Russia cannot capitalise on the shortage.</td><td>Specialised cryogenic ISO containers have no Russian equivalent routing. The shadow fleet that moved oil cannot move liquid helium at -268.9°C. Moscow cannot reroute Qatari helium.</td><td>RT frames the semiconductor shortage as evidence that "Western AI supremacy rests on a single Qatari gas plant" — geopolitically convenient, factually accurate.</td><td>Russia's strategic embarrassment: it profits from oil price elevation but cannot exploit the helium shortage because Amur is broken.</td></tr>
      <tr><td class="pname">🇮🇳 India</td><td>India is not a major helium consumer — semiconductor manufacturing is nascent. But the India Semiconductor Mission's fab ambitions face higher equipment and material import costs as chip prices rise 15–20%.</td><td>Indian IT sector benefits from nearshoring demand but faces rising cloud infrastructure costs as AWS and Azure pass through energy surcharges.</td><td>India has no domestic helium production of note. Its non-aligned position lets it negotiate supply access from both US producers and Central Asian sources without political friction.</td><td>India quietly lobbies for inclusion in any post-crisis helium supply diversification framework — positioning itself as a neutral hub.</td></tr>
      <tr><td class="pname">🇩🇪 Europe</td><td>Europe is "already feeling the pinch". LNG prices up 60% inflating industrial energy costs. Air Liquide benefits on revenue but faces logistical stress managing reallocation across hospital and fab customers.</td><td>Euronews reported MRI services at risk. European hospitals face helium rationing — medical use is being prioritised over industrial.</td><td>AI training runs in European HPC facilities throttled — both energy cost and helium allocation for cooling superconducting magnets. CERN activated contingency helium conservation protocols.</td><td>Der Spiegel frames it as "the hidden cost of the Middle East war that nobody explained to voters".</td></tr>
      <tr><td class="pname">🇯🇵 Japan</td><td>Japan is among the biggest consumers of Qatari LNG and helium. Iwatani Corporation is managing emergency reallocation. Renesas and Sony Semiconductor on the six-week supply clock.</td><td>South Korea and Taiwan "are feeling the shortage the most" per NPR, but Japan is closely behind. Trading houses activated emergency sourcing from US producers, paying spot premiums of 40–100%.</td><td>METI activated a helium allocation task force — assigning priority tiers: defence and medical first, semiconductors second, consumer electronics last.</td><td>Japan formally requested the US increase helium export allocation as part of the bilateral security relationship — framing semiconductor-grade helium as a defence-critical material.</td></tr>
      <tr><td class="pname">🌍 Global South</td><td>HP, Dell, Lenovo, Acer and ASUS warned enterprise clients of 15–20% price hikes for H2 2026. For emerging market consumers, smartphones, laptops and tablets are about to become materially more expensive.</td><td>Fertiliser and food price shocks hit the Global South hardest but chip inflation compounds it. A farmer in Egypt faces higher fuel, fertiliser, AND higher mobile device costs simultaneously.</td><td>Global South data centre programmes in Africa and Southeast Asia face double jeopardy: higher server hardware costs AND higher energy costs from LNG disruption.</td><td>Al Jazeera frames the helium crisis as "a rich-world technology problem with poor-world consequences" — the semiconductor shortage delays affordable 4G/5G device availability in developing markets by 12–18 months.</td></tr>
    </tbody>
  </table>
</div>

<hr>

<div class="two-col">
  <div>
    <div class="sec-title">💬 Key Quotes</div>
    <div class="quotes">
      <div class="qcard"><div class="qtext">"The world can't compensate for the loss of a third of its helium supply."</div><div class="qattr">— <strong>Phil Kornbluth</strong> · C\&EN</div></div>
      <div class="qcard"><div class="qtext">"It's kind of like a nice sunny day on the beach, but you heard there's a tsunami out there."</div><div class="qattr">— <strong>Phil Kornbluth</strong> · Scientific American</div></div>
      <div class="qcard"><div class="qtext">"About 33% of the world's helium supply is offline for at least the next three to five years."</div><div class="qattr">— <strong>Cliff Cain, President, Pulsar Helium</strong> · NewsNation</div></div>
      <div class="qcard"><div class="qtext">"A prolonged regional conflict could potentially disrupt chipmakers' manufacturing operations regarding sourcing materials like helium and bromine."</div><div class="qattr">— <strong>Ray Wang, SemiAnalysis</strong> · CNBC</div></div>
      <div class="qcard"><div class="qtext">"If helium went up 10x or 100x, then it would start to be a big problem for semiconductors."</div><div class="qattr">— <strong>Scotten W. Jones</strong> · NPR</div></div>
    </div>
  </div>
  <div>
    <div class="sec-title">📺 Worth Reading</div>
    <div class="media">
      <div class="mcard"><span class="mbadge b-read">📰 READ</span><div><div class="mtitle">Iran war disrupts global helium supply and AI chipmakers</div><div class="msrc">Scientific American</div><div class="mwhy">The container clock, MRI/chip priority, Kornbluth's full analysis</div></div></div>
      <div class="mcard"><span class="mbadge b-read">📰 READ</span><div><div class="mtitle">Qatar helium shutdown puts chip supply on a two-week clock</div><div class="msrc">Tom's Hardware</div><div class="mwhy">SK Hynix exposure, HDD crisis, evaporation window mechanics</div></div></div>
      <div class="mcard"><span class="mbadge b-read">📰 READ</span><div><div class="mtitle">Strait of Hormuz closure deflates global helium supply</div><div class="msrc">NPR</div><div class="mwhy">South Korea and Taiwan shortage timeline clearly explained</div></div></div>
      <div class="mcard"><span class="mbadge b-read">📰 READ</span><div><div class="mtitle">Helium hitch: Why Iran war could cause MRI scan delays</div><div class="msrc">Al Jazeera</div><div class="mwhy">Medical rationing, MRI at risk, Global South consequences</div></div></div>
      <div class="mcard"><span class="mbadge b-read">📰 READ</span><div><div class="mtitle">Hormuz LNG disruption and AI data center energy costs</div><div class="msrc">abhs.in</div><div class="mwhy">Quantification of AI compute cost inflation — LNG-to-data-center chain</div></div></div>
    </div>
  </div>
</div>

<hr>

<div class="footer">
  <div class="footer-grid">
    <div>
      <div class="flabel fa">👁 Watch Next 7 Days</div>
      <div class="ftext">Early April fab allocation cuts from Samsung and SK Hynix as the six-week container clock expires. Watch for formal force majeure declarations from Linde and Air Liquide — that is the signal a full global shortage is confirmed.</div>
    </div>
    <div>
      <div class="flabel ft">⚖️ Media Bias Note</div>
      <div class="ftext">Western tech press focuses on stock winners and fab risk. Al Jazeera and NPR lead with medical rationing and Global South consumer price impact — same crisis, opposite frame, both factually accurate.</div>
    </div>
  </div>
  <div class="fcred">Geopolitical Intelligence Newsletter · April 8, 2026 · Geopolitical Scan Framework v1.1Sources: Scientific American · Tom's Hardware · CNBC · NPR · Al Jazeera · C\&EN · Fortune · IndexBox · J2 Sourcing · PolitiFact · NewsNation · abhs.in</div>
</div>

</div>
</body>
</html>

