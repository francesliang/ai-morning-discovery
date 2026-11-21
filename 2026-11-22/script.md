Speaker1: Good morning, and welcome to Morning Discovery for Sunday, November twenty-second, twenty twenty-six. I'm Maya.

Speaker2: And I'm Jax. Big ideas, useful context, and a robot that still can't ask the world to pause for coffee.

Speaker1: This is our weekend edition, covering seven oh-five a.m. on November fifteenth to seven oh-five a.m. on November twenty-second, Melbourne time, Australian Eastern Daylight Time.

Speaker2: On the menu: a major mathematics verification update, Brazil's open tax calculator, a looping language model, and research into understanding video and evaluating robots. Let's get into it.

Speaker1: Yesterday, we reported proposed Riemann Hypothesis proofs and checks still in progress. There is now a substantial development. In a November twenty-first joint statement, the Lean and Mathlib communities certify that both the statement and proof of the Riemann Hypothesis in Levent Alpöge's library are correct. The statement is endorsed by the Lean FRO and Mathlib Initiative.

Speaker2: What did they check beyond whether a large software project successfully builds?

Speaker1: They report checking the mathematical statement against Mathlib's established definition, compiling the library, comparing the theorem against that statement using two tools, and checking the exported proof using multiple checkers. They also say the checks operated on an inert export, away from potentially interfering source code. Those are separate parts of the verification argument.

Speaker2: Andrew Sutherland at MIT has published a detailed audit too. It lists successful module-level checks and independent checker results, alongside some runs still marked in progress. Its status table is a snapshot, rather than a claim that every listed checking route has finished. We haven't executed the proof ourselves.

Speaker1: The scope matters. The joint statement explicitly certifies the Riemann Hypothesis. We should preserve that wording when discussing the wider Generalized Riemann Hypothesis announcement, and keep the separate human-written proposal separate.

Speaker2: The new thread passed four hundred comments. Readers ask about matching the intended theorem, the assumptions beneath proof checkers, and what mathematicians can learn from the argument. The community statement looks forward to explaining the proof's ideas. Verification and explanation can advance at different speeds; that doesn't make either activity unimportant.

Speaker1: The takeaway is to update our confidence when substantive checking appears, while saying exactly which result was checked. A formal result can become much better established before its mathematical strategy becomes easy to teach.

Speaker2: Earlier in the week, Brazil's federal revenue authority announced a different kind of inspectable artifact: its consumption-tax reform calculator in public GitHub repositories under the MIT licence. The announcement was published November sixteenth. The code had already been downloadable through another official platform since last year; collaborative publication is the new step.

Speaker1: The authority says businesses and software suppliers can incorporate its calculation logic into their existing systems, with calculation records and legal grounding. The regular-regime repository describes an API for calculating the relevant taxes, looking up official tables, and generating or validating tax-document fields. This is a reusable component, rather than a replacement for every business system.

Speaker2: That distinction gets attention in the discussion, which had roughly a hundred and ninety comments in the weekly snapshot. Readers debate whether governments should publish the software implementing public rules. Others distinguish this business-tax calculation release from opening an entire personal income-tax filing application. We shouldn't stretch one announcement to cover both.

Speaker1: My reading is that a shared implementation could reduce a particular source of disagreement: separate developers translating the same rule into slightly different calculations. It also creates somewhere concrete to investigate a surprising result. That is an opportunity for scrutiny, not proof that every calculation or integration will be correct.

Speaker2: Open code still needs maintained versions, appropriate inputs and checks against the situation being represented. A calculator can faithfully implement a rule while someone applies it to the wrong case. The useful question is whether the official component makes those boundaries clearer and disagreements easier to reproduce.

Speaker1: The takeaway is that publishing rules and publishing an inspectable implementation offer different kinds of access. Both can matter when a policy has to become working software.

Speaker2: Thinking Machines Lab's November twentieth release, Inkling Two Mini, changes how a model spends computation. It runs its middle layers three times for each token. That's a loop inside the model, rather than simply asking it to write a longer answer.

Speaker1: The publisher reports twenty-six point four billion total parameters and three point four billion active, rising to five point four billion weight activations when repeated use is counted. Its stated memory footprint is around twenty gigabytes. Those figures describe different things; the active parameter count isn't the amount of memory needed to store the whole model.

Speaker2: The release reports forty-eight point two percent on Deep SWE version one point one. It also acknowledges weaker results on demanding multi-turn conversation and instructions with many constraints. These are publisher evaluations, with setup differences across comparisons, not a demonstration that a small model wins every task.

Speaker1: In the roughly two-hundred-and-seventy-comment discussion, readers welcome local use but debate the trade-off between memory capacity, bandwidth and repeated computation. Some ask whether benchmark gains will survive everyday workloads. That's a practical disagreement about the entire system, rather than a vote on whether looping is clever.

Speaker2: Imagine a task that needs three passes over a compact working process. Reusing machinery could help avoid storing a much larger machine, while each extra pass still takes work. That analogy explains the attraction; it doesn't predict the speed on a particular laptop.

Speaker1: The takeaway is to evaluate the work completed, response time and resource use together. A model that fits locally is an interesting starting point. Whether it fits the job depends on what it can reliably finish.

Speaker2: Turning to research, Friday's third-ranked Hugging Face daily paper was WeMM-Video, with forty-three upvotes in our snapshot. The original paper appeared November nineteenth, followed by discovery-feed attention on the twentieth. It concerns understanding video together with its sound.

Speaker1: The authors introduce Chinese-English models in several sizes, combining text, images, audio and video. They support a direct-answer mode and a mode with explicit step-by-step reasoning. Training uses approximately one point two trillion multimodal tokens, and the report evaluates more than a hundred and twenty benchmarks.

Speaker2: The authors report leading open-model results in their joint audio-video evaluations and release an evaluation and reproduction pipeline. We haven't reproduced those comparisons. A broad benchmark collection is useful evidence, but doesn't settle the reliability of every individual capability or recording condition.

Speaker1: Here's a question the work raises. Suppose a recording shows two people, while a sound comes from outside the frame. A useful system has to connect the right evidence without automatically assigning every sound to the visible person. Fluent description alone wouldn't tell us whether it made that connection correctly.

Speaker2: Or consider a question whose answer changes if the soundtrack is removed. Testing that difference can reveal whether the audio contributes useful evidence. That's our example of an evaluation question, not an experiment we've run on this model.

Speaker1: My takeaway is to ask which combinations of evidence a video system actually handles, and how failures change when one channel becomes ambiguous.

Speaker2: The weekly paper rankings also highlight embodied systems. Envisioning Agentic Robotics had a hundred and thirty-six upvotes. Its paper was first submitted November thirteenth, before our window, and entered the daily discovery feed on November sixteenth. It's a research roadmap and evaluation proposal, rather than a newly demonstrated autonomous robot.

Speaker1: One concrete proposal concerns the clock. The authors argue that evaluations should distinguish a simulated world paused during model inference from a world that continues changing. Their project illustrates a cup moving on a belt: the same reasoning delay leaves a robot acting on older information when the belt keeps running.

Speaker2: The cup has declined the meeting invitation to wait for further reasoning.

Speaker1: They also propose fixing the surrounding system when comparing models, and fixing the model when comparing surrounding systems. Otherwise, a changed interface or verification process can be mistaken for a model improvement. These are methodological proposals, not measured universal gains from adopting the framework.

Speaker2: A reader raises another practical issue: a job site can reveal conditions that the original plan didn't anticipate, and a robot may need to stop and ask. An author replies that this belongs within the framework's safety dimension. That exchange makes the evaluation question concrete without establishing that the problem has been solved.

Speaker1: The roadmap distinguishes individual actions, complete tasks, coordinated workflows and continuing responsibilities. Being able to finish one episode doesn't establish dependable performance over days. The authors describe sustained roles as a target for development and evaluation.

Speaker2: My takeaway is to ask whether the test gives the robot the same deadlines, changing surroundings and responsibility it would have in use. A high score means more when the world in the test behaves like the world outside it.

Speaker1: This weekend's discoveries give us several different forms of progress: stronger verification, inspectable public software, a new computation trade-off, and proposals for better evaluation. Their practical value depends on the details we can inspect and the conditions under which they hold.

Speaker2: I'm Jax. Enjoy your Sunday, preferably somewhere without a moving conveyor belt.

Speaker1: I'm Maya. Thanks for listening to Morning Discovery. Have a good morning.
