Speaker1: Good morning, and welcome to Morning Discovery for Wednesday, November eleventh, twenty twenty-six. I'm Maya.

Speaker2: And I'm Jax. Today, a smaller AI bill, a very large proof, and a drum machine that mercifully doesn't need a system prompt.

Speaker1: This is our daily edition, covering seven a.m. on November tenth to seven a.m. on November eleventh, Melbourne time, Australian Eastern Daylight Time.

Speaker2: On the menu: Amazon's ticket-sorting experiment, a carbon headline with an important qualification, and robots learning a common language of touch. Let's get into it.

Speaker1: Amazon engineers describe replacing Claude Sonnet 4.6 in a high-volume internal ticket-labeling workflow with Strands Decider. The job chooses among twenty categories. Their November ninth write-up gained substantial discussion in our window. They report a ninety-eight percent cost reduction for this particular task.

Speaker2: The distinction is that Decider chooses from supplied options rather than writing an answer. If the entire job is choosing a drawer, you might not need a novelist to label the filing cabinet.

Speaker1: The team tested a Gemma-based build, adjusted its confidence threshold, and compared both systems on real traffic before switching. Their published cost comparison is approximately twenty-two thousand two hundred dollars versus five hundred dollars per million tickets. Those are their figures, with utilisation assumptions; they are not independently reproduced savings for an arbitrary business.

Speaker2: There are compromises. Long tickets lose their oldest comments to fit the smaller context. The team also reports that changing the order of JSON keys shifted probabilities, so they standardised the order. A narrow task can still have surprisingly sensitive plumbing.

Speaker1: The Hacker News discussion, at roughly two hundred and twenty-eight comments, asks whether this is a return to ordinary classification. Some participants point to older, fast ticket-routing systems. Others argue that general pretrained models reduce the data and feature-engineering work needed to get started. The useful takeaway is to define the decision before selecting the model.

Speaker2: A related discussion was even busier: Evan Merz's November seventh essay about fragile AI-generated codebases, now drawing around two hundred and eighty-two comments. He argues that shallow tests and narrow task focus can miss long-term engineering problems. This is a practitioner's account, not a controlled study of every coding model.

Speaker1: Replies question whether the underlying cause is AI or organisational pressure to ship, and whether experienced developers can retain architectural responsibility while delegating code. Those positions can overlap. The question raised by both stories is what the surrounding process measures. A lower inference bill and a healthier codebase are different outcomes; neither proves the other.

Speaker2: Now for that very large proof. Google DeepMind announced AlphaProof Code on November tenth. Researchers used human-reviewed specifications and AI proof agents to verify key security properties of a build using libsignal, the Signal protocol's reference implementation, down to machine code.

Speaker1: Their technical paper describes about six and a half million lines of machine-checked Lean proofs, supported by trusted specifications and a model of the processor's instructions. The work connects protocol guarantees to compiled implementation. That's a meaningful step beyond checking an abstract protocol while leaving the implementation gap unexplored.

Speaker2: But six million lines is a quantity, not a magic spell. What exactly has to remain trustworthy?

Speaker1: The specification, the checking machinery, and the stated assumptions. The paper explicitly limits the result to its build and environment. Its computational security theorem has restrictions on the attacker, and it does not cover Signal's complete applications or multi-device state. It also does not establish a general guarantee against a quantum attacker. Those boundaries matter alongside the achievement.

Speaker2: The discussion, around a hundred and sixty-three comments in our front-page snapshot, turns on that distinction. Some readers initially interpret verification as meaning no bugs anywhere. Others emphasise that proofs establish specified properties under assumptions. My takeaway: the exciting development is cheaper, deeper assurance of particular guarantees. A proof still needs a clearly stated job description.

Speaker1: Our next story needs a careful reading of the headline. The Global Carbon Project's new annual budget projects fossil carbon dioxide emissions down zero point four percent in twenty twenty-six, to thirty-eight point two billion tonnes. Exeter's November tenth announcement attributes the change to clean-energy expansion and an oil-demand shock associated with the Iran conflict.

Speaker2: So that's a projected fall in fossil emissions, rather than a completed measurement of the whole year. And fossil emissions aren't the entire carbon account.

Speaker1: Correct. Including land-use change, Exeter reports projected total carbon dioxide emissions of forty-three point three billion tonnes, compared with forty-two point eight billion last year. The budget preprint was posted on November tenth and is under review. The researchers warn that clean-energy growth is not yet fast enough to secure a durable fall in fossil emissions.

Speaker2: In the discussion, with roughly a hundred and seventy-seven comments, people distinguish annual emissions from the amount already accumulating in the atmosphere. Others debate whether disrupted fossil supplies will accelerate clean-energy adoption or produce a temporary dip. Those are different questions: the size of this year's flow, the accumulated stock, and what happens next.

Speaker1: The practical reading is that a small projected fossil decline can coexist with rising total emissions. It is evidence to examine, not a declaration that warming has stopped. Watch the scope of the number and whether the changes behind it persist.

Speaker2: Let's move from planetary accounting to making music. Ableton's Live 13 announcement attracted about two hundred and thirty-five comments. The product page says release is planned for early twenty twenty-seven, with limited public-beta places. This is an announced upgrade, not a claim that the finished release is already in everyone's studio.

Speaker1: The listed additions include step-sequencer clips, support for compatible ARA 2 audio-editing plug-ins, and Capture Automation, which turns control movements into recorded automation. A new Drum Synth offers more than twenty engines. Features vary by edition, and the publisher notes compatibility limits.

Speaker2: Capture Automation is an appealing idea: keep the interesting knob movement before your brain has time to say, actually, let's spend forty minutes recreating that. The significance is workflow. Helping a musician preserve an experiment can be as useful as adding another sound generator.

Speaker1: The discussion also explores programming inside the music environment. One developer describes their Scheme extension for Max for Live, and replies compare timing, scripting and other live-coding tools. That extension is their separate project, not a newly announced built-in Live 13 feature.

Speaker2: My takeaway is to distinguish the release's own capabilities from the ecosystem around it. Both can matter, but they answer different questions about how someone actually makes a track.

Speaker1: Now to research. LingBot-Touch led the November tenth Hugging Face daily board with ninety-two upvotes in our snapshot, and also led the current weekly board. The paper was originally published November ninth. It addresses a basic robotics problem: touch sensors based on different physical mechanisms do not naturally speak the same data language.

Speaker2: A pressure-sensitive sensor, a magnetic sensor and a camera-based tactile sensor can all help a robot understand contact. But swapping one for another should not mean teaching the robot the entire alphabet again.

Speaker1: The authors propose a shared representation across those sensor types. They turn tactile information into tokens that can be integrated with different control policies, including diffusion policies and vision-language-action models. They report benefits in simulation and on real robots across multiple hardware platforms.

Speaker2: Those are author-reported findings. They don't establish that any new sensor works without adaptation, or that a robot can now manipulate every unfamiliar object. The question raised by the work is how much useful knowledge transfers when the sensing hardware changes. That's especially important when a policy has to act on contact, rather than only recognise an object in an image.

Speaker1: The memorable contribution is the interface: making heterogeneous touch data useful to a common learning system. We have a method and reported experiments, rather than a universal dexterity guarantee.

Speaker2: Our final discovery, WorldFoundry, tackles the infrastructure for evaluating world models. Published November seventh and submitted to the feed on November tenth, it had fifty-two upvotes and ranked second on the daily board. The weekly board also shows strong interest in embodied systems and reproducible evaluation.

Speaker1: WorldFoundry's concrete contribution is a shared framework for discovering models and benchmarks, preparing runtimes, running evaluations and preserving the resulting evidence. Its catalog reports two hundred and seventy model entries, seventy-four benchmarks and sixty-two metric entries. Importantly, it records whether something is ready to execute separately from what has actually been demonstrated.

Speaker2: That's the distinction between a restaurant being listed in a guide and someone actually having eaten there. A model entry isn't an evaluation result.

Speaker1: The framework spans video, spatial and embodied systems while retaining their different inputs and evaluation protocols. The authors argue for tracing claims back to durable artifacts. That could make comparisons easier to audit; catalog size alone doesn't establish fair comparisons or validated performance across every entry.

Speaker2: My takeaway is to ask for the run behind the score. Shared infrastructure can help researchers answer that question, provided the evidence remains inspectable.

Speaker1: Today's recap: a smaller model can be a better fit for a bounded decision; a machine-checked proof still depends on its specification; and a projected fossil-emissions decline needs its wider context. We also have new creative tools, transferable touch representations and more auditable research infrastructure.

Speaker2: Plenty to explore, and at least one filing cabinet spared an unnecessary essay. I'm Jax.

Speaker1: And I'm Maya. Thanks for listening to Morning Discovery. Have a good Wednesday.
