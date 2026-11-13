# Morning Discovery — 2026-11-14

Weekend edition. Seven-day reporting window: 2026-11-07 07:04 through 2026-11-14 07:04 Australia/Melbourne (AEDT, UTC+11), equivalent to November 6 20:04 through November 13 20:04 UTC. Trigger: November 14 07:04:27 AEDT; endpoint rounded down to the minute. Retrieved November 14 AEDT. Rankings are snapshots and do not establish historical peaks. Earlier original publications qualify through new discussion/developments in the week, as noted below.

## Whole-week discovery and archive audit

Fetched default branch main; archive revision `e49a7ce7abf3c55dc7e35518ebc29bd1029dd268`. Read and indexed all archived dated scripts and sources (November 9–13), including subjects, URLs and paper IDs. Searched whole archive for selected URLs, discussion IDs and paper IDs. No selected discovery was previously explained. Smart-home essay and Microsoft outage had appeared in prior selection notes as omitted/unverified candidates, not substantive narrated coverage. No follow-up to a previously explained discovery is claimed.

Reviewed the entire seven-day interval using current HN plus Algolia story discovery restricted to start/end timestamps, retrieving 100 popular story results and ranking that retrieved set by comment count. This is a broad popular-story sample, not an exhaustive census of every submission. Original query: https://hn.algolia.com/api/v1/search?tags=story&numericFilters=created_at_i%3E1793995440%2Ccreated_at_i%3C1794600240&hitsPerPage=100 . Query timestamps are recorded in the local retrieval JSON; the readable window above is authoritative.

Most-discussed sampled subjects included Huang resignation 3,388 comments, preparing-to-oust report 1,642, Huang letter 1,293, Fable/Mythos 1,054, AI-bubble opinion 974, Microsoft service degradation 960, IPO 899, United agents 698, employee petition 627, fragile-code essay 625, Starlink Mini 2 618, men's health report 611. Comments prioritised, points secondary; primary verification and prior coverage then determine selection. Selected topics synthesise operational dependencies, delegation and reliability rather than seven daily recaps.

Skipped unchanged repeats: NVIDIA investigation/transition, Fable/Mythos, Anthropic IPO, fragile-code discussion, Tim Peters, archaeology correction, AWS Emulator, carbon budget, and previously explained research papers including LingBot-Touch, Confucius, SplatAnything, P²-MOPD, WorldFoundry, World ICL, Tree-Ising, TOME-Math and SteerDistill. New employee-petition reporting was not promoted without primary confirmation. Higher votes/new discussion URLs are not treated as new discoveries. Prior archive: https://github.com/francesliang/ai-morning-discovery/tree/main . No same-date rerun existed.

## Microsoft 365 service disruption

- Primary live incident page: https://status.cloud.microsoft/m365/
- Web parser only returned JavaScript shell; inspected rendered browser page and expanded official details.
- Official notice last updated November 13 20:02:18 UTC, inside window, still showed service degradation, queued-message draining, traffic rebalancing and no ETA for full recovery. Exchange-dependent features distinguished from working functions. No final cause or universal outage asserted.
- Discussion inspected: https://news.ycombinator.com/item?id=50471731
- Weekly API snapshot: 1,140 points, 960 comments; thread: 1,139 points, 957 comments.
- Supporting reporting checked, not used to replace official current status: https://apnews.com/article/d92547a821930290db2964388016979a and https://apnews.com/article/6376045281feb430c0b923e3a4b251c2 . Prior-edition selection notes had insufficient verification; today's rendered official page supplies it. No claim all services recovered or that all suite functions failed.

## United's unauthorised personal-agent restrictions

- Primary November 11 statement: https://united.mediaroom.com/news-releases?item=125496
- Original linked reporting inspected: https://www.cbsnews.com/news/united-airlines-bans-ai-agents-booking-flights/
- Discussion inspected: https://news.ycombinator.com/item?id=50458900
- Weekly API: 677 points, 698 comments; thread: 676 points, 698 comments. Submitted November 11.
- Airline rationale distinguished from legal findings or universal bans on automation. No airline regulation independently interpreted. Approved delegation examples in script are hosts' analysis, not announced United features. No evasion methods included.

## Coding-agent settings and secret exposure

- Primary researcher report published November 5, with November 8 response update inside week: https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again
- Discussion: https://news.ycombinator.com/item?id=50407882
- Regular page returned HTTP 429; read the thread via official Algolia HN item mirror https://hn.algolia.com/api/v1/items/50407882 , including bcherny comments 50408126, 50408176 and 50408250. Response and discussion occurred November 7–8, within window.
- Weekly snapshot: 626 points, 431 comments.
- Research survey not independently reproduced. Distinguish storing a command from committing/exposing a file. Product-team proposals are not a shipped remediation. No actual exposed secrets retrieved, displayed or reused. Security guidance stays limited to the report's credential-rotation/history distinction.

## Household local control

- October essay, with major discussion November 10: https://docodethatmatters.com/home-automation-overnight-success/
- Inspected discussion: https://news.ycombinator.com/item?id=50441707 . Weekly sample 1,194 points, 442 comments. Earlier archive only recorded it as omitted; not previously narrated.
- Separate November 11 author project: https://scottjg.com/posts/2026-11-11-reverse-engineering-my-coway-air-purifier-to-ditch-the-cloud/
- Discussion inspected: https://news.ycombinator.com/item?id=50474959 . Current front page 559 points, 157 comments; detail 570 points, 159 comments. First-person result not independently reproduced; firmware/model compatibility not established broadly.
- Both primary accounts inspected. Synthesis about service boundaries is hosts' analysis. No electrical work, device modification, network-security changes or bypass procedure performed or recommended to the user.

## Few-Step Streaming Video Generation / APEX

- Original: https://arxiv.org/abs/2611.14033
- Discovery and author community explanation: https://huggingface.co/papers/2611.14033
- Published November 10; submitted November 11. Current weekly #3, 88 upvotes. Higher-ranked entries already covered; this discovery has no prior explanation in archive.
- Author abstract and post inspected. Higher instruction following/aesthetics reported alongside worse motion quality, mostly tied audio sync and unchanged usability. Efficiency comparison and output-quality comparison have different baselines; not merged into a universal performance claim. No reproduction, no invented independent debate.

## SO-Arena

- Original: https://arxiv.org/abs/2611.15777
- Discovery and inspected author/reader discussion: https://huggingface.co/papers/2611.15777
- Published November 11; submitted November 13. Daily #1, 72 votes; weekly #4, 72.
- Reported accuracy/reliability ranking distinction applies to benchmark's 21 models, 11 domains and five capability families. Reader's domain-gap question attributed as a question. No independent benchmark run performed; no broad consensus or universal unreliability asserted.

## Other enabled feeds and coverage limits

- HN starting page https://news.ycombinator.com/ plus date-restricted weekly discovery above. Important beyond-ranking verification included current official incident details and the airline's direct statement.
- Daily https://huggingface.co/papers and weekly https://huggingface.co/papers/week/2026-W46 both inspected. Weekly page labels November 8–14; full window additionally includes November 7 via archive and week discovery. Weekly leaders: tactile representation 102, Confucius 93, streaming condition shifting 88, SO-Arena 72; themes include efficient generation, fast-decision reliability and embodied systems. Covered selected new work once, excluding archived repeats.
- Sole Reddit discovery input https://www.reddit.com/r/popular/ returned cached content marked four days old, without adequate current metrics. Direct https://www.reddit.com/r/popular/.json?limit=15 returned HTTP 403. No substitute subreddit discovery used; incidental search results were not used as a replacement ranking.
- Podcast starting page https://lastweekin.ai/s/podcast returned subscription content. Direct https://lastweekin.ai/feed checked. Newsletter recap #347 appeared November 11 14:21:42 GMT, inside weekend window, but image enclosure and its text identify a newsletter rather than new audio. Most of its highlighted subjects already covered; no unverified financial/intelligence claims added. Latest audio-enclosure item returned remains October 3. No older episode portrayed as fresh.
- Starlink candidate https://starlink.com/mini-2 and discussion https://news.ycombinator.com/item?id=50444129 inspected; primary page yielded JavaScript-only content, and travel-plan anecdotes were not independently corroborated. Omitted rather than inventing hardware specs or current plan rules. Other high-ranked opinion/health articles not selected without adequate verification or room for substantive treatment.

## Production

Maya/Speaker1 uses Callirrhoe, Jax/Speaker2 uses Puck. Weekend dialogue preserves exact seven-day window and avoids daily chronology/repeated explanations. Source-selection and coverage notes remain here, outside speech. Intro music uses existing checkout-root track with five-second lead-in and fade by nine seconds. Existing Gemini model/project reused; key parsed only as data into child-process environment. No keys, caches, source music or temporary audio intended for staging. Final measured duration must not exceed 900 seconds.

Draft: 1554 spoken words excluding labels, 39 labelled turns.

## Audio and publication checks

Completed five sections using the existing Gemini model/project configuration. Intro music mixed with the configured five-second lead-in and fade. Final AAC/M4A is 4,761,974 bytes, measured at 577.094792 seconds (00:09:37); below the 900-second maximum. Whole-file PCM decode succeeded; seven three-second samples spanning intro, early dialogue, middle and ending were inspected for signal and clipping. No full listening or speech-transcription review performed; speaker configuration was checked, but audible voice/content fidelity was not independently established.

Feed parsed successfully; new episode appears once with unique date GUID, audio/mp4 MIME type and actual enclosure size/duration. Historical items and channel metadata preserved. Only script.md, sources.md, podcast.m4a and root feed.xml are intended for staging; source music, credentials and caches are excluded.
