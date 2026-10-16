Today's Field Developments

1. First Proof Third Batch — public research-mathematics evaluation, 14 October
   
Mohammed Abouzaid, Nikhil Srivastava, Rachel Ward, and Lauren Williams published the third First Proof benchmark report through Hexagon, with the problem set and supplementary artifacts linked from the project page [1–3]. Ten naturally occurring research-mathematics problems, each with a human-known proof of at most 12 pages, were tested from 2–5 October. Five systems received one shot per problem, up to 24 hours, with no human interaction; about 30 expert referees separately scored correctness, exposition, and attribution. The rubric ranges from −1 to 1, including negative scores for harmful incorrect submissions [1].

2. A $15 million community initiative on mathematics and AI — announced 15 October

The Simons Foundation announced a combined $15 million commitment with Anthropic and OpenAI to support workshops and community initiatives for evaluating AI-assisted mathematical results, learning to use tools, and developing shared standards. OpenAI separately states that its contribution is $5 million and that it will provide models and computing resources to researchers supported by the foundation [4, 5]. This is a research-infrastructure and governance development, not a new mathematical theorem or benchmark result.

Important Research Developments and Critical Assessment

1. First Proof Batch 3: high solve counts coexist with persistent research-quality failures
   
Main reported result. Using the report’s correctness threshold of at least 0.5, ProofCouncil solved 9/10 problems, direct GPT-6 Astra 7/10, MerLean 4/10, Anthropic’s Siege 3/10, and Humanize, built around the open-weight Kimi K3 model, 0/10. Every benchmark problem was solved correctly by at least one system when citation and exposition were set aside. Reported total costs were approximately $1,888 for ProofCouncil, $36 for GPT-6 Astra, $5,323 for MerLean, $1,400 for Siege, and $2,127 API-equivalent for Humanize; the authors explicitly note that cost accounting differs by system [1, 3].

The benchmark’s important methodological choice is to score three distinct dimensions rather than collapse them into a single pass/fail number. Only 4/10 direct GPT-6 Astra solutions received adequate citations, compared with 7/10 for ProofCouncil; even ProofCouncil had negative average exposition scores on roughly a third of its responses. Referees also reported cases involving unsupported or nonexistent results, incorrect use of older references, and serious attribution failures [1]. These findings make it difficult to equate a plausible proof-shaped answer or even a correct core argument with a research-ready contribution.

Why the result matters. Batch 3 extends the first two First Proof evaluations by explicitly scoring exposition and attribution and by penalizing wrong answers, thereby making abstention or a clearly marked partial result preferable to a confident false proof. It also publishes a substantial audit trail: problems, human solutions, AI outputs, referee reports, system logs, and participating teams’ harness code [1, 2, 6, 7]. That transparency makes the benchmark useful not only as a leaderboard but as a corpus for studying failure modes.

What the comparison does not establish. This is a comparison of five complete systems, not a controlled experiment isolating base-model quality. The systems differ in model composition, use of web search, multi-agent orchestration, compute, and cost. The open-weight result is one Kimi K3-based system, self-hosted without web search; it cannot by itself establish a general open-weight/closed-model law. Ten selected problems are informative but too few to estimate broad mathematical research capability precisely. The problems were chosen to involve nonstandard insight and were screened against contemporary models, so the sample is not a random draw from mathematics [1].

The authors’ interpretation is appropriately narrower than a claim of autonomous discovery: the benchmark measures the ability to solve specified, already-human-solved problems and to present the results in a useful, attributable form. It does not measure open-ended conjecture formation, definition invention, or whether a system independently advances a research programme. Nor does a referee score constitute formal proof verification. The report is an author-produced benchmark paper with expert human assessment; its released materials enable independent scrutiny, but this report has not independently regraded the 50 system-problem outputs.

2. The Simons–Anthropic–OpenAI initiative: evaluation capacity becomes part of the research agenda

The 15 October announcement commits $15 million in combined funding and resources, with the Simons Foundation managing awards, including an open call for proposals. It is intended to help mathematicians evaluate recent AI-assisted results, learn and use tools, and shape community standards. OpenAI identifies $5 million as its own contribution and offers model and compute access for supported researchers [4, 5].

The significance is institutional: the field is investing in independent mathematical scrutiny and shared practice alongside model development. This could improve access to expert evaluation and lower barriers to examining AI-generated claims. However, the announcement does not yet establish the award criteria, independent review safeguards, or long-term outcomes. Because model developers are among the contributors, transparent governance, reviewer independence, disclosure of conflicts, and public reporting of evaluation methods will matter. Funding itself is not evidence that any mathematical claim is correct.

Assessment across both developments. The strongest near-term signal is not simply that a system can solve many research problems. It is that credible progress claims require multiple layers of evidence: correctness, intelligibility, attribution, reproducibility, and a clear statement of what the evaluation did not test. The First Proof materials make those dimensions inspectable; the new initiative may provide resources for broader scrutiny, but its impact remains to be observed.

References and Primary-Source Links

Primary sources below were checked for bibliographic identity and the specific facts attributed to them. Reported benchmark scores are attributed to the First Proof authors; no independent rerun or regrading is claimed.

[1] Abouzaid, M.; Srivastava, N.; Ward, R.; Williams, L. First Proof Third Batch. Hexagon preprint, v1, 14 October 2026 (CC BY 4.0). https://hexagonmath.org/2610.00244v1

[2] First Proof Project. Third Batch results and supplementary materials: problem statements, human solutions, AI solutions, referee reports, logs, and harness code. https://1stproof.org/third-batch.html

[3] First Proof Project. “Frontier AI Systems Solve up to 9/10 Problems in First Proof Benchmark; Open-Weight Entrant Solves None.” 14 October 2026. https://1stproof.org/third-batch-press-release.html

[4] Simons Foundation. “Simons Foundation Launches $15M Effort To Help Mathematicians Navigate AI Era.” 15 October 2026. https://www.simonsfoundation.org/news/simons-foundation-launches-15m-effort-to-help-mathematicians-navigate-ai-era/

[5] OpenAI. “Sharing AI progress in mathematics.” Original post 6 October 2026; update dated 15 October 2026. https://openai.com/index/sharing-ai-progress-in-mathematics/

[6] Abouzaid, M.; Blumberg, A. J.; Hairer, M.; et al. First Proof. arXiv:2602.05192, submitted 5 February 2026, revised 16 March 2026. https://arxiv.org/abs/2602.05192

[7] Abouzaid, M.; Srivastava, N.; Ward, R.; Williams, L. First Proof Second Batch. arXiv:2606.18119, submitted 16 June 2026. https://arxiv.org/abs/2606.18119

[8] Banerjee, A.; Bhattacharjee, A. “Failure Modes of Large Language Models on Research-Level Mathematics: A Taxonomy and an Empirical Characterisation.” arXiv:2606.24902, submitted 12 June 2026 (preprint). https://arxiv.org/abs/2606.24902

[9] Ravi, N. et al. “FormalProofBench: Can Models Write Graduate Level Math Proofs That Are Formally Verified?” arXiv:2603.26996, submitted 27 March 2026. https://arxiv.org/abs/2603.26996
