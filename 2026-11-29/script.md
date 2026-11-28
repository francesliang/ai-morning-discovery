Speaker1: Good morning, and welcome to Morning Discovery for Sunday, November twenty-ninth, twenty twenty-six. I'm Maya.

Speaker2: And I'm Jax. Big ideas, useful context, and a closer look at what changes when a resource, a service or an experiment moves into a new phase.

Speaker1: This is our weekend edition, covering six fifty-six a.m. on November twenty-second to six fifty-six a.m. on November twenty-ninth, Melbourne time, Australian Eastern Daylight Time.

Speaker2: On the menu: a withdrawn neural-networks book, storage prices, a new inbox, state lawsuits over Grok, and two research approaches to using computation differently. Let's begin.

Speaker1: Michael Nielsen has replaced his online book, Neural Networks and Deep Learning, with a statement explaining why he took it down. The page is dated November twenty twenty-six; a new discussion during our reporting week passed four hundred and seventy comments.

Speaker2: His explanation is an ethical one. He says his expectations have changed since writing the book between twenty eleven and twenty fifteen. He now argues that rapid frontier-AI development is outpacing society's ability to respond to its risks, and doesn't want to help train people to contribute to that work.

Speaker1: Those are Nielsen's judgments, not a new experimental result establishing a particular probability of catastrophe. His argument also extends beyond whether an individual AI system follows instructions: he worries about accelerated discovery of technologies against which societies struggle to defend themselves.

Speaker2: Readers challenge the practical effect of removing educational material. Some argue that restricting people's access to understanding could increase their dependence on models. Others discuss the distinction between present harms and future possibilities. The debate doesn't establish that either effect will follow this particular withdrawal.

Speaker1: What makes this consequential is the concrete choice by an author about how to participate in a field. Whether someone shares his forecast or disagrees with it, the action and the forecast should remain separate objects of discussion.

Speaker2: My takeaway is to read the author's stated reason before supplying one of our own. A resource disappearing can tell us something about its creator's priorities without settling the larger question that motivated the decision.

Speaker1: A major consumer-hardware discussion concerns the price of hard drives. In his November twenty-sixth post, Alex Kretzschmar compares his purchase history with current listings. A twenty-terabyte WD EasyStore he says cost two hundred and forty-nine dollars ninety-nine in November twenty twenty-four is listed for five hundred and forty-nine dollars ninety-nine this Black Friday, before tax, in US dollars.

Speaker2: We checked the retailer's listing, which shows that newer price. That corroborates the listing, rather than independently auditing every historical receipt. It's a three-hundred-dollar difference for the example, not a market-wide price index or proof that every drive doubled in price.

Speaker1: The thread reached nearly five hundred comments. Readers report similar difficulties and debate demand from AI infrastructure, supplier concentration and what alternatives remain. Some allege coordination between manufacturers. The post and those anecdotes don't establish collusion, or isolate how much any one cause contributed.

Speaker2: The article also raises a concrete systems question: what happens when replacing a few disks becomes expensive enough to make redesigning storage attractive? Fewer higher-capacity disks can change the number of slots required, while moving existing data and changing a layout can create work of their own.

Speaker1: That's an example of why capacity price and replacement cost aren't the same question. A particular headline deal says little about the entire cost of maintaining a collection over time.

Speaker2: The takeaway is to keep the exact product, date and unit beside a price comparison. The word sale is doing considerably less work than the number underneath it.

Speaker1: Earlier in the week, Kagi announced the public beta of Kagi Mail. Its November twenty-third post describes hosted email and calendar, support for personal domains and fifty gigabytes of storage. The advertised offer is a sixty-day trial, then ninety-nine US dollars a year plus sales tax, with access included in Kagi Ultimate.

Speaker2: The company says the service uses standard email and calendar protocols, so compatible clients can connect. It also describes optional AI-assisted organisation and inbox search, with a switch to turn AI features off. Those are publisher descriptions; we haven't tested the service or audited its privacy commitments.

Speaker1: Its announcement distinguishes the beta from the roadmap: contacts and native mobile applications aren't all part of the initial offering. In the discussion, approaching four hundred comments, readers compare price, existing providers, future ownership and the trust involved in moving an inbox.

Speaker2: A useful question is what can move independently of the service. A domain, stored mail, calendar data and the habits of everyone using them can have different migration costs. Standard protocols can address part of that without making a transition effortless.

Speaker1: My takeaway is to evaluate the launch and the exit together. The announced feature set tells us what the beta aims to do; compatibility and export options help frame what adopting it would mean over time.

Speaker2: There's also a significant legal development. Virginia's November twenty-third announcement describes separate state actions in Virginia and Oregon against the companies behind X and Grok, including SpaceX. The states allege failures to prevent the generation of child sexual abuse material and non-consensual intimate images, alongside misleading assurances about safeguards.

Speaker1: The Virginia complaint brings a consumer-protection claim. It asks the court for an injunction, consumer restitution, disgorgement and civil penalties. These are requested remedies and allegations in a civil lawsuit, not a judgment establishing liability or a penalty already imposed.

Speaker2: Readers debate platform responsibility and the meaning of assurances about protection. Some comments make broad claims about what courts have already allowed. We aren't treating those comments as legal findings in this case.

Speaker1: The distinction the filing raises is between a company's stated protections and the conduct the state alleges occurred. Evaluating that difference requires evidence about the representations, product behaviour and applicable law. The filing initiates that argument; it doesn't supply the court's eventual answer.

Speaker2: The takeaway is to follow the actual claim and procedural stage. A serious allegation deserves accurate reporting, including that the requested safeguards and financial remedies remain for a court to consider.

Speaker1: Turning to research, the weekly rankings show continuing attention to how models route information and how their abilities are tested. Loom Attention had ninety-four votes in the weekly listing and ninety-six on its opened paper page. The paper was first submitted November twenty-third, revised the twenty-fourth and entered the discovery feed on the twenty-fifth.

Speaker2: What does it change inside a Transformer?

Speaker1: It lets each attention head select among earlier heads' outputs as well as attend across tokens. A per-token matrix memory holds compressed head outputs alongside the usual vector stream. The resulting LoomFormer architecture separates control and content across those two streams.

Speaker2: So it changes the information available when an attention head forms its computation. That is a more specific contribution than saying a network simply thinks harder. It also gives researchers something concrete to compare with other ways of mixing information between layers.

Speaker1: In a reported experiment using three hundred billion training tokens, the two point eight-billion-parameter version uses about two percent extra arithmetic work and matches the twelve-billion-parameter Pythia comparison in zero-shot downstream evaluation. The author also reports reduced wall-clock speed relative to a standard Transformer on the tested hardware. Arithmetic counts and elapsed time aren't interchangeable measurements.

Speaker2: Those are author-reported comparisons, not results we've reproduced. The question is how the trade-off changes across hardware, model scale and workloads. A favourable benchmark comparison doesn't make every larger model unnecessary.

Speaker1: My takeaway is to examine the routing mechanism and the cost measurements together. A small increase in nominal computation can still have a different practical cost, while opening up a useful improvement in what the model learns.

Speaker2: Finally, Friday's third daily paper, Solve Vision with Code, had sixty-three upvotes. First submitted November twenty-fifth, it compares two ways to answer visual tasks: generate the answer video directly, or write a program that renders it.

Speaker1: The authors use five hundred instances across five categories, giving both approaches the same initial frame, prompt and output specification, then applying the same rule-based evaluator. Coding agents get one attempt per instance without access to the hidden answer or generation metadata.

Speaker2: Three tested closed-model coding agents score about point nine-two, point eight-nine and point eight-nine. Each is more than point two-two above the strongest video model in that comparison. Those are benchmark scores, not necessarily percentages of complete tasks solved, and they concern problems computable from the initial frame and prompt.

Speaker1: A reader points out that a coding agent can perform explicit operations and use tools. The author responds by raising a comparison with direct human perception. That exchange doesn't settle how humans reason; it highlights that the systems use different processes even when their inputs and output requirements match.

Speaker2: The useful question is whether a benchmark meant to measure visual reasoning should require the reasoning itself to happen in pixels. If a program reliably constructs the requested outcome, its success challenges that restriction. It doesn't establish an advantage on every open-ended video or perception task.

Speaker1: The memorable result is that a symbolic route deserves a matched comparison with a visual one. We haven't reproduced these experiments, and the paper's stated task boundary belongs beside the headline.

Speaker2: This weekend's discoveries give us concrete choices to examine: withdrawing a resource, comparing a price, offering a new service, bringing a legal claim, and changing an experimental method. Their meaning becomes clearer when the evidence and the limits travel with the claim.

Speaker1: I'm Maya. Thanks for listening to Morning Discovery.

Speaker2: And I'm Jax. Have a good Sunday.
