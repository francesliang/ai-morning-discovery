Speaker1: Good morning, and welcome to Morning Discovery for Wednesday, November eighteenth, twenty twenty-six. I'm Maya.

Speaker2: And I'm Jax. Today, we're checking what computers report about us, what classrooms gain without phones, and what a new generation of models actually promises.

Speaker1: This is our daily edition, covering seven oh-three a.m. on November seventeenth to seven oh-three a.m. on November eighteenth, Melbourne time, Australian Eastern Daylight Time.

Speaker2: On the menu: Windows telemetry, new school research, OpenAI's latest release, and free computer-science lectures. Let's begin.

Speaker1: Our most-discussed discovery is Xusheng Li's investigation of a Windows eleven diagnostic component. It attracted roughly five hundred and eighty comments. He reports finding checks for coding agents and development tools, followed by stored indicators of which categories had been observed.

Speaker2: This goes beyond finding product names in a binary. In his test, he renamed a copy of the command shell to match an agent's executable name. The corresponding indicator appeared in saved state and a diagnostic report. A separate compiler-name test also triggered the broader development-tool category.

Speaker1: The report describes a bitmap: flags for observed tool categories, rather than a transcript of what someone did. Li says he found no prompt text or source code in this report. He says this component discarded the incoming events' detailed usage measurements.

Speaker2: The transmission claim needs care. He found the event queued for upload when optional diagnostics were allowed. That's stronger evidence than a local event alone, but it isn't an independent confirmation of Microsoft's receipt. His default-setting test used a clean United States setup, and his running-component test used a particular Windows ARM virtual machine. We shouldn't generalise those defaults to every installation.

Speaker1: In the discussion, some participants recommend moving to Linux. Others push back that games, anti-cheat systems and required applications can make switching difficult. Those are practical disagreements about alternatives, not independent verification of the reverse engineering.

Speaker2: The takeaway is to distinguish the collection, the payload and the upload condition. Tool-usage flags can still reveal something meaningful about a person, even when they contain neither their code nor their conversations.

Speaker1: Next, a November seventeenth Harvard-led study examines strict school phone restrictions. Its researchers follow three point three million students across forty-six hundred schools, using mathematics and reading growth before and after policies requiring phones to be stored in lockable pouches.

Speaker2: The authors estimate an annual improvement of about one-hundredth of a standard deviation, which they translate into roughly one or two additional weeks of learning. That's a modest gain, not a sudden transformation of a school.

Speaker1: The particular policy matters. Storing phones for the school day isn't identical to asking students to keep them out of sight during lessons. The researchers separately examine statewide restrictions, but caution that those estimates could reflect trends already present in the states adopting them.

Speaker2: And the research picture isn't unanimous. A separate Stanford-led study, described earlier this month, found lower phone use but little overall change in test scores or attendance. The new result adds evidence; it doesn't make every earlier finding disappear or prove that phones explain every learning problem.

Speaker1: The nearly five-hundred-comment discussion includes a parent's account of children enjoying more face-to-face social time after a ban. Others discuss why parents want a reliable way to reach their children. Those experiences help explain the trade-offs, but they aren't substitutes for the study's comparison.

Speaker2: My takeaway is to keep the policy, outcome and effect size together. Small improvements can matter when sustained, while a headline about banning phones leaves many implementation choices unanswered.

Speaker1: OpenAI also announced GPT six point two Astra and Sol on November seventeenth. It positions Astra for its hardest professional projects and Sol for everyday work. The release emphasises better deliverables and fewer output tokens, alongside coding and computer-use improvements.

Speaker2: There's a useful concrete comparison in the announcement. On OpenAI's internal GDPval version two evaluation, Astra improves six point two percentage points over the previous Astra while using twenty-two percent fewer output tokens. That's a publisher-reported benchmark result, not a promise about every task, and the comparison uses a particular evaluation setup.

Speaker1: Official API documentation lists standard short-context rates of eight dollars per million input tokens and forty dollars per million output tokens for Astra. Sol's corresponding rates are two dollars and ten dollars. Requests above two hundred and seventy-two thousand input tokens have higher rates, and processing tiers change prices too. Those base numbers aren't a complete bill.

Speaker2: Which is why token efficiency and token price need separate attention. A lower rate, fewer tokens and fewer rounds of revision can affect cost in different ways. None of those alone tells us the cost of an accepted result.

Speaker1: In the roughly four-hundred-comment discussion, a prominent concern is overengineering: whether the model chooses an appropriate amount of structure instead of adding unnecessary abstractions. That's a question about behaviour on real projects, not something a release-day comment establishes has been solved.

Speaker2: The takeaway is to look beyond whether it can finish the task. Can it finish with a sensible amount of code, a usable deliverable and a clear account of any obstacles? A new benchmark score is a starting point for that test.

Speaker1: A different kind of access story comes from Carnegie Mellon. Its CS Learn site offers free lecture recordings on YouTube, with free courseware described as coming next. The initiative gained almost three hundred comments and more than twenty-two hundred points in our snapshot.

Speaker2: The initial selection includes Principles of Computing and Machine Learning with Large Datasets. The published schedule adds software construction and machine-learning systems, then architecture, quality management and agent courses during the week. More subjects are scheduled for January. A schedule isn't a claim that every course is already fully available.

Speaker1: In the original discussion, programme organiser Phillip Compeau says the project releases full semesters of current courses. He describes student-built tools helping automate production, with people reviewing every lecture. That's his description of how a small team makes the work manageable.

Speaker2: Commenters discuss what free recordings provide and what remains distinctive about a university: assessment, feedback, collaboration and an organised course of study. Watching a lecture gives access to an explanation; it doesn't automatically supply those other parts.

Speaker1: The practical takeaway is to connect the lectures to work you can check. Solving problems and building something gives the material a place to stick. The university says the courseware will follow, so distinguish that promise from the videos available now.

Speaker2: Your browser may now contain an entire computer-science semester. Unfortunately, the tabs still won't do the assignments for you.

Speaker1: Turning to security, Report URI describes malicious JavaScript reaching visitors through Optimizely's web experimentation platform on November sixteenth. The important new confirmation is Optimizely's November seventeenth statement that an unauthorised party exploited a vulnerability and added code to customer projects.

Speaker2: The vendor says it fixed the vulnerability, removed the injected code and took steps to secure affected accounts. Its incident page remains in monitoring in the update we checked. That is the vendor's remediation statement, not a complete accounting of harm.

Speaker1: Report URI's investigation says the attacker modified a customer-project JavaScript field inside snippets served from a trusted domain. It reports exposure across one hundred and seventy-eight organisations, including Zoom and GitLab. That count is the researcher's finding; it doesn't mean every visitor was infected or that each organisation's own infrastructure was breached.

Speaker2: In a November seventeenth update, the researchers say their monitored infected files had all been cleaned. They also say they cannot determine the full extent of stolen card data, cookies or device infections. Cleaning the delivery path and measuring the consequences are different jobs.

Speaker1: The discussion debates the security cost of allowing third-party tools to change pages, and notes that some experimentation can happen on the server instead. Our takeaway is that approving a script's delivery address doesn't guarantee its contents stay trustworthy. The authority granted to a dependency matters as much as where it is hosted.

Speaker2: Finally, K Two Horizon's technical report gained fresh research attention on November seventeenth, a day after its original paper submission. It ranks second on the daily paper page with sixty-seven upvotes. The work describes six language models, from under a billion parameters to a much larger mixture-of-experts model.

Speaker1: One contribution is a controlled architecture comparison. The authors' thirty-six-billion-parameter model activates roughly four billion parameters, combining changes to attention with sparse computation. They report that it nearly matches a thirty-two-billion-parameter dense model trained on the same data, with about one-seventh the active parameters. That's their experimental result, not a universal equivalence between those model sizes.

Speaker2: The other contribution is what the authors propose to make inspectable: training code, intermediate checkpoints, data and development records. The project links to training resources as well as final models. We haven't audited every artifact or reproduced the training, so openness here describes the release's stated materials, not our certification of completeness.

Speaker1: The question raised by that approach is what other researchers can isolate and test. If several models share a recipe and corpus, a comparison can reveal more about an architectural choice than comparing unrelated finished systems. Access also doesn't remove the compute needed to repeat a large training run.

Speaker2: My takeaway is that a model release can offer both a tool and an experiment others can examine. Those are different kinds of value, and the development record helps with the second.

Speaker1: Today's recap: check what telemetry actually contains, keep school-policy effects in proportion, and evaluate new models through usable results. Free lectures widen access, while the security incident and open-model report remind us to inspect the systems and materials behind an output.

Speaker2: I'm Jax. Thanks for listening, and good luck with those newly acquired lecture tabs.

Speaker1: I'm Maya. This has been Morning Discovery. Have a good Wednesday.
