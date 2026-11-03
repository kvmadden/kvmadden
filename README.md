### Kevin Madden

**Healthcare leader and pharmacist who designs and tests AI tools for clinical and pharmacy work.**

I bring a clinician's view from 15+ years in healthcare: caring for patients, leading care teams, and rolling out new clinical programs and technology across many sites.

**How I work:** Start with a problem from the field, build, measure, and publish the limits.

### Selected public work

**AI systems and evaluation**
- [clinical-evidence-map](https://github.com/kvmadden/clinical-evidence-map): a review workspace for faxed prior-authorization packets that quotes the source words for every finding and marks uncertain criteria for a nurse to review. On 24 blind packets written by other AI models, it got 85 of 120 criterion statuses right, against 49 for always answering found, by sending 72 of 120 to review. That's short of its 90% target, and the labels are drafts pending pharmacist review.
- [pii-redaction-gate](https://github.com/kvmadden/pii-redaction-gate): clinical text redaction that removes the identifiers it finds before any model sees the text, and blocks the send if the redactor itself fails. On a blind test of 132 synthetic clinical documents written by other AI models, it left 12 of 2,577 identifiers in documents it marked clean, against 701 for Microsoft Presidio, by sending 120 of the 132 to a person. Not validated for clinical use.
- [knowledge-mcp](https://github.com/kvmadden/knowledge-mcp): shared agent memory where every save passes one gate, with audit decisions and dry-run review. On a blind test of 564 synthetic writes, it made 295 right calls, against 227 with no gate and 257 for Microsoft Presidio. It caught only 2 of 48 names and addresses written in prose, and it held 65 of 216 harmless writes for a reviewer.
- [local-model-workshop](https://github.com/kvmadden/local-model-workshop): a pharmacist's schema review changed the extraction task. On 37 short synthetic medication lines, three local models got every field right on 24 to 25 of 25 lines and 10 to 12 of 12, and a short rules parser did as well. No model is chosen until a new blind test set runs.
- [jargon](https://github.com/kvmadden/jargon): personalized AI explanations, each checked by the same model before it's shown. An offline eval found 5 wrong outputs among 78 accepted (6.4%), a floor from partial expert review.

**Clinical learning and agent tooling**
- [counter-intelligence-sim](https://github.com/kvmadden/counter-intelligence-sim): vaccine conversation practice with 24 CDC-sourced claims across five fictional patients. The build blocks missing sources or author review stamps. [Play](https://counter-intelligence.vercel.app)
- [vax-or-fiction-game](https://github.com/kvmadden/vax-or-fiction-game): immunization discussion game with 150 distinct questions and citations on all 180 question appearances. Content has no clinical review.
- [operator-skills](https://github.com/kvmadden/operator-skills): a Claude Code plugin of 10 skills and 118 rules for agent-assisted coding. In a small live eval on November 3, Claude Code loaded none of its skills in 12 of 12 plugin runs, so as shipped it had no measured effect.

[More selected work](https://kvmadden.com/projects)

Most of my other work is private because it's built around real teams. All data in public code and demos is fictional or synthetic.

[LinkedIn](https://www.linkedin.com/in/kvmadden/) · [kevin@kvmadden.com](mailto:kevin@kvmadden.com)
