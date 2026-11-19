# ConsultUsNow – Meta Ads Creative Test (50 Hooks × 3 Bodies × 3 CTAs)

Files in this folder:
- `hooks_rated.csv` – all 50 hooks with theme, score (out of 10), tier, Phase 1 yes/park
- `all_450_combinations.csv` – every combination with its final ad name, phase and status column (use as the tracker)

## 1. Why we don't launch all 450 at once
- Meta allows max 50 ads per ad set and will push spend to 3–5 ads anyway; the other ~440 get almost no delivery, so we learn nothing about them.
- To judge one ad on lead quality we need ~10–15 WhatsApp conversations. 450 ads × 10 × ~₹150 per conversation = ₹6.75 lakh just for testing.
- Hook, body and CTA do different jobs, so test them one layer at a time:
  - Hook → stops the scroll (3-sec hook rate)
  - Body → keeps them watching and builds trust (hold rate, CTR)
  - CTA → decides who messages (cost per conversation, qualified %)

Result: ~86 ads in 3 phases instead of 450, and every winner is a proven combination.

## 2. Ratings

### Bodies
| Body | Score | Strength | Fix |
|---|---|---|---|
| B1 – Leads → CRM → optimise | 7/10 | Simple, clear flow | No proof, no numbers. Add "90,000+ leads, 50+ brands" line. Cut "CRM-la track panradhu mattum podhuma?" repetition. |
| B2 – Beyond low CPL | 7.5/10 | Best logic (Creative → Destination → Follow-up). Perfect for CPL/quality hooks | Too long, jargon ("friction", "Lead Destination"). Say "WhatsApp / Form / Website" instead. Add proof line. |
| B3 – 7 yrs, 90,000+ leads, end-to-end | 8.5/10 | Authority + unique differentiator (shoot team comes to your location) | Longest. Fix "Nan … pannirukkom" → "Naanga … pannirukkom". REMOVE "keezha irukkura link-ah click panni contact pannunga" – it fights the WhatsApp CTA. Add a bridge line from the hook problem. |

### CTAs
| CTA | Score | Effect |
|---|---|---|
| C1 – "Innum neraya therinjukka WhatsApp pannunga" | 7/10 | Most messages, lowest quality (curiosity seekers) |
| C2 – "Selected brands kooda dhaan work pannrom… qualify aagudhanu therinjukka WhatsApp pannunga" | 8.5/10 | Exclusivity + filter. Best quality/volume balance. **Default CTA for Phase 1–2** |
| C3 – "Serious-ah irukkeenganna mattum WhatsApp pannunga" | 8/10 | Strong filter, lower volume. "Next level" is cliché → "Unga business-ah adutha level-ku…" or add a hard filter: "Maasam ₹30,000+ ad budget irukkura businesses mattum". |

### Hooks (full list in `hooks_rated.csv`)
- **Tier A (8+):** H01, H02, H05, H09, H50, H04, H08, H17, H18, H20, H23, H47, H48
- **Tier B (6.5–7.5):** H03, H06, H07, H10, H11, H12, H16, H21, H24, H25, H26, H42, H45, H49, H19, H22, H35, H37, H43, H44
- **Park / rewrite (<5.5):** H14, H15, H29, H30, H31, H34, H36, H38, H41

Why park those 9: the bodies talk about **lead quality, CRM and sales conversion**. Hooks about "no leads at all" or technical media-buying doubts (duplicate ad, broad vs interest, notifications) promise an answer the body never gives. They also attract DIY marketers and freelancers, not business owners. If you want them, rewrite to bridge to the body, e.g.:
- H14 → "Daily ₹1,000 spend pannreenga… aana adhula evlo sales-nu theriyalaya?"
- H38 → "Broad-ah, interest-ah nu yosikkuradhu dhaan problem-nu nenaikkureengala? Unmaiyana problem vera."

Duplicates to watch (similar message – pick the winner, drop the other): H05/H47/H50 (spend vs sales), H08/H17/H23 (no conversion), H03/H11 (CPL), H12/H21/H22 (junk leads).

Small text fixes: "solrangala" → "solraangala"; H01 "Kuzhandhai theriyama click pannittaanga" should be shown as on-screen text in a customer voice; keep every hook under 4 seconds spoken.

## 3. Production
| Asset | Count | Notes |
|---|---|---|
| Hooks | 41 (+9 if rewritten) | Shoot separately, 2–4 sec each, 2 takes each. Same outfit/background as body so stitching is seamless. On-screen text = hook text. |
| Bodies | 3 | Shoot as separate clips. Body 3 without its old CTA line. |
| CTAs | 3 | Separate 4–6 sec clips. Same frame as body end. |

Editing: build one template (captions, logo, end card) and swap clips. Export 9:16 (Reels/Stories) and 4:5 (Feed). Phase 1 = 41 edits only.

## 4. Test structure (Click-to-WhatsApp, CRM sends Converted event to Meta)

| Phase | What | Ads | Fixed | Decide on |
|---|---|---|---|---|
| P1 Hook test | 41 hooks | 41 | B3 + C2 | Hook rate (3s views ÷ impressions) ≥ 30%, cost per conversation, CRM qualified % |
| P2 Body test | Top 10 hooks × 3 bodies | 30 | C2 | Hold rate (ThruPlay ÷ 3s views), cost per **qualified** lead |
| P3 CTA test | Top 5 hook+body × 3 CTAs | 15 | – | Cost per qualified lead, qualified %, converted |
| Scale | Top 3–5 combos | – | – | Cost per conversion (CRM CONVERTED) |

Ad set setup for tests: ABO (budget per ad set), 5–6 ads per ad set so each ad gets spend, same audience in all ad sets (Tamil Nadu, 25–55, business owners / broad), placements Reels + Feed. Don't edit ads during a phase – it resets learning.

Kill rules (after ~₹500 spend on an ad): hook rate < 20% → off. No conversation after 2× target cost → off.

## 5. Naming convention (must match the CSV)

```
Campaign : CUN_CTWA_<Phase>-<Purpose>_<MonYY>        e.g. CUN_CTWA_P1-HookTest_Dec26
Ad set   : <Phase>_AS<nn>_<Audience>_<Hooks>          e.g. P1_AS01_TN-Broad-25-55_H01-H06
Ad       : H<nn>-<THEME>_B<n>_C<n>_v<n>               e.g. H01-QUAL_B3_C2_v1
```
Themes: QUAL (lead quality), SALES (sales team), ROI (spend vs revenue tracking), CONV (no conversion), CPL, DIAG, TECH, NOLEAD, CREA.

Rules: underscores only between fields, no spaces, never rename a live ad (make v2 instead). Analysis can then group by hook, theme, body or CTA by splitting the ad name.

## 6. CRM tracking
Current baseline (ConsultUsNow, all time, CRM): 388 leads → 54 Qualified + 15 Converted (~18% qualified, ~4% converted), 182 Closed, 130 still NEW.

Must-do before launch:
1. CRM must store the **ad ID / ad name** for each Click-to-WhatsApp lead (from the WhatsApp referral `source_id`). Today the CRM only marks `from_ad = true` – without the ad name we cannot tell which combo produced which lead.
2. Sales team updates status within 24 hrs: NEW → QUALIFIED / NOT_QUALIFIED → CONVERTED / CLOSED. Clear the 130 NEW backlog first so data is clean.
3. Weekly sheet: Ad name | Spend | Conversations | Qualified | Converted | Cost per qualified | Cost per conversion.

## 7. Timeline (deadline: 2 Jan 2027)
| Dates | Task | Owner |
|---|---|---|
| 19–22 Nov | Finalise script edits, ratings sign-off, CRM ad-name capture | Strategy + CRM |
| 24–26 Nov | Shoot hooks, bodies, CTAs | Shoot team |
| 27 Nov–1 Dec | Edit 41 Phase 1 ads, name per convention, upload | Editor + Ads |
| 2–8 Dec | **P1 Hook test** live | Ads |
| 9 Dec | P1 review → top 10 hooks | Strategy |
| 10–16 Dec | **P2 Body test** (30 ads) | Ads |
| 17 Dec | P2 review → top 5 hook+body | Strategy |
| 18–24 Dec | **P3 CTA test** (15 ads) | Ads |
| 25–31 Dec | Scale winners, wait for CRM conversions to mature | Ads + Sales |
| 2 Jan | Final report: winning combos, cost per qualified, cost per conversion | Strategy |
