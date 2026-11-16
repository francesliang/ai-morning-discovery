Speaker1: Good morning, and welcome to Morning Discovery for Tuesday, November seventeenth, twenty twenty-six. I'm Maya.

Speaker2: And I'm Jax. Today, the models are getting bigger, the discount labels need a second look, and the game-playing agents have homework.

Speaker1: This is our daily edition, covering seven oh-three a.m. on November sixteenth to seven oh-three a.m. on November seventeenth, Melbourne time, Australian Eastern Daylight Time.

Speaker2: On the menu: Qwen's new flagship, a study of Amazon sale prices, and research into agents that can act, remember and check their work. Let's begin.

Speaker1: Alibaba released Qwen Four Max on November sixteenth. The announcement describes a model with native vision, a million-token context window, and a mixture-of-experts architecture containing two point four trillion parameters. The company says seventy-one billion parameters are active for each token.

Speaker2: Those two parameter counts describe different things: the overall model and the portion used for a particular computation. The very large total doesn't mean every parameter participates in every step. That helps explain why an architecture change can matter alongside a bigger headline number.

Speaker1: Alibaba's most useful efficiency claim is conditional. On its proprietary Work Three Sixty benchmark, it reports stronger overall performance than Qwen Three Point Eight Max while using thirty-five percent fewer tokens at the high reasoning setting, with average cost per task reduced by around sixty percent. Those are company-reported results in its evaluation, not savings we've reproduced across other workloads.

Speaker2: And availability needs a separate label. The release is offered through QwenCloud and Alibaba applications. The announcement promises smaller open-weight Qwen Four models later; it doesn't announce an open-weight download for the flagship itself.

Speaker1: The discussion attracted about four hundred and fifty comments. One lively exchange concerns the familiar test of asking a model to draw a pelican riding a bicycle. Some readers see a useful, consistent demonstration of visual and spatial details. Others question whether a widely repeated prompt still tests unfamiliar work, and point out variation between runs. The thread doesn't establish that this particular test contaminated the training data.

Speaker2: Somewhere, a pelican is wondering why its bicycle keeps appearing in performance reviews. The serious takeaway is to distinguish a memorable demo from a representative evaluation. For a workflow, the useful comparison is the quality and cost of a completed task under comparable conditions.

Speaker1: Turning to shopping, Groundwork Collaborative published a November sixteenth investigation into Amazon's Black Friday and Cyber Monday promotions. It examined more than three hundred and fifty products featured on Amazon's own deal pages for the twenty twenty-four and twenty twenty-five events.

Speaker2: So the study isn't measuring this year's sale, and the sample isn't every item Amazon sells. It's asking whether selected promotions beat prices available shortly beforehand.

Speaker1: Using historical pricing data, the authors report that twenty-nine point one percent of the sampled products had been available for the same price or less during the preceding thirty days. Nine point four percent were more expensive during the sale than an earlier price in that period. The second figure is part of the first group, not another group to add on top.

Speaker2: That denominator matters. A price lower than a reference label and a price lower than last week's offer are different comparisons. A large discount badge can be visually persuasive while leaving the more useful comparison unanswered.

Speaker1: Groundwork is an economic think tank and advocacy organisation. These are its findings, which we haven't independently reproduced. Its report also proposes showing customers a product's lowest price over the previous thirty days. That's a policy recommendation from the authors, not a new requirement announced by this study.

Speaker2: In the roughly four-hundred-comment discussion, some shoppers describe cancelling subscriptions or ordering less often to reduce impulse purchases. Others defend the convenience and delivery speed, or question whether competing retailers provide an equally good overall experience. Those personal accounts don't independently validate the pricing sample.

Speaker1: The takeaway is to ask what a claimed saving is relative to. Price history, a genuine need for the item and the final amount paid answer different questions. A promotion can be convenient without being the lowest recent price.

Speaker2: Now a security disclosure about uBlock Origin. Researcher Smitty van Bodegom describes an issue in the Firefox version's element picker, the interface used to select parts of a page to block. The disclosure gained fresh discussion on November sixteenth, although the fixes arrived earlier.

Speaker1: The important boundary is between a website and an extension's trusted controls. In the reported attack, a malicious site could manipulate the picker and trick a user's click into creating a trusted filter. That could let code run in the context of another website. This required particular conditions; it isn't a claim that simply having any ad blocker installed makes every page exploitable.

Speaker2: The maintainer's advisory lists version one point seventy-five point two and earlier as affected, and one point seventy-five point four as patched. It dates that patch to November third, with additional hardening in one point seventy-six point zero on November eighth. The new event is public disclosure and explanation, rather than a fix released today.

Speaker1: In the discussion, participants question why an extension's interface must share space with the page it is trying to control. One contributor argues for a browser-provided overlay that websites cannot interfere with. That's a design argument from the thread, not a new browser feature being announced.

Speaker2: The researcher also says an AI model helped find the issue and that he verified the finding. That is his account of the investigation. The broader lesson is that an interface can look like a trusted tool while still interacting with an untrusted page. Authenticating those interactions is part of the security boundary.

Speaker1: Today's research rankings put embodied agents and verification in focus. Gamer was published on November thirteenth and submitted to Hugging Face's daily papers on the sixteenth. It ranks second in our snapshot with eighty-seven upvotes, so the discovery attention is newer than the paper.

Speaker2: The miHoYo team's agent plays through screenshots and keyboard-and-mouse actions. The authors say it doesn't receive privileged game state or game-specific control APIs. That makes observing, remembering and acting through an interface central to the task.

Speaker1: The project describes training on more than ten thousand hours of gameplay. It samples screenshots five times a second, while its action representation supports keyboard control at thirty updates a second. Seeing a new frame and issuing a control signal needn't happen at the same frequency.

Speaker2: It also trains the agent to reason at important decisions and retain summaries as older interactions leave the active context. Remembering an unfinished objective is different from keeping every previous screenshot in view. The system needs to preserve what matters for the next action.

Speaker1: The authors report handling more than ninety-five percent of challenges across studied main storylines in Honkai: Star Rail. That's a result claimed for their evaluation, not evidence of the same success in every game, or in a physical robot. The project also studies puzzles and other games, but broad transfer remains something to measure.

Speaker2: The question raised by the work is how well the agent recovers when memory is incomplete or a plan stops matching the screen. That's a question to test, rather than a result established by those headline scores. My takeaway is that real-time performance depends on the whole loop: observations, memory, decisions and action timing.

Speaker1: Finally, Vibe Previs Bench asks whether a coding agent can build an animated scene that actually matches a brief. Published November eleventh, it gained attention on the sixteenth, ranking third with eighty-three upvotes. The benchmark has two hundred and forty-two tasks and evaluates eleven coding agents.

Speaker2: The agent creates an executable scene in Blender and renders a simplified preview video. The fourth dimension here is time: objects and cameras can move, and a request may span multiple shots. A scene that looks plausible in one still image can fail the animation brief.

Speaker1: Evaluation has two parts. A rule-based check reruns the code and compares the underlying scene with hidden facts across nine dimensions. A separate vision-language-model judge checks whether qualifying facts can actually be recognised in the rendered preview. The stored scene and what the viewer sees are separate things to inspect.

Speaker2: The authors report that basic staging and camera work are much easier than demanding spatial and camera-motion requests. They also find agents inspecting their renders without successfully correcting the mistakes. These are findings in this benchmark, not a claim that every generated scene fails.

Speaker1: One reader's comment praises checking the scene and screen separately, then asks which dimensions caused the most trouble. It's a useful question because a successful render alone doesn't tell us which requirements were met. A model-based judge also introduces its own limits; this isn't a substitute for every form of human production review.

Speaker2: The takeaway is that looking at an output and verifying it are different actions. A useful revision loop needs a specific requirement, a check against the result and a correction tied to the mismatch. Admiring the preview is the easy part.

Speaker1: Today's recap: Qwen's release makes efficiency claims worth testing at the task level; the pricing study asks what a discount is compared with; and the extension disclosure shows why trusted controls need a firm boundary. The research adds memory, timing and concrete verification to the agent checklist.

Speaker2: I'm Jax. May your next preview contain everything the brief asked for, and your next sale price have a useful comparison.

Speaker1: I'm Maya. Thanks for listening to Morning Discovery. Have a good Tuesday.
