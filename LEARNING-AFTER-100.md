# Extra repository lessons after the 100-hour plan

Updated 2026-10-03. **Plan kind: personal-session-plan.** This file owns only the follow-on schedule, checks and progress. [LEARNING.md](LEARNING.md) owns the original 100-hour plan.

## Sequence and scope

Finish the 100-hour allocation in LEARNING.md first, including its final mocks and application-material sessions. The next `learn` invocation selects this file; an early request continues the base plan. Then use this separate **40-hour follow-on plan: 40 one-hour slots, or 2,400 minutes**. The combined allocation is 140 hours, with separate budgets and cursors. The original schedule and completion gates stay in LEARNING.md.

Continue the same document Q&A lab under `learning-artifacts/ai-engineering/`. Prioritize applications built with existing models for the agreed AI/ML/LLM/GenAI role interests. These additions give more practical evidence; completion does not guarantee a job or establish readiness for all model-training roles.

All assigned study material below is an existing lesson under `phases/`. Use named sections, checked-in reference implementations and learner-owned adaptations of those exercises. Current official API/library documentation supports the existing integrations; it adds no separate course. Keep the base plan's dependency exception, free-provider rules and protection of checked-in lesson code.

## Prior coursework and quick revision

The [official syllabus comparison](exa-results/iitm-syllabus-and-remaining-lessons-2026-10-03.md) records substantial overlap with the learner's completed Foundation courses, both Diplomas and degree core, plus the stated DLP, MLOps, App Dev Lab, LLM and GenAI study. Exact elective versions and the GenAI course code remain uncertain. Credit demonstrated concepts through quick checks rather than assigning those courses again.

| Prior study | Revision already in the base plan or assigned here |
|---|---|
| Foundation math/statistics/Python; diploma SQL/programming | Base-plan slots 1, 4-6 and 9, plus its conditional references. |
| MLF, MLT and MLP | Base-plan slot 9; follow-on slots 1-2 check preprocessing, leakage and evaluation. |
| Core DL and DLP | Follow-on slot 3 checks a small PyTorch/debugging case. |
| LLM and GenAI | Base-plan slot 6; follow-on slot 4 checks SFT masking and LoRA parameters. |
| MAD/App Dev, Software Engineering and Testing | Base-plan API/debug/test work; follow-on slots 21-24 check identity, configuration and clean startup. |
| MLOps | Base-plan slots 53 and 66-71; follow-on slots 25-31 apply metrics, load, cost and rollout lessons. |

R/F rows begin with an unhinted explanation and a practical changed case. Repair only the missed concept. A passed check releases the remaining work time for the review queue or independent practice. These checks credit the sampled concepts, not full lesson or course mastery. Check source prerequisites in the same way; repair a blocking gap before dependent work within this budget.

## Tutor contract for a fresh Codex session

When the learner asks to start or resume this follow-on plan:

1. Read this file's Resume state, last Progress log entry and Review queue. On first activation, read LEARNING.md's Resume state, final evidence and remaining gaps. Start follow-on teaching only after the base allocation's 100 slots are closed. While that allocation is open, resume its current task. Base-plan completion and follow-on completion are assessed separately.
2. Use the teaching, practical checks, quiz handling and evidence method in [LEARNING.md's tutor contract](LEARNING.md#tutor-contract-for-a-fresh-codex-session). This file owns the follow-on budget and repair policy. Load the current row's named lesson sections and learner files. Use one language, normally Python, and record unavailable runtimes or unsuccessful commands as gaps.
3. Give a worked example for new material, then require an independent learner change and changed-case check. Run the relevant finite reference demo and available deterministic tests where useful. Keep tutor-written code and fixture results identified in the evidence.
4. Fit each ordinary slot into 45 minutes of listed work, 10 minutes of relevant interview questions/quiz and 5 minutes of records. A repair slot uses up to 30 minutes repair, 25 minutes practice and 5 minutes records; adjust within the hour if a prerequisite blocks work. Retrieve available relevant stored quiz items without exposing keys before answers. If quiz.json is absent or has no relevant items, use the assigned interview prompt and independent changed-case check; record quiz as unavailable and the practical result separately. Record actual N/M only for answered stored items, and queue focused gaps below 70%.
5. In the last five minutes, update this file's Resume state, Progress log and Review queue with minutes, slot/work IDs, check/quiz result, learner artifact, exact command/result, live or fixture mode, remaining action and displaced work. Keep the base plan's cursor and elapsed minutes as its historical record.

An interrupted hour stays `in_progress` and resumes with its unused allowance. Closing an hour closes the time slot, not the task's mastery. A deliberately closed short hour records unused minutes as forfeited. Use `passed`, `partial`, `deferred` or `cut` for task outcomes.

## Repair policy and budget

Recall/repair slots are 12, 20, 28 and 36. Slots 1-4 are focused prior-course checks. If the queue is empty, use a recall slot for an independent changed case or the next scheduled task, and record its work ID so the later row provides further practice or repairs another gap.

At activation, copy unresolved base-plan gaps that block these lessons into this file's Review queue. Fix them within the follow-on allowance before dependent work. Keep the original gaps visible in the base plan's record; new evidence can cross-reference their resolution.

If work runs long, preserve its pending action and reallocate within these 40 slots. Reduce optional query-transformation or rollout breadth, then redundant passed revision and less relevant breadth. Preserve the four recall slots and prioritize validation, access checks, measured retrieval, actual restart recovery and finite MCP exchanges. Mark displaced work deferred/cut; a deferred completion requirement stays a gap.

After a gap of at least seven calendar days, use up to 10-15 minutes of the open or next slot for recall and a practical re-entry check. Missed days consume no study time. After slot 40, report passed gates and remaining gaps. Further study needs an agreed new budget.

## Budget and numbered schedule

| Work block | Hours including drills/notes |
|---|---:|
| Focused prior-course revision checks | 4 |
| Advanced retrieval in the same lab | 7 |
| Durable execution and recovery | 7 |
| Service identity and measured operation | 10 |
| Local MCP integration | 8 |
| Spaced recall and repair | 4 |
| Total | 40 |

S = study/practice; R = conditional revision; F = focused introduction. Each numbered row below is a follow-on hour. Follow-on slot 1 comes after the base plan's slot 100. Rows are budget allocations, not promises of full-lesson completion in an hour.

### Prior-course practical revision

Use the focused exercises below to verify prior coursework. Check relevant prerequisite concepts rather than assigning the full Phase 2, 3 or 10 chains. Use stdlib/NumPy or the allowlisted PyTorch; the existing learner-copy framework exception stays as listed above. The examples in lesson prose that use other packages stay reference-only.

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 1 | R, selected sections: 02.08 [Feature Engineering](phases/02-ml-fundamentals/08-feature-engineering/docs/en.md)<br>02.13 [ML Pipelines](phases/02-ml-fundamentals/13-ml-pipelines/docs/en.md) | Without hints, explain a preprocessing leakage case and make one changed-case fix using scratch/NumPy transforms fitted only on training data. Check an unseen category or missing value. Credit the sampled pipeline skills, then use remaining work time on the current queue. | Q38,C17 |
| 2 | R, selected sections: 02.09 [Model Evaluation](phases/02-ml-fundamentals/09-model-evaluation/docs/en.md) | Evaluate a changed imbalanced prediction set and justify its split/metric. Use the available Python evaluation functions or a tiny learner check; this lesson has no Python main.py. Explain one misleading accuracy result. Repair only the missing concept. | Q37-Q39,C17 |
| 3 | R, selected exercises: 03.11 [Introduction to PyTorch](phases/03-deep-learning-core/11-intro-to-pytorch/docs/en.md)<br>03.13 [Debugging Neural Networks](phases/03-deep-learning-core/13-debugging-neural-networks/docs/en.md) | Trace one training step and diagnose a gradient, shape or train/eval-mode failure without a supplied solution. Use a tiny deterministic example or cached data to fit the slot. Save the independent fix and check; a missing runtime remains a visible gap. | Q40,Q61,C17 |
| 4 | R, selected sections: 10.06 [Instruction Tuning](phases/10-llms-from-scratch/06-instruction-tuning-sft/docs/en.md)<br>11.08 [Fine-Tuning with LoRA](phases/11-llm-engineering/08-fine-tuning-lora/docs/en.md) | Check assistant-token loss masking and a small LoRA shape/frozen-weight example. If prior fine-tuning work is available, explain and change a relevant part. Otherwise use the repo toy example and record its limits; full pretrained-model training is not assigned. | Q15,Q62 |

### Advanced retrieval in the same lab

Build on base-plan slots 25-41 and 19.68's metric functions. Base-plan slot 38 was only an optional introduction. Keep T cases fixed for comparisons; inspected H cases remain exploratory. If new held-out claims are needed, freeze new question/source labels before looking at outputs, within these slots.

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 5 | S: 11.07 [Advanced RAG](phases/11-llm-engineering/07-advanced-rag/docs/en.md) | Inspect the BM25, RRF, lexical reranker and templated HyDE reference. Select the relevant sections and freeze a baseline on the lab's existing query IDs, versions and evidence labels. Record which reference paths are substitutes. | Q20-Q22 |
| 6 | S: 11.07 [Advanced RAG](phases/11-llm-engineering/07-advanced-rag/docs/en.md) | Apply BM25 to the existing chunks with stable IDs. Independently test an exact identifier, a paraphrase and an empty query. Reuse the learned-vector path and record the different evidence retrieved by each method. | Q20,C12 |
| 7 | S: 11.07 [Advanced RAG](phases/11-llm-engineering/07-advanced-rag/docs/en.md) | Implement reciprocal-rank fusion over BM25 and learned-vector rankings. Handle repeated candidate IDs and a missing branch. Compare the fused list with both baselines on unchanged T cases; avoid adding raw scores on incompatible scales. | Q56,C12 |
| 8 | S: 11.07 [Advanced RAG](phases/11-llm-engineering/07-advanced-rag/docs/en.md) | Apply the reference lexical reranker to a bounded candidate set. Save one difficult distractor and a changed case. Measure ranking and latency effects; label the method a heuristic, with no learned cross-encoder claim. | Q21-Q22,C12 |
| 9 | S: 11.07 [Advanced RAG](phases/11-llm-engineering/07-advanced-rag/docs/en.md)<br>11.06 [RAG](phases/11-llm-engineering/06-rag/docs/en.md) | Try one bounded query rewrite or HyDE-style retrieval query using the existing provider adapter if free quota permits. Compare with the original query on fixed cases. Generated text stays a search aid, never cited evidence; label templated/replayed paths separately. | Q16,Q20 |
| 10 | S, selected metric functions: 11.07 [Advanced RAG](phases/11-llm-engineering/07-advanced-rag/docs/en.md)<br>19.68 [RAG Evaluation Metrics](phases/19-capstone-projects/68-rag-eval-precision-recall/docs/en.md) | Score the unchanged retrieval cases with P@k, R@k, MRR and a small nDCG changed-list exercise. Keep retrieval ranking, answer support and answer relevance separate. Save per-case results and explain one ranking tradeoff. | Q22,Q55-Q56,C11-C12 |
| 11 | S: 11.07 [Advanced RAG](phases/11-llm-engineering/07-advanced-rag/docs/en.md)<br>11.10 [Evaluation and Testing](phases/11-llm-engineering/10-evaluation/docs/en.md) | Choose the simplest measured retrieval path for the lab. Run it through answer validation and scope checks; preserve a failure and a changed-case regression. Report an unchanged or worse outcome as observed, rather than requiring an improvement. | Q44,Q47,C12 |
| 12 | Recall/repair; current Review queue and earlier assigned rows | Retrieve a previously learned concept without hints, repair the missed part and retest with a changed case. Use an empty queue for independent practice or the next scheduled task; record the work ID and reused time. | Current gaps and assigned quizzes |

### Durable execution and recovery

Keep the agent read-only. Persist workflow state and recorded model/tool results; use a local fake destination for the side-effect/idempotency exercise. The destination's state must survive as well as the checkpoint. These are bounded lesson adaptations, not a distributed workflow-service project.

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 13 | F/S, selected prerequisites: 15.01 [Long-Horizon Agents](phases/15-autonomous-systems/01-long-horizon-agents/docs/en.md)<br>15.10 [Permission Modes](phases/15-autonomous-systems/10-claude-code-permission-modes/docs/en.md)<br>15.12 [Durable Execution](phases/15-autonomous-systems/12-durable-execution/docs/en.md) | Check existing stop/permission concepts, then separate deterministic orchestration from model/tool activities. Identify a stable run ID, caller scope and configuration version. Assign only the long-run and permission sections needed for recovery. | Q26-Q27,Q57 |
| 14 | S: 15.12 [Durable Execution](phases/15-autonomous-systems/12-durable-execution/docs/en.md) | Run the finite event-log reference and inspect its replay key and pretend activities. Connect a small learner workflow to recorded results, including source/prompt/model versions and scope; reject replay under a mismatched configuration. | Q27,Q57 |
| 15 | S: 15.12 [Durable Execution](phases/15-autonomous-systems/12-durable-execution/docs/en.md)<br>15.16 [Checkpoints and Rollback](phases/15-autonomous-systems/16-checkpoints-rollback/docs/en.md) | Persist workflow progress and result records in a stable learner file or SQLite database. Use the atomic-checkpoint sections. Test a partial/corrupt record and keep keys/private text out of saved state. This row builds on existing SQL knowledge. | Q10,Q57,C13 |
| 16 | S: 15.12 [Durable Execution](phases/15-autonomous-systems/12-durable-execution/docs/en.md) | Force a stop after a completed step, then invoke a second Python process using the same state path. Demonstrate resume and reuse of the saved result without repeating the completed activity. An exception caught in one process is insufficient evidence. | Q27,Q57,C13 |
| 17 | F/S, selected prerequisite sections: 15.15 [Propose-Then-Commit](phases/15-autonomous-systems/15-propose-then-commit/docs/en.md)<br>15.16 [Checkpoints and Rollback](phases/15-autonomous-systems/16-checkpoints-rollback/docs/en.md) | Trace propose, verify and rollback with a synthetic local action. Define the precondition and destination verification before committing. Read only the approval concepts needed by 15.16; external or paid side effects are not assigned. | Q25-Q26,Q57 |
| 18 | S: 15.16 [Checkpoints and Rollback](phases/15-autonomous-systems/16-checkpoints-rollback/docs/en.md) | Explain the reference's gap between recording committed and executing its in-memory side effect. Persist the fake effect and unique idempotency key in one SQLite transaction. Stop after checkpoint intent but before the destination transaction, and after that transaction but before the final checkpoint update. Retry in a fresh process; consult the destination record to apply or skip, rather than trusting the checkpoint's committed label. | Q10,Q57,C13 |
| 19 | S: 15.12 [Durable Execution](phases/15-autonomous-systems/12-durable-execution/docs/en.md)<br>15.16 [Checkpoints and Rollback](phases/15-autonomous-systems/16-checkpoints-rollback/docs/en.md) | Run a recovery suite for completed-step replay, duplicate retry, invalid version/scope and failed verification. Show that checkpoint and fake destination agree after restart. Save a bounded recovery demo and its limits; no cross-service exactly-once guarantee is implied. | Q42,Q45,Q57,C13 |
| 20 | Recall/repair; current Review queue and earlier assigned rows | Retrieve a previously learned concept without hints, repair the missed part and retest with a changed case. Use an empty queue for independent practice or the next scheduled task; record the work ID and reused time. | Current gaps and assigned quizzes |

### Service identity and measured operation

Reuse the existing local service, provider adapter and evaluation cases. Check retained MAD/App Dev/MLOps concepts before reading the selected sections. Relevant inference, caching and rollout prerequisites can be credited through those checks; full GPU autoscaling, gateway or A/B-platform routes are not assigned. Public deployment is conditional on an existing permitted free environment and its access requirements.

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 21 | R/F, selected sections: 11.13 [Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>17.25 [Security and Secrets](phases/17-infrastructure-and-production/25-security-secrets-audit/docs/en.md) | Check authentication versus authorization, then define two server-side development principals with document scopes. Specify how a validated credential chooses the principal. Ignore caller-supplied user_id/scope as proof of identity; this is a bounded local prototype. | Q5,Q23,Q58,C14 |
| 22 | S, lesson adaptation: 11.13 [Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>17.25 [Security and Secrets](phases/17-infrastructure-and-production/25-security-secrets-audit/docs/en.md) | Add environment-configured opaque development credentials and server-side scope lookup before retrieval/cache/model calls. Check valid, missing, invalid, expired/revoked and wrong-scope cases. Save redacted results; this does not establish a production identity-provider integration. | Q23,Q51,Q58,C14 |
| 23 | R/S, selected sections: 17.25 [Security and Secrets](phases/17-infrastructure-and-production/25-security-secrets-audit/docs/en.md)<br>17.13 [LLM Observability](phases/17-infrastructure-and-production/13-llm-observability/docs/en.md) | Trace allowed and denied requests through the actual service. Check that development credentials, provider keys and private evidence are absent from errors/logs/fixtures. Demonstrate safe configuration failure and server-derived scope in the cache key. | Q32,Q35,Q58,C14 |
| 24 | R/S, selected packaging sections: 00.07 [Docker for AI](phases/00-setup-and-tooling/07-docker-for-ai/docs/en.md)<br>11.13 [Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Start the service from a clean process with recorded dependencies/config, health check and shutdown command. Package it in Docker if available; otherwise save the runtime blocker and verify the existing Python environment. Local packaging remains distinct from public deployment. | Q33,Q45 |
| 25 | F/S, metric and workload sections: 17.08 [Inference Metrics](phases/17-infrastructure-and-production/08-inference-metrics-goodput/docs/en.md)<br>17.22 [Load Testing LLM APIs](phases/17-infrastructure-and-production/22-load-testing-llm-apis/docs/en.md) | Measure a bounded mix of actual local requests with cold/warm retrieval/cache and limited concurrency. Label fixture-provider and live-call runs separately; use a small live sample only within free quota. Report available latency/errors and leave unmeasured token-stream metrics blank. | Q4,Q31,Q59,C16 |
| 26 | F/S, selected attribution sections: 17.27 [FinOps for LLMs](phases/17-infrastructure-and-production/27-finops-llms/docs/en.md) | Record per-principal/run/route call and token counts where supplied, with dated model/pricing metadata only when verified. Compare per-answer resource use and apply a small local call budget. Mark unavailable costs unknown; a free bill is not evidence of free unlimited traffic. | Q26,Q31,Q59,C16 |
| 27 | S, selected monitoring sections: 17.13 [LLM Observability](phases/17-infrastructure-and-production/13-llm-observability/docs/en.md)<br>11.10 [Evaluation and Testing](phases/11-llm-engineering/10-evaluation/docs/en.md) | Connect the actual trace IDs and configuration versions to saved case outcomes. Diagnose a failed answer across retrieval, provider and validation, then rerun a changed case. Use existing tuning/held-out labels honestly and keep simulated dashboards labeled. | Q22,Q35,Q46,C16 |
| 28 | Recall/repair; current Review queue and earlier assigned rows | Retrieve a previously learned concept without hints, repair the missed part and retest with a changed case. Use an empty queue for independent practice or the next scheduled task; record the work ID and reused time. | Current gaps and assigned quizzes |
| 29 | F/S, local rollout sections: 17.20 [Shadow, Canary and Progressive Deployment](phases/17-infrastructure-and-production/20-shadow-canary-progressive/docs/en.md)<br>11.13 [Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Version a small prompt/retrieval/config change with predeclared quality/error/latency criteria. Apply and roll back locally against unchanged T cases. Measure the actual lab path; the seeded canary simulator does not prove a public rollout. | Q36,Q44,C16 |
| 30 | S, selected deployment sections: 11.13 [Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>00.07 [Docker for AI](phases/00-setup-and-tooling/07-docker-for-ai/docs/en.md) | Prepare and smoke-test the lesson's service configuration and access checks. If an existing permitted free hosting environment is available, verify a deployed request, secrets/config, transport security and cleanup; otherwise record the blocker and perform the clean local smoke test. Do not enable billing. | Q33,Q45,Q58 |
| 31 | S: 11.13 [Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>17.25 [Security and Secrets](phases/17-infrastructure-and-production/25-security-secrets-audit/docs/en.md)<br>11.10 [Evaluation and Testing](phases/11-llm-engineering/10-evaluation/docs/en.md) | Run the client-to-service path with server-verified principal scope, a supported answer, abstention and denied/error cases. Include persisted recovery and measured-operation evidence in a short runbook. Record deployment/auth/recovery limits beside the exact commands. | Q41,Q45,Q57-Q59,C13-C16 |

### Local MCP integration

Use the existing document lookup and caller-scope policy. This is an eight-hour block in this follow-on plan. It uses the same lab and the assigned MCP lesson sections. Review the relevant tool-interface/function/schema concepts from 13.01-05 through the existing tool and validator; repair only failed prerequisites. Keep all transports local, with no remote MCP/OAuth service assigned.

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 32 | F/S, selected prerequisites: 13.05 [Tool Schema Design](phases/13-tools-and-protocols/05-tool-schema-design/docs/en.md)<br>13.06 [MCP Fundamentals](phases/13-tools-and-protocols/06-mcp-fundamentals/docs/en.md) | Check the existing tool schema/arguments/permission boundary, then trace JSON-RPC correlation, discovery and tool calls in 13.06. Follow the repository lesson's protocol/version contract. Self-reported client metadata does not authenticate a caller. | Q25,Q60 |
| 33 | S: 13.07 [Building an MCP Server](phases/13-tools-and-protocols/07-building-an-mcp-server/docs/en.md) | Run the finite server --demo and available deterministic tests, then map the existing read-only lookup to its tool contract in the learner copy. Keep JSON protocol output separate from diagnostics. Inspect the schema and response envelope. | Q25,Q60 |
| 34 | S: 13.07 [Building an MCP Server](phases/13-tools-and-protocols/07-building-an-mcp-server/docs/en.md)<br>13.05 [Tool Schema Design](phases/13-tools-and-protocols/05-tool-schema-design/docs/en.md) | Independently check malformed arguments, unknown tool, restricted document and empty evidence at the server boundary. Authorize in server code before the lookup. Metadata/annotations remain hints and cannot grant a document scope. | Q23,Q25,Q60,C15 |
| 35 | S: 13.08 [Building an MCP Client](phases/13-tools-and-protocols/08-building-an-mcp-client/docs/en.md) | Run the reference client and explain its in-process peer calls. Build the learner's discovery/routing adapter over the same lookup contract with explicit request IDs, versions and safe errors. Save one changed tool/schema case. | Q24,Q60,C15 |
| 36 | Recall/repair; current Review queue and earlier assigned rows | Retrieve a previously learned concept without hints, repair the missed part and retest with a changed case. Use an empty queue for independent practice or the next scheduled task; record the work ID and reused time. | Current gaps and assigned quizzes |
| 37 | S, transport adaptation: 13.07 [Building an MCP Server](phases/13-tools-and-protocols/07-building-an-mcp-server/docs/en.md)<br>13.08 [Building an MCP Client](phases/13-tools-and-protocols/08-building-an-mcp-client/docs/en.md)<br>13.09 [MCP Transports](phases/13-tools-and-protocols/09-mcp-transports/docs/en.md) | Use stdlib subprocess.Popen for the learner's stdio server peer. Exchange newline-delimited JSON-RPC on stdin/stdout with bounded timeout, separate stderr and clean termination. Save a successful discovery/lookup exchange across processes. | Q7,Q60,C15 |
| 38 | S: 13.09 [MCP Transports](phases/13-tools-and-protocols/09-mcp-transports/docs/en.md) | Run the lesson's finite loopback Streamable HTTP probe and use the transport contract with the learner lookup. Compare the stdio and local HTTP paths on the same case. Preserve the configured server principal boundary; public exposure/OAuth is outside this block. | Q5,Q23,Q60,C15 |
| 39 | S: 13.07 [Building an MCP Server](phases/13-tools-and-protocols/07-building-an-mcp-server/docs/en.md)<br>13.08 [Building an MCP Client](phases/13-tools-and-protocols/08-building-an-mcp-client/docs/en.md)<br>13.09 [MCP Transports](phases/13-tools-and-protocols/09-mcp-transports/docs/en.md) | Test malformed/unsupported requests, denied lookup, timeout and peer shutdown without a live provider. Prove that errors reach the caller and the child process/HTTP server stops. Explain where a caller is trusted or credential-verified. | Q3,Q7,Q58,Q60,C15 |
| 40 | S: 13.06 [MCP Fundamentals](phases/13-tools-and-protocols/06-mcp-fundamentals/docs/en.md)<br>13.09 [MCP Transports](phases/13-tools-and-protocols/09-mcp-transports/docs/en.md)<br>11.10 [Evaluation and Testing](phases/11-llm-engineering/10-evaluation/docs/en.md) | Demonstrate one read-only lookup through MCP and the existing Q&A path. Compare with direct lookup on unchanged cases and record transport overhead/provider mode. Keep the simpler default if appropriate. Save finite integration evidence and update the lab's evidence summary with passed checks, remaining gaps and exact commands. | Q24,Q42,Q47,Q60,C15 |

## Follow-on interview and coding practice

Use these IDs within the rows' allotted drill time. Existing Q1-Q55 are in [the base interview bank](LEARNING.md#interview-practice-bank), and C1-C11 are in [the base coding bank](LEARNING.md#coding-and-sql-practice). The new IDs continue that numbering without changing either base bank. This plan's slot numbers remain 1-40.

| ID | Topic | Prompt | What a useful answer covers |
|---|---|---|---|
| Q56 | Advanced retrieval | How would you combine keyword and vector rankings with reciprocal-rank fusion? | Rank positions rather than incompatible raw scores, stable document IDs, deduplication, a missing branch, and comparison on fixed gold evidence. |
| Q57 | Recovery | What survives a process crash, and how do you avoid repeating a completed action? | Persisted workflow and destination state, replay keys including scope/version, transactional idempotency for the local fake effect, fresh-process evidence, and the remaining distributed crash windows. |
| Q58 | Service identity | Which part of a request proves caller identity, and where is document scope decided? | Server-verified credential-to-principal lookup before retrieval/cache/model calls; caller-supplied IDs and MCP metadata are not proof. Explain the development verifier's limits and safe denied responses. |
| Q59 | Service operation | What does your load/cost report measure, and what remains unknown? | Actual request path, workload and concurrency, fixture versus live modes, available latency/token fields, unknown streaming/billing fields, dated rates when used, and small-sample/free-quota limits. |
| Q60 | MCP | How do discovery, routing and transport change a direct document lookup? | Repository protocol/version contract, JSON-RPC correlation, tool schema and server authorization, stdio or loopback HTTP framing, timeout/cleanup, and actual process evidence versus an in-process peer. |
| Q61 | Prior DL revision | How would you diagnose a training loop that stops learning or changes validation results unexpectedly? | Data/shape checks, loss and gradients, optimizer update, train/eval mode, leakage, a small reproduced failure and an independent changed-case fix. |
| Q62 | Prior fine-tuning revision | Which tokens and parameters are trained in the SFT/LoRA example? | Assistant-token masking, frozen base weights, adapter dimensions and parameter count, gradients, and a clear distinction between the toy example and past pretrained-model work. |

| Task | What to implement or explain | Relevant scheduled material |
|---|---|---|
| C12 | Merge two ranked document lists with RRF and independently score the result on fixed evidence labels; handle duplicate IDs and a missing branch. | 11.07 Advanced RAG and the existing evaluation set |
| C13 | Persist a small workflow and a local fake destination, stop after checkpoint intent and after the destination transaction, then retry in a fresh process using the destination's unique idempotency record. Verify completion plus idempotency records agree and scope/version changes reject replay. | 15.12 Durable Execution and 15.16 Checkpoints and Rollback |
| C14 | Verify an environment-configured development credential, derive document scope server-side and reject an attempted caller-ID override before retrieval/cache/provider work. Include an invalid/expired or denied case with safe errors. | 11.13 service boundary and 17.25 selected security sections |
| C15 | Exchange one successful and one invalid/denied MCP tool call with a subprocess peer or loopback HTTP server. Bound the timeout and demonstrate protocol output, diagnostics and process cleanup. | 13.06-13.09 local MCP block |
| C16 | Aggregate actual local latency/error/resource counts by run and principal, retain provider mode, and explain missing or simulated fields. Compare a configuration change on unchanged cases and demonstrate rollback. | Selected Phase 17 metrics/load/FinOps and existing evaluation lessons |
| C17 | Fix one changed ML/DL case involving train-only preprocessing, imbalanced evaluation, a missing gradient or train/eval mode. Explain the failure and verify the fix without a full course repeat. | Prior-course revision excerpts in follow-on slots 1-3 |

The original 100-hour plan already includes its timed mocks. These follow-on rows add short checks and changed cases within their 60 minutes. Use the base mock rubric only as a personal repair signal if a recall slot includes a mock-style exercise.

## Reference lab limitations

These limits describe the checked-in runners. Record separate learner runs before claiming the assigned practical experience.

| Lesson | Limitation and follow-on evidence |
|---|---|
| 11.07 Advanced RAG | The reference vectors use TF-IDF, reranking is lexical and HyDE is templated. Slots 5-11 reuse learned vectors and label real query transformations versus substitutes. A learned cross-encoder is not assigned. |
| 02.09 Model Evaluation | The metadata says Python, but its main runner is Julia. Slot 2 uses available Python functions or a tiny learner check rather than requiring a Python main.py. |
| 03.11/03.13 DL revision; 10.06/11.08 SFT/LoRA | Selected small exercises check retained concepts. They do not establish a new pretrained-model training run or full course mastery. |
| 15.12/15.16 Recovery | The reference has JSON logs/file checkpoints with pretend activities and in-memory destination state. A checkpoint can say committed before the action occurs. Slots 15-19 persist the fake destination and test separate-process retry at both checkpoint/destination crash windows. |
| 11.13 Production Application | The reference pipeline is simulated. Slots 21-31 extend the actual learner service; a local development credential verifier remains a prototype identity boundary. |
| 17.08/17.13/17.20/17.22/17.27 Operation | Reference metrics, traces, rollout, load and cost data are synthetic. Slots 25-31 collect actual local data and label provider mode, unknown streaming fields and unavailable billing data. |
| 17.25 Security | Scrubbing/audit examples do not implement user authentication or a production secret store. Slots 21-23 require a server-verified development principal and safe denied cases. |
| 13.07/13.08/13.09 MCP | The finite server demo and reference client include in-process calls. Slots 37-40 require actual subprocess stdio and a loopback HTTP exercise, with timeout and cleanup. Self-reported client metadata is not identity proof. |
| 19.68 RAG Metrics | Metric functions are deterministic math; the supplied pipeline and token-overlap judge use fixtures/heuristics. Use learner qrels and human-reviewed support/relevance for claims about actual outputs. |

Full pretrained fine-tuning, remote MCP/OAuth, large-model self-hosting and broader cloud study remain outside this follow-on allocation. Public deployment is conditional on an existing permitted free environment in slot 30. If unavailable, keep the blocker and local smoke evidence; public deployment stays unproven.

## Completion checks

Assess these against saved learner evidence after the 40-hour allocation. Time spent alone does not pass them.

- Record the four prior-course checks as passed, partial, deferred or repaired, and demonstrate an independent changed case for the sampled concepts.
- Compare BM25, learned-vector retrieval and fusion on unchanged evidence labels; document the reranking/query-transformation path actually tried and its limits. Keep retrieval quality, answer support and relevance separate, and preserve a failed case with a learner-explained repair.
- Resume the workflow in a fresh process. For the persisted fake destination, test a stop after checkpoint intent but before the destination transaction, and after the destination transaction but before the final checkpoint update. Use the destination's unique idempotency record on retry, verify final state and reject incompatible scope/configuration replay.
- Demonstrate server-verified development credentials and scope before retrieval/cache/provider calls, including caller-ID override, denied/error and secret-redaction checks. State what the local verifier establishes.
- Retain actual local request measurements with workload/concurrency and provider-mode labels, a quality-case diagnosis, a configuration rollback and clean-process commands. Record public-host evidence or its conditional blocker.
- Save finite MCP discovery/tool exchanges through subprocess stdio and loopback HTTP, including invalid/denied cases, timeout and cleanup. Compare the lookup with the direct path using the same cases.
- Update the continuing lab's README/demo and any resume claim with observed evidence, learner contributions, AI assistance and remaining gaps. Prototype authentication, a local fake destination and bounded request tests do not establish enterprise identity, cross-service exactly-once behavior or production scale.

Use the final five-minute record in slot 40 to summarize these gates. A cut/deferred requirement prevents a claim of full follow-on completion; it does not erase the original plan's separate result.

## Resume state

This cursor belongs to the follow-on allocation. The `learn` skill activates it on the next invocation after the original 100 slots close. Until then, retain the waiting state and resume the base cursor.

| Field | Current value |
|---|---|
| Activation | waiting_for_base_100_hours |
| Current slot | 1 / 40 |
| Slot status | not_started |
| Minutes used in current slot | 0 / 60 |
| Closed slots | 0 / 40 |
| Total study minutes used | 0 / 2400 |
| Forfeited minutes in closed short slots | 0 |
| Last study date | None recorded |
| Current task | Wait for the base plan's 100 slots to close |
| Pending next action | Review base-plan evidence and blocking gaps, then begin follow-on slot 1's unhinted preprocessing check |
| Learner artifact directory | learning-artifacts/ai-engineering/ (continue the existing lab) |
| Last runnable evidence | None recorded for this follow-on plan |
| Displaced work | None |

On activation, set Activation to `active` and Current task to the first pending check. On closing an hour, increment Closed slots, advance Current slot and reset open-slot minutes to 0. Total used plus forfeited minutes equals 60 times closed slots plus minutes used in the open slot. After closing slot 40, set Current slot and Activation to `budget_exhausted`, with open-slot minutes 0; report completion checks and remaining gaps.

## Progress log

Append continuation entries for interrupted slots; sum their minutes within the same hour. Planning a task does not complete it.

| Date | Follow-on slot / work IDs | Minutes this entry / slot state | Task outcome and check / quiz N/M | Learner artifact / command / result / provider mode | Pending action / displaced work |
|---|---|---|---|---|---|

## Review queue

| Lesson / question / gate | Specific gap and prerequisite it blocks | Changed-case retest | Allocated repair slot or displaced row | Status |
|---|---|---|---|---|
