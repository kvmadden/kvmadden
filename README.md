### Kevin Madden, PharmD

**Healthcare leader and pharmacist who designs, builds and tests AI and clinical software.**

I bring a clinician's view from 16 years in healthcare: caring for patients, leading care teams, and rolling out new clinical programs and technology across many sites.

**How I work:** Start with a problem from the field, build, measure, and publish the limits.

### Selected public work

**AI systems and evaluation**
- [pii-redaction-gate](https://github.com/kvmadden/pii-redaction-gate): clinical text redaction with 90.3% identifier recall on the original synthetic set and 96.3% on a frozen held-out set. [Every miss published](https://github.com/kvmadden/pii-redaction-gate/blob/main/eval/comparison.md), not validated for clinical use.
- [knowledge-mcp](https://github.com/kvmadden/knowledge-mcp): shared agent memory with audit decisions and dry-run review before resubmission. Frozen red-team set: 30/40 risky writes blocked, 5/20 benign writes falsely blocked.
- [local-model-workshop](https://github.com/kvmadden/local-model-workshop): a pharmacist's schema review changed the extraction task. Qwen scored 12/12 on the frozen synthetic holdout under the revised schema, but missed the latency budget.
- [jargon](https://github.com/kvmadden/jargon): personalized AI explanations with a second-model check. An offline eval found 5 wrong outputs among 78 accepted (6.4%), a floor from partial expert review.

**Clinical learning and agent tooling**
- [counter-intelligence-sim](https://github.com/kvmadden/counter-intelligence-sim): vaccine conversation practice with 24 CDC-sourced claims across five fictional patients. The build blocks missing sources or author review stamps. [Play](https://counter-intelligence.vercel.app)
- [vax-or-fiction-game](https://github.com/kvmadden/vax-or-fiction-game): immunization discussion game with 150 distinct questions and citations on all 180 question appearances. Content has no clinical review.
- [operator-skills](https://github.com/kvmadden/operator-skills): 10 coding-agent skills and 117 correction rules, with 28/28 synthetic routing checks passing. Live agent behavior is unmeasured.

[More selected work](https://kvmadden.com/projects)

Most of my other work is private because it's built around real teams. All data in public code and demos is fictional or synthetic.

[LinkedIn](https://www.linkedin.com/in/kvmadden/) · [kevin@kvmadden.com](mailto:kevin@kvmadden.com)
