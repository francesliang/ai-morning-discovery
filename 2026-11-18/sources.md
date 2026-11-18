# Morning Discovery — 2026-11-18

Daily edition. Reporting/attention window: **November 17 07:03 to November 18 07:03 Australia/Melbourne (AEDT, UTC+11)**, equivalent to November 16 20:03–November 17 20:03 UTC. Retrieved November 18 Melbourne. Older underlying work is distinguished from current discussion or verified updates. Popularity metrics are changing snapshots, not audience measurements.

## Archive check and selection

Fetched origin/main and checked fast-forward state before selection. Archive revision: **`2b4d68f9682556878daa3a2ea5351b331b60d37c`**. Read all 16 dated script/source files in eight published editions (November 9–14, 16–17), indexed complete texts locally and searched each selected subject, original URL/domain and paper ID across that archive. No selected discovery was previously explained. Prior omission notes are not counted as coverage. No follow-up recap is required.

[Hacker News front page](https://news.ycombinator.com/) plus a bounded Algolia popular-story query (up to 100 submissions created inside the window), sorted by comments then points. This is not an exhaustive census. Internal snapshot `work/hn-2026-11-18.json` is excluded from publication. Leading discussion signals: Windows telemetry 577 comments/696 points; phone restrictions 497/997; GPT-6.2 392/674; BugMeNot closure 324/704; CMU lectures 297/2,212; Optimizely 253/640. Chosen stories retain both AI and consequential non-AI subjects. BugMeNot and national-security outages lacked sufficient verified explanatory detail for inclusion; no common cause between unrelated outages is inferred.

Skipped unchanged archive subjects: NVIDIA investigation/leadership and financing arguments (November 9–13); Microsoft 365, United agent restrictions, Apiiro configuration exposure and local smart-home control (November 14); Starship catch, FAA preliminary details and generated-code reciprocity (November 16); Qwen4-Max, Amazon sale pricing, uBlock disclosure, Gamer and VibePrevisBench (November 17). Higher votes or another discussion alone do not qualify a repeat. [Published archive](https://github.com/francesliang/ai-morning-discovery/tree/main).

## 1. Windows developer-tool telemetry investigation

- Original researcher: [Xusheng Li investigation](https://xusheng.dev/posts/windows-coding-agent-telemetry/), dated November 16. Direct public HTML retrieval succeeded after the web research service failed. Author's described tests, event payload and upload queue were read; no local Windows experiment or packet-capture replication performed here.
- [HN discussion](https://news.ycombinator.com/item?id=50524736), created November 16 22:58:20 UTC; 577 comments/696 points in ranking snapshot (opened at 573 comments). Actual disagreement over Linux migration, application compatibility and anti-cheat requirements inspected. These comments are not independent validation of the telemetry analysis.
- Distinguish event collection, saved bitmap, queued upload and actual delivery. The dialogue reports the demonstrated queue; it does not claim independent proof of Microsoft's receipt. Default-setting and rollout evidence applies to the author's tested United States installation and ARM VM, not every region/build. No prompt or source-code exfiltration claim is made. No settings changed on the user's computer.

## 2. New school phone-restriction findings

- Discovery: [NYT article](https://www.nytimes.com/2026/11/17/upshot/school-phone-bans-study-scores.html), November 17, inaccessible to the web tool. Claims verified against [Harvard CEPR primary announcement](https://cepr.harvard.edu/cell-phone-press-release), November 17; not against an archived paywall bypass.
- [HN discussion](https://news.ycombinator.com/item?id=50530163), created November 17 11:45:51 UTC; 497 comments/997 points (opened earlier at 495/982). Read actual parent social-experience account and communication/implementation objections. Anecdotes remain labelled.
- Earlier comparison, not fresh news: [Stanford primary account](https://news.stanford.edu/stories/2026/11/school-phone-bans-research), November 2. Used briefly to retain uncertainty; different studies must not be collapsed into one verdict. No AP article or search-only Reddit result used as factual evidence.
- Findings are author estimates; a learning-week equivalence is an interpretation of an effect size, not literal additional school days. Strict lockable-pouch policy and statewide estimates are distinguished; the latter have explicit pre-existing-trend concerns. No claim that the new study explains all achievement changes or all phone-policy effects. No independent reanalysis performed.

## 3. GPT-6.2 Astra and Sol

- Original publisher release: [OpenAI announcement](https://openai.com/index/introducing-gpt-6-2-astra-sol/), November 17. GDPval v2 comparison is publisher-reported and not reproduced.
- Used **OpenAI Docs** guidance for source verification: official-domain search followed by actual fetched model documentation: [Astra](https://developers.openai.com/api/docs/models/gpt-6.2-astra), [Sol](https://developers.openai.com/api/docs/models/gpt-6.2-sol). Markdown versions were fetched to inspect the actual pricing and context qualifications. No API calls, model tests or configuration changes performed.
- [HN discussion](https://news.ycombinator.com/item?id=50535230), created November 17 17:46:43 UTC; 392 comments/674 points (opened earlier at 387/672). Actual overengineering/abstraction concern read; no release-day consensus or solved-behaviour claim inferred.
- Pricing in dialogue is standard short-context uncached input/output per million tokens; long-context and tier modifiers are retained. No cached-input price is passed off as a general rate, and base rates are not a complete workflow-cost estimate. Token efficiency, unit price and accepted-task cost remain distinct. News reporting does not change the Gemini model/project used for podcast production.

## 4. Carnegie Mellon CS Learn

- Primary: [CS Learn](https://www.cs.cmu.edu/learn/), current November premiere schedule. Lecture access and forthcoming courseware are explicitly separated; January courses and future premieres are not described as already fully available. No exact original webpage publication timestamp displayed.
- [HN discussion](https://news.ycombinator.com/item?id=50522980), created November 16 20:43:36 UTC; 297 comments/2,212 points (opened at 294/2,192). Organiser Phillip Compeau's first-person launch-day explanation, student production tooling and human lecture review were read. Other participants discuss what a university provides beyond recorded curriculum. These are attributed discussion views.
- Host suggestions about problems and projects are analysis, not promises of assessment, accreditation, certificates, admission or personal feedback. No course enrolment or message submission performed.

## 5. Optimizely web experimentation incident

- Original investigation: [Scott Helme / Report URI](https://blog.report-uri.com/worlds-largest-brands-infected-with-malware-via-optimizely/), November 16, with a **November 17 09:17 UTC** update. Researcher findings and limited visibility remain attributed. Report URI sells related monitoring services; its analysis is not an independent vendor certification. No malicious URLs, payloads or demonstrations executed.
- Vendor confirmation: [Optimizely incident page](https://status.optimizely.com/incidents/ftw0fh9wx43z), **November 17 01:02 UTC**, marked Monitoring at retrieval. The vendor's fix/removal/account-security statement is distinct from a complete harm assessment or final incident report.
- [HN discussion](https://news.ycombinator.com/item?id=50524767), created November 16 23:00:34 UTC; 253 comments/640 points. Read third-party-code-authority concerns and server-side/edge alternatives. No claim that an alternative automatically removes every risk.
- The organisation count is research-reported exposure, not a count of infected visitors or compromised first-party infrastructures. Cleanup does not establish the number of stolen records or infected devices. This story is different from the previously covered uBlock disclosure; no unverified connection is asserted.

## 6. K2-Horizon technical report

- Original: [arXiv 2611.21003](https://arxiv.org/abs/2611.21003), first submitted November 16.
- [HF paper and community](https://huggingface.co/papers/2611.21003), submitted November 17; daily rank 2, 67 votes when opened (initial listing 66). Community content inspected is an author/submitter explanation, not independent replication. Questions in dialogue are host analysis.
- Primary [project and linked resources](https://ifm.ai/k2/). The project's timeline references September 2026; this episode reports a newly submitted technical paper and fresh attention, not a claim that the entire model family launched for the first time today. Links to code/data/checkpoints were visible; all artifacts were not downloaded or comprehensively audited.
- Architecture comparisons are author-reported, with the shared-training-data condition retained. Active parameters and total parameters are distinguished. Stated release openness does not certify completeness, legal compliance or cheap reproducibility. No benchmark or training run performed.

## Enabled-source audit and omissions

- [HF daily](https://huggingface.co/papers), November 17: Sage S2.1 Flash 83–84 votes; K2-Horizon 66–67; AllocFlow 66; InclusionMed 62; SPILLWAY 48; SWE-CoWork 44; ScaleVLA 41. Sage's title says S2.1 while its abstract repeatedly says S1.5, on both [HF](https://huggingface.co/papers/2611.21072) and [arXiv](https://arxiv.org/abs/2611.21072). The version inconsistency was not resolved, so specific new-model claims were omitted. Allocation/health papers were not promoted into trading or clinical guidance from ranking alone.
- [HF weekly W47](https://huggingface.co/papers/week/2026-W47), labelled November 15–21: web service failed, direct public HTML succeeded. Snapshot: robotics roadmap 124, Gamer 117, VibePrevisBench 88, Sage 84, K2 67, AllocFlow 66, InclusionMed 62, MIRIX 52. This is a partial-week board. Prior explained Gamer/VibePrevis discoveries are skipped; themes include embodied agents, memory, efficiency and evaluable work. Daily/weekly overlap is covered once.
- [Reddit Popular](https://www.reddit.com/r/popular/) again returned a stale listing, marked three days old, with coffee-change, Titanic, airport and entertainment posts and no usable fresh votes/timestamps. No current ranking or factual claim inferred; no substitute subreddit used. Unsolicited Reddit results from general research search were not used as configured-feed discoveries.
- [Last Week in AI podcast](https://lastweekin.ai/s/podcast) returned a subscription page; direct [RSS](https://lastweekin.ai/feed) returned HTTP 403. No current-window audio verified; no older episode presented as fresh.
- Important-beyond-rankings review included vendor incident confirmation and primary research qualifications. Apple/NSA outage headlines were not linked by conjecture. Source gaps, version checks and selection audits remain outside spoken dialogue.

## Text checks

Six substantive topics, four-turn recurring intro, exact daily window, speaker-labelled paragraphs, no spoken URLs, and a brief recap. Maya/Speaker1 uses Callirrhoe; Jax/Speaker2 uses Puck. No invented personal experiences or forced disagreement. Existing bundled Gemini TTS, project/model configuration and intro track retained. The drafting count excludes speaker labels; measured audio determines the 900-second limit.

## Production resumed November 19

The November 18 attempt was blocked by Gemini HTTP 403 PERMISSION_DENIED, reporting an outstanding billing-account balance. The same existing key and configured model accepted generation on November 19. Resumed this already-authorized edition using its unchanged script and original reporting window. No payment, key change, project switch or model switch was performed by the agent. Both this edition and November 19 are being validated for publication together.

## Audio and publication checks

Completed the validated speech sections using the existing Gemini model/project configuration. Intro music mixed with the configured five-second lead-in and fade. Final AAC/M4A is 4,940,700 bytes, measured at 598.414792 seconds (00:09:58); below the 900-second maximum. Whole-file PCM decode succeeded; seven three-second samples spanning intro, early dialogue, middle and ending were inspected for signal and clipping. No full listening or speech-transcription review performed; speaker configuration was checked, but audible voice/content fidelity was not independently established.

Feed parsed successfully; new episode appears once with unique date GUID, audio/mp4 MIME type and actual enclosure size/duration. Historical items and channel metadata preserved. Only script.md, sources.md, podcast.m4a and root feed.xml are intended for staging; source music, credentials and caches are excluded.
