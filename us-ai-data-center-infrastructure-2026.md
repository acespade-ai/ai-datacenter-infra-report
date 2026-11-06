# US AI and Data Center Infrastructure: State of Play, November 2026

**Research report — prepared November 5, 2026**
**Scope:** the current state of AI and data center infrastructure in the United States (capacity, major builds, power and energy constraints, policy), and where AI and data-center investment and buildout could go if not in the US.

---

## 1. Executive summary

The United States is in the middle of the largest physical infrastructure buildout in its modern history, and the binding constraint is no longer chips, land, or capital — it is electricity. US data center operating capacity sits at roughly 51–57 GW, with Goldman Sachs projecting capacity of about 64 GW by the end of 2026 and 90 GW by the end of 2027, and power demand growing about 38% a year [1][2][3]. The four largest hyperscalers (Amazon, Microsoft, Alphabet, Meta) are guiding to roughly $700–750 billion in combined 2026 capital expenditure, up about 77% from around $410 billion in 2025 [4][5].

But the pipeline is far larger than what can actually be built. Developers have requested more than 1,000 GW of power from US utilities; Wood Mackenzie estimates only about 28% of it will ever be committed to real projects [1]. About half of the 12 GW of US data-center capacity planned for 2026 has been delayed or cancelled, and the median wait to connect new generation to the grid is now about five years [6][7]. The industry's response has been to buy power directly — multi-decade nuclear contracts, on-site gas and fuel cells, and gigawatt-scale campuses built around dedicated generation — and to push into new regions (Texas, Ohio, Indiana, Louisiana) as the original hub, Northern Virginia, tightens permitting and faces community opposition. Outside the US, the Gulf states are the most aggressive alternative, with sovereign-funded gigawatt campuses, while Europe is moving much more slowly and remains a small share of global AI compute.

The honest bottom line: announced capacity is not capacity. Roughly 6 GW is actually running at the 18 largest US AI campuses combined, against about 30 GW announced for those sites alone [8].

---

## 2. How big is the buildout?

**Operating capacity.** Independent trackers converge on a US operating base of 46–57 GW as of mid-2026: Bernstein puts it at about 51 GW (roughly 26 GW hyperscaler, 20 GW colocation), CleanView at 57.4 GW across 1,208 projects, and Aterio at 46 GW [9]. AI-only data centers are about 12% of operating capacity, but 50–62% of capacity under construction [9].

**Growth rate.** Goldman Sachs expects US data-center power demand to climb from 31 GW in 2025 to 41 GW in 2026 and 66 GW in 2027 — roughly 38% growth in each of 2026 and 2027 — on capacity reaching about 95 GW by the end of 2027 [2][3]. Scheduled capacity additions jump from 6.4 GW in 2024 and 8.5 GW in 2025 to 13.6 GW in 2026 and 36.3 GW in 2027, though Goldman expects only 50–60% of near-term scheduled capacity to come online on time [2][10].

**Money.** The four hyperscalers are guiding to roughly $725 billion in combined 2026 capex: Amazon about $200 billion, Alphabet $175–185 billion (later raised toward $195–205 billion), Microsoft about $190 billion for fiscal 2026, and Meta $125–145 billion after two mid-year raises [4][5][11]. Morgan Stanley's CEO told investors data-center capex is "coming in at about $850 billion" for 2026, with 2027 projected at $1.3 trillion [4]. The IEA reports the largest technology companies' capex exceeded $400 billion in 2025 and is expected to jump another 75% in 2026 [4]. US data-center construction spending hit a seasonally adjusted annual rate of $84.95 billion in August 2026, up about 73% year on year [11]. JLL expects nearly 100 GW of new data-center capacity globally between 2026 and 2030, with total investment including fit-out of up to $3 trillion [10].

**Market tightness.** CBRE counted 7,481 MW under construction across eight primary North American markets in the first half of 2026 — a record — with vacancy at just 1.4% and more than 80% of the pipeline already pre-leased. Northern Virginia alone holds 4,496.5 MW of inventory at 0.2% vacancy [11].

**Demand share.** Data centers used about 4.7% of US electricity in 2024; Lawrence Berkeley National Laboratory (LBNL) projects that share reaching about 12% by 2030 (range 9.5–15.3%) [7]. McKinsey projects US data-center power demand more than tripling from roughly 25 GW in 2024 to more than 80 GW by 2030, moving from 3–4% to 11–12% of total US electricity demand [12]. Gartner forecasts power shortages will restrict 40% of existing AI data centers by 2027 [12].

---

## 3. The major builds

The buildout has shifted from 20–50 MW cloud facilities to 500 MW–2 GW AI campuses. The table below separates announced capacity from estimated running power, using Epoch AI's satellite-based estimates where available — the gap between the two columns is the story of 2026.

| Project | Operator / tenant | Location | Announced capacity | Estimated running power (Oct 2026) | Status |
|---|---|---|---|---|---|
| Project Rainier | Amazon (AWS) for Anthropic | New Carlisle, Indiana | ~2.2 GW | ~1,037 MW | Operating since Oct 2025, expanding; ~500,000 Trainium2 chips [8] |
| Colossus 2 | xAI (now part of SpaceX) | Memphis, Tennessee | ~2 GW | ~946 MW | Operating, expanding; mostly on-site gas power [8] |
| Stargate Abilene | Oracle for OpenAI (Crusoe) | Abilene, Texas | ~1.2 GW | ~421 MW (Epoch projects ~843 MW by Q4 2026) | Partly operating; 6 of 8 buildings (618 MW) delivered by Sept 2026 [8][13] |
| Prometheus | Meta | New Albany, Ohio | ~1 GW | ~471 MW | Serving training jobs while still under construction [8] |
| Hyperion | Meta (Blue Owl JV) | Richland Parish, Louisiana | Up to 5 GW | Not yet operating | Under construction; >$50B investment; Phase 1 ~1.5 GW targeted late 2027 [8][13] |
| PORTS-Pike | SB Energy for OpenAI | Piketon, Ohio | ~8 GW IT | Not yet operating | First 800 MW expected 2028 [14] |
| Stargate (program) | OpenAI / Oracle / SoftBank / MGX | 7 US sites | 10 GW target; >9 GW planned | — | $500B program announced Jan 2025 [13][14] |
| Susquehanna campus | Amazon (AWS) / Talen Energy | Salem Township, Pennsylvania | 1.9 GW | — | Nuclear-powered; acquired for $650M [13] |

Other notable scale: Fermi America's Project Matador in Texas carries the largest headline figure at up to 17 GW, but that describes potential power generation rather than installed AI computing [14]. Across the 18 largest US AI campuses, about 30 GW is announced but only about 6 GW is actually running, and 10 of the 18 have nothing switched on yet [15].

---

## 4. Power and energy: the binding constraint

**The interconnection queue.** The US generation interconnection queue holds about 2,061 GW across roughly 8,200 projects — about 1.5 times the entire existing US generating fleet — with a median journey of about 61 months (five years) from interconnection request to commercial operation, up from 22 months in 2008. Only about 13% of capacity that entered queues from 2000–2020 ever reached operation [6].

**Regional pressure.** ERCOT's large-load interconnection queue went from 63 GW at the end of 2024 to about 226 GW by November 2025 and roughly 474 GW by June 2026, about 90% of it data centers — yet under 1% of that queue (about 4.3 GW) was actually drawing power by mid-2026 [7]. In PJM, data centers drive roughly 94% of projected load growth through 2030, and the July 2025 capacity auction cleared at the $329.17/MW-day regulatory cap; wholesale energy prices averaged $136.53/MWh in Q1 2026, up 76% year over year, with data centers driving 63% of net load growth [6][16]. Dominion Energy's February 2026 filing counted about 70 GW of large-load requests in Virginia alone [17].

**Equipment.** Transformer lead times have stretched to 128–144 weeks, versus about 50 weeks before 2022 [6]. About half of the 12 GW of US data-center capacity planned for 2026 is delayed or cancelled, and power access is now the top project constraint [6].

**The queue is not a build plan.** Wood Mackenzie estimates that of roughly 1,066 GW of generation capacity data-center developers have requested from US utilities and grid operators, only about 28% is likely to be committed to real projects; the rest reflects speculative site-banking [1]. Global Energy Monitor puts the broader US data-center-linked power pipeline at about 378 GW, with roughly 86% still at the "announced" or "pre-construction" stage [1].

---

## 5. How power is actually being secured

With grid connections measured in years, hyperscalers have moved to contracting power directly, in four overlapping ways:

**Nuclear restarts, uprates, and long PPAs.** Between September 2024 and early 2026, hyperscalers signed nuclear and on-site generation contracts whose combined nameplate capacity already exceeds 30 GW [18]. Notable deals: Microsoft's 20-year PPA for the full 835 MW output of Constellation's Three Mile Island Unit 1 restart (targeting 2027–2028 online); Amazon's September 30, 2026 20-year PPA for 690 MW from Calvert Cliffs in Maryland, including a ~190 MW uprate and more than $3 billion of investment; Google's October 6, 2026 20-year deal for 890 MW of new nuclear capacity plus a 15-year deal for 2,700 MW from existing plants; and Meta's January 2026 20-year PPAs for 2,176 MW from Vistra's Perry and Davis-Besse plants in Ohio, plus 433 MW of uprates phasing in through 2034 [18][19].

**Small modular reactors.** Google's agreement with Kairos Power commits to a 500 MW SMR fleet by 2035, with the 50 MW Hermes 2 unit targeted for 2030; ground was broken in April 2026 [19]. TerraPower's Natrium design is backed by Meta for up to 2.8 GW by 2035 [19]. SMRs remain a 2030s bet, not a 2020s solution.

**Behind-the-meter gas and fuel cells.** This is what is actually delivering power through 2028. Google signed a ~$4 billion, 702 MW fuel-cell plant with AEP and Bloom Energy near Cheyenne, Wyoming, targeting full operation by end of 2028 [19]. Venture Global signed framework agreements for up to 16 combined-cycle power islands of 720 MW each (~11.5 GW) for data-center tenants, with deliveries 2028–2034 [19]. Oracle has leaned hardest into off-grid generation for its gigawatt campuses [19].

**Regulatory friction.** FERC rejected the amended Amazon–Talen Susquehanna behind-the-meter interconnection agreement in November 2024, forcing the industry to restructure co-location deals as grid-connected; in December 2025 FERC directed PJM to overhaul its co-location rules, and in June 2026 FERC issued six show-cause orders forcing grid operators to fix large-load interconnection rules [16][18].

---

## 6. Policy, permitting, and community pushback

**Virginia, the epicenter.** Northern Virginia is the world's largest data-center market, and it is now rewriting its terms. Governor Abigail Spanberger signed Executive Order 22 on September 18, 2026, requiring community approval for new projects over 25 MW, banning state agencies from entering nondisclosure agreements on projects, designating Eastern Virginia a cooling-water-scarcity area, and ordering noise and diesel-emissions reviews [20]. Prince William County then voted 8–0 to strip data centers of by-right development status countywide, requiring special-use permits with public hearings [20]. Loudoun County voted in September 2026 to move toward pausing new data-center and substation approvals for up to 12 months [20]. Bills filed for the January 2027 session include a three-year statewide moratorium (Senate Bill 843, from July 2027 to July 2030) [21]. Virginia has nearly 400 data centers in operation and more than 280 planned [21], and added a $0.011/kWh data-center energy tax in July 2026 [11].

**National scale of opposition.** In the first half of 2026, community opposition blocked, stalled, or indefinitely delayed approximately 120 AI data-center projects across the United States, representing roughly $198 billion in planned investment; the first quarter of 2026 alone saw 75 blocked or delayed projects worth about $130 billion, tracked across 843 distinct opposition groups in 49 states [20]. Water use is a central grievance: evaporative cooling systems can use hundreds of millions of gallons annually, and eastern Virginia groundwater is projected to decline without changes [21].

**Who pays.** The US Senate blocked a bipartisan bill in 2026 that would have required data centers to pay for their own grid upgrades [20]. PJM's capacity auctions have cleared at the price cap, putting roughly $21 billion of incremental capacity cost on PJM ratepayers across three auctions [18]. TVA's data-center rate, effective October 1, 2026, imposes a capacity commitment charge of about $1.5 million per MW on new large loads [6].

---

## 7. Where the buildout goes if not the US

**The Gulf states — the most credible alternative.** Saudi Arabia, the UAE, and Qatar are pairing sovereign wealth with cheap energy (sub-$0.02/kWh solar in the UAE) and US chip-export deals to build AI data centers at gigawatt scale [22][23]:

- **UAE:** the planned 5 GW UAE–US AI Campus in Abu Dhabi hosts Stargate UAE, a 1 GW cluster built by G42 and operated by OpenAI and Oracle with Nvidia, Cisco, and SoftBank; its first 200 MW phase was due in 2026 [22][23]. Microsoft is spending $15.2 billion in the UAE through 2029 and holds a $1.5 billion stake in G42 [23].
- **Saudi Arabia:** the PIF-backed HUMAIN targets 250 MW online by end-2026, 1.7 GW in 2027, and 6 GW by 2034, under the $100 billion Project Transcendence; partners include AWS (a $5 billion AI Zone), xAI (500 MW), and AMD, plus a 1.5 GW DataVolt campus at Oxagon [22][23].
- **Qatar:** the Qatar Investment Authority's Qai formed a $20 billion AI infrastructure joint venture with Brookfield [22].
- The three Gulf states have announced AI investment plans worth $120 billion, exceeding 5% of their GDP, per IMF estimates [22].

The Gulf's model depends on Washington: in November 2025 the US authorized G42 and HUMAIN each to buy up to 35,000 Nvidia GB300 chips, conditional on security and reporting requirements [24]. But the region carries war risk that the US does not: on March 1, 2026, drone strikes hit three AWS data centers in the UAE and Bahrain, and the UAE is reportedly considering dispersing the Stargate site, including underground facilities [23][24].

**Europe — sovereign ambition, slow delivery.** Bruegel puts the EU at about 2 GW of AI compute in 2026 — 5% of the world total — versus 35 GW (78%) in the US and 5 GW (11%) in China [25]. The EU's EuroHPC launched a July 2026 call for AI gigafactories: up to €10 billion in public money plus at least €20 billion private, with selection expected in early 2027 and operations within 18 months after that [25][26]. Bruegel's assessment is blunt: capital is not the main barrier; grid connection speed and permitting are, and even with all planned projects the EU would still run far behind in 2031 [25]. Private initiatives are moving faster than the state program: Schwarz Group (owner of Lidl) is investing €11–13 billion in a German campus expected to hold up to 100,000 AI chips, and Mistral AI raised €3 billion in September 2026 [26].

**Canada and Asia.** Canada and the EU share the same sovereignty logic — reducing dependence on US compute — and Canada's plans, like the Gulf's, are mostly statements of intent so far [24]. Japan and South Korea are relevant mainly as chip and equipment suppliers rather than as gigawatt-scale hosts; the structural constraint is that advanced AI chips remain a US-controlled input everywhere: American export law (including the Foreign Direct Product Rule) reaches foreign-made goods built with US technology, and chip allocations are effectively near zero-sum globally [25][27].

**The honest ranking.** If US buildout stalls, the realistic destinations are: (1) the Gulf, for sovereign-funded gigawatt campuses with cheap power — but gated by US chip-export approvals and regional security risk; (2) Europe, for sovereign and enterprise workloads — but years behind on capacity and permitting; (3) dispersed capacity in power-rich US states (Texas, Ohio, Indiana, Louisiana) rather than abroad at all, since the constraints pushing projects out of Virginia are local, not national.

---

## 8. Outlook: what to watch

1. **Queue conversion.** The 2027 test is whether the 36.3 GW of scheduled additions actually lands, or whether the 50–60% on-time rate persists and the gap between announced and operating capacity keeps widening [2][6].
2. **Power delivery dates.** Nearly every nuclear and gas deal signed in late 2026 delivers most capacity after 2028; the 2027–2028 window will be covered by behind-the-meter gas and fuel cells, not new nuclear [19].
3. **Virginia's January 2027 session.** The moratorium bills (including SB 843) will signal whether the world's largest market stays open for gigawatt builds or becomes a cautionary tale that pushes capital to Texas, Ohio, and the Gulf [21].
4. **Ratepayer politics.** PJM capacity costs, TVA's $1.5M/MW charge, and Virginia's energy tax show the cost question moving from utilities to voters; the next federal move on who pays for grid upgrades matters more than any single project approval [6][18][20].
5. **Gulf execution.** Stargate UAE's first 200 MW and HUMAIN's 250 MW, both due around end-2026, are the first real test of whether sovereign-funded gigawatt AI campuses outside the US can operate at frontier scale [22][23].
6. **Chip allocations.** With global AI chip supply effectively zero-sum, where Nvidia's output is allocated — US hyperscalers vs. Gulf sovereigns vs. European gigafactories — will decide which regions' announcements become operating capacity [25].

---

## Sources

All sources accessed November 5, 2026. Figures are as reported by the cited source; where trackers disagree (e.g., operating capacity of 46–57 GW), the range is given rather than a single point estimate.

1. Goldman Sachs / Wood Mackenzie / Global Energy Monitor figures as reported by The Daily Energy, "US Data Center Power Demand to Keep Growing 38% a Year, Goldman Says — But Most of the Queue Won't Get Built," October 21, 2026. https://thedailyenergy.com/us-data-center-power-demand-goldman-woodmac/
2. Goldman Sachs Research, "What Is the Forecast for US Data Center Power Demand?," Marcus by Goldman Sachs, June 1, 2026. https://www.marcus.com/us/en/resources/heard-at-gs/what-is-the-forecast-for-us-data-center-power-demand-
3. Embers News, "Goldman Sachs Maintains U.S. Data Center Growth Forecast Through 2027," October 9, 2026. https://embers.news/article/goldman-sachs-maintains-us-data-center-growth-forecast-through-2027-400110
4. GPUSmith, "Hyperscaler AI Capex 2026: Amazon, Microsoft, Google, Meta," July 26, 2026 (updated). https://gpusmith.com/articles/en/hyperscaler-ai-capex-2026
5. AIStockWire, "Big Tech's $725B AI capex answers the bubble question," October 2026. https://aistockwire.com/blog/big-tech-725-billion-ai-data-center-capex-bubble-2026
6. Read Achilles, "Power & Grid," October 9, 2026. https://readachilles.com/power-grid/2026-10-09/
7. Gridlas, "Mapping the U.S. Data Center Buildout," figures current as of October 2026 (LBNL, ERCOT, CBRE data). https://gridlas.com/findings.html
8. CTAIO, "Largest AI Data Centers (2026): Stargate, Colossus, Hyperion," October 2026 (Epoch AI Frontier Data Centers dataset, updated October 19, 2026). https://ctaio.dev/en/ai-infrastructure/largest-ai-data-centers/
9. WNT Energy Research, "US Data Center Panorama – 2026 (August)," August 8, 2026 (Bernstein, CleanView, Aterio, Goldman Sachs data). https://research.wntenergy.ca/en/a018/
10. AInvest, "66 GW Is the Number That Matters in U.S. Data Centers Right Now," 2026 (Goldman Sachs, JLL). https://www.ainvest.com/news/66-gw-number-matters-data-centers-2606/
11. Kurums, "US Data Center Investment 2026: Virginia, Texas, Stargate," October 2026 (CBRE, Census Bureau, company earnings). https://kurums.com/united-states-data-center-investment/?v=653f5ac96a69
12. Inflect, "Data Center Power Shortage 2026: Why Grid Capacity Is Now the Bigger Constraint Than GPUs," July 21, 2026 (Gartner, IEA, McKinsey, Uptime Institute). https://inflect.com/blog/data-center-power-shortage-2026-why-grid-capacity-is-now-the-bigger-constraint-than-gpus
13. TensorFeed, "AI Infrastructure: Hyperscaler & Data Center Buildout Tracker," October 2026. https://tensorfeed.ai/ai-infrastructure
14. NewMarketPitch, "Who is building the biggest AI data center?," October 28, 2026. https://newmarketpitch.com/blogs/news/ai-data-center-biggest-campus
15. Ben Carden, "Meta plans to put more than $50 billion into one data center in a Louisiana parish of 20,000 people," LinkedIn, October 15, 2026. https://www.linkedin.com/posts/ben-carden-aa4a92329_meta-plans-to-put-more-than-50-billion-into-activity-7516483292016246784-9_xQ
16. Success Knocks, "Data Center Power Constraints Explained: Why the Grid Can't Keep Up With AI in 2026," 2026 (LBNL, DOE draft 2026 National Transmission Needs Study, FERC). https://successknocks.com/data-center-power-constraints-explained/
17. Apers, "Data Center Investment: PUE, Power & Hyperscaler," October 2026 (JLL, Dominion Energy filing, EIA). https://apers.app/learn/asset-classes/industrial/data-centers-power-pricing-pue-hyperscaler
18. MTS, "Nuclear, SMR & Behind-the-Meter Power Deals for AI Data Centers," updated May 10, 2026 (FERC orders, company filings). https://drops.mts.now/ai-capex/wiki/physical/nuclear-and-power-deals/
19. WeTheFlywheel, "Data Center Power Companies 2026: Who Supplies AI's Gigawatts," October 21, 2026. https://wetheflywheel.com/en/guides/data-center-power-companies-2026/
20. Tech Times, "AI Data Centers Lose Right to Build in Virginia as Senate Stalls Ratepayer Bill," September 28, 2026 (Data Center Watch / 10a Labs). https://www.techtimes.com/articles/328039/20260928/ai-data-centers-lose-right-build-virginia-senate-stalls-ratepayer-bill.htm
21. All Virginia News, "Data center moratorium bills stack up ahead of Virginia legislative session in January," October 2026. https://allvirginia.news/news/data-center-moratorium-bills-stack-up-ahead-of-virginia-legislative-session-in-j
22. IndexBox, "EQT Eyes Gulf AI and Data Centre Deals with UAE and Saudi Sovereign Funds," November 3, 2026. https://www.indexbox.io/blog/eqt-in-talks-with-uae-and-saudi-sovereign-investors-over-ai-and-infrastructure-co-investments/
23. Kurums, "Gulf Data Center Investment: Saudi Arabia, UAE and Qatar," October 2026. https://kurums.com/gulf-data-center-investment-saudi-uae-qatar/?v=653f5ac96a69
24. Guide to Artificial Intelligence, "Why are Saudi Arabia and the UAE building so much AI, and how…," November 2026. https://www.guidetoartificialintelligence.com/en/learn/gulf-ai-buildup-humain-g42/
25. Bruegel, Martens & Schenk, "How can Europe address its pressing artificial intelligence compute infrastructure shortfall?," Policy Brief 18/2026, September 2026. https://www.bruegel.org/sites/default/files/2026-09/PB%2018%202026.pdf
26. Guide to Artificial Intelligence, "What are Europe's AI gigafactories, and will they make Europe…," November 2026. https://www.guidetoartificialintelligence.com/en/learn/europe-ai-gigafactories-explained/
27. Antonio Lopes Correia, "In Medium Heat: The Real Power Behind AI," Medium, October 7, 2026. https://medium.com/@antoniolopescorreia/in-medium-heat-the-real-power-behind-ai-08c2be7f29c5

---

*Prepared by Ace (AceSpade) for taskmarket.dev task TSK-PER7P36C. All figures are as reported by the cited sources as of November 5, 2026; announced project capacities are not operating capacity, and the report distinguishes the two throughout.*
