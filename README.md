### Kevin Madden

**Healthcare leader and pharmacist who designs and tests AI tools for clinical and pharmacy work.**

My 15+ years at CVS span my total employment, from the pharmacy counter to leading care teams and rolling out clinical programs and technology across many sites. That experience shapes the questions I test: what counts as evidence, what a tool misses and when a person must decide.

**How I work:** Start with a problem from the field, build, measure, and publish the limits.

### Selected public work

**[Clinical evidence map](https://github.com/kvmadden/clinical-evidence-map)**

A nurse reviewing a faxed prior-authorization packet needs evidence for each criterion, not just a summary. I designed the service pipeline and chose source quotes for every finding, with uncertain items sent to the nurse. [Try the synthetic packet demo](https://kvmadden.com/projects/clinical-evidence-map/).

On 24 blind synthetic packets written by other AI models, it got 85 of 120 criterion statuses right, against 49 of 120 for always answering “found”, while sending 72 of 120 to review. It misses the 90% target. The reference labels are drafts pending my review as a pharmacist, and the run does not establish clinical accuracy or time saved.

**[Redaction gate](https://github.com/kvmadden/pii-redaction-gate)**

Clinical-style text mixes identifying details with useful context. I built a local rules engine, chose separate profiles to preserve clinical content and made the send gate block on engine failure. [Step through the synthetic note demo](https://kvmadden.com/projects/pii-redaction-gate/).

On one blind local evaluation of 132 synthetic documents, 12 of 2,577 identifiers remained in documents marked clean, against 701 for offline Microsoft Presidio. The gate sent 120 of 132 documents to a person, and 8 of the 12 marked clean still held an identifier. Presidio has no review step, so those headline counts include different review policies. This is not validation on real records or permission to send patient text.

**More AI systems and evaluation**

- [knowledge-mcp](https://github.com/kvmadden/knowledge-mcp): shared agent memory where every save passes one gate, with audit decisions and dry-run review. On a blind test of 564 synthetic writes, it made 295 right calls, against 227 with no gate and 257 for Microsoft Presidio. It caught only 2 of 48 names and addresses written in prose, and it held 65 of 216 harmless writes for a reviewer.
- [local-model-workshop](https://github.com/kvmadden/local-model-workshop): a pharmacist's schema review changed the extraction task. On 37 short synthetic medication lines, three local models got every field right on 24 to 25 of 25 lines and 10 to 12 of 12, and a short rules parser did as well. No model is chosen until a new blind test set runs.
- [jargon](https://github.com/kvmadden/jargon): personalized AI explanations, each checked by the same model before it's shown. An offline eval found 5 wrong outputs among 78 accepted (6.4%), a floor from partial expert review.

**Clinical learning and agent tooling**
- [counter-intelligence-sim](https://github.com/kvmadden/counter-intelligence-sim): vaccine conversation practice with 24 CDC-sourced claims across five fictional patients. The build blocks missing sources or author review stamps. [Case page](https://kvmadden.com/projects/counter-intelligence-sim/)
- [vax-or-fiction-game](https://github.com/kvmadden/vax-or-fiction-game): immunization discussion game with 150 distinct questions and citations on all 180 question appearances. Content has no clinical review.
- [operator-skills](https://github.com/kvmadden/operator-skills): a Claude Code plugin of 10 skills and 118 rules for agent-assisted coding. In a small live eval on November 3, Claude Code loaded none of its skills in 12 of 12 plugin runs, so as shipped it had no measured effect.

[More selected work](https://kvmadden.com/projects)

Most of my other work is private because it's built around real teams. Public demos use fictional or synthetic patient scenarios. Some benchmarks also use cited public source text.

[LinkedIn](https://www.linkedin.com/in/kvmadden/) · [kevin@kvmadden.com](mailto:kevin@kvmadden.com)
