### Kevin Madden

**Healthcare leader and pharmacist who designs and tests AI tools for clinical and pharmacy work.**

I bring a clinician's view from 15+ years in healthcare: caring for patients, leading care teams, and rolling out new clinical programs and technology across many sites.

**How I work:** Start with a problem from the field, build, measure, and publish the limits.

### Selected public work

**AI systems and evaluation**
- [clinical-evidence-map](https://github.com/kvmadden/clinical-evidence-map): a review workspace for faxed prior-authorization packets that quotes the source words for every finding and marks uncertain criteria for a nurse to review. Its scores come from development packets built by the same generator its rules were written against, so they aren't quoted as results. Labels are drafts pending pharmacist review.
- [pii-redaction-gate](https://github.com/kvmadden/pii-redaction-gate): clinical text redaction that removes the identifiers it finds before any model sees the text, and blocks the send if the redactor itself fails. No test score is quoted: the synthetic notes it was scored on shaped some of its rules. Not validated for clinical use.
- [knowledge-mcp](https://github.com/kvmadden/knowledge-mcp): shared agent memory where every save passes one gate, with audit decisions and dry-run review. No planted test value reached storage in 324 tests. On its own attack set, whose phrasings were visible while the rules were written, it now stops 4 of 6 kinds it used to miss. It still misses encoded instructions and false clinical claims, and it can refuse a harmless write.
- [local-model-workshop](https://github.com/kvmadden/local-model-workshop): a pharmacist's schema review changed the extraction task. The chosen model got every field right on 25 of 25 lines in both runs, and on 12 of 12 later lines built from the same six patterns. Speed counts against it: on those 12 lines the other two models stayed under the 10-second limit and it did not, so the choice is provisional.
- [jargon](https://github.com/kvmadden/jargon): personalized AI explanations, each checked by the same model before it's shown. An offline eval found 5 wrong outputs among 78 accepted (6.4%), a floor from partial expert review.

**Clinical learning and agent tooling**
- [counter-intelligence-sim](https://github.com/kvmadden/counter-intelligence-sim): vaccine conversation practice with 24 CDC-sourced claims across five fictional patients. The build blocks missing sources or author review stamps. [Play](https://counter-intelligence.vercel.app)
- [vax-or-fiction-game](https://github.com/kvmadden/vax-or-fiction-game): immunization discussion game with 150 distinct questions and citations on all 180 question appearances. Content has no clinical review.
- [operator-skills](https://github.com/kvmadden/operator-skills): 10 coding-agent skills and 117 correction rules, with 28/28 synthetic routing checks passing. Live agent behavior is unmeasured.

[More selected work](https://kvmadden.com/projects)

Most of my other work is private because it's built around real teams. All data in public code and demos is fictional or synthetic.

[LinkedIn](https://www.linkedin.com/in/kvmadden/) · [kevin@kvmadden.com](mailto:kevin@kvmadden.com)
