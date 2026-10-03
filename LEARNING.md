# My 100-hour junior AI engineering learning plan

Updated 2026-10-03. **Plan kind: personal-session-plan.** This file owns the schedule, tutor instructions and progress.

## Target and agreed scope

Prepare for paid internships/trainee roles and junior LLM application jobs in India, including onsite/hybrid and India-eligible global remote work. The goal is to implement, explain and debug a small feature under guidance. Country, degree, enrollment and experience eligibility still need a check when applying.

The budget is **100 one-hour learning slots, or 6,000 minutes**. There is no fixed completion date. Lessons, revisions, quizzes, mocks, feedback, repairs and two hours of application materials fit inside it. A missed calendar day consumes no slot. Opening a fresh Codex chat does not start the next hour automatically.

Credit IITM BS coursework, DLP, MLOps, App Dev Lab, LLM and Gen AI through small unhinted checks. Learn unfamiliar topics through a worked example first, then an independent changed case. Tessera, DSA, AWS exam preparation, system design and remaining degree work stay separate. Use one repository-derived document Q&A lab; no additional portfolio project is assigned.

## Research and priorities

The [full curriculum comparison](exa-results/learning-plan-curriculum-review-2026-10-03.md) records dispositions for all 523 phase lessons and 67 certification lessons. This review added focused outcome/specification, attention, metric-setting and secrets checks inside existing slots, and replaced the optional reranker survey with a RAG metric exercise. These are assigned sections and practical checks, not six extra full lessons.

The [Exa market review](exa-results/learning-plan-market-review-2026-10-02.md) retains 17 distinct employer descriptions for comparison and separates archived, restricted and uncertain sources. It distinguishes required qualifications, duties and preferences. This is a selected LLM-role sample, not market-wide prevalence or a promise that those vacancies are open.

In its 11-description junior cohort, Python appears in required qualifications or duties in 9/11; API/backend integration in 8/11; prompting/structured outputs in 9/11; RAG in 8/11; evaluation/testing in 9/11; and LLM frameworks in 6/11. Explicit hosted LLM API integration appears in 4/11, rather than being inferred from general LLM familiarity. These counts overlap. The fresher cohort has overlapping employers and is not added to these totals. Sources and coding details are in the linked review.

My inference is to prioritize a connected application with evidence-grounded answers, tested boundaries and repeatable evaluation. Framework practice belongs in the route because some sampled jobs require it. For example, [Anteriad](https://job-boards.greenhouse.io/anteriad/jobs/5386350004) names LangChain/LangGraph and FastAPI/Flask; [Mobio](https://mobiosolutions.freshteam.com/jobs/8O8aIBiTdyF-/generative-ai-engineer) asks for framework experience. [RevRag](https://www.revrag.ai/careers/ai-engineer-intern) assigns response testing and treats vectors/cloud as preferences; those labels differ by employer.

| Priority | Included work |
|---|---|
| Common preparation | Python/SQL/Git checks, HTTP/JSON, real model calls, prompts and schemas, ingestion/chunking/retrieval, citations/abstention, evaluation, debugging and safe error/access handling. |
| Job-stack exposure | Scratch concepts followed by two sessions each for Chroma, FastAPI/Uvicorn, LangChain LCEL and LangGraph. Basic configuration, logs, local packaging and CI checks. |
| Extras or references | Hybrid retrieval and local rollback are cuttable introductions; the full reranker lab stays a reference. Public deployment, deeper MCP, broad vendor surveys, fine-tuning/self-hosting, durable agents and advanced cloud infrastructure are outside required completion. |

Global remote means the employer can hire an India-based applicant. The research did not verify an explicitly worldwide junior opening; that limits this sample, not the whole market. Unpaid descriptions are supplementary skill evidence, not the agreed job target.

## One continuing lab and free access

Keep learner-owned work under `learning-artifacts/ai-engineering/`. Begin with 8-12 tiny public or synthetic documents and a few questions. Grow one path: ingestion -> retrieval -> real model -> answer/citations/abstention -> validation -> evaluation -> local API. Add a bounded read-only agent for comparison later. Preserve checked-in reference code.

The learner has approved a narrow dependency exception for this personal lab: `chromadb`, `fastapi`, `uvicorn`, `langchain-core` and `langgraph`, plus their required dependencies. Use an isolated Python environment, record working versions, and consult current official documentation before each library session. This exception does not change the curriculum dependency policy. Use stdlib clients and unittest checks; no extra provider SDK, framework survey, hosted vector service or paid account is required.

Google's documentation lists free generation and embeddings (pricing rechecked 2026-10-03), with India access checked in the market review. Verify available free models, account access and quotas in slot 2 and again before embedding practice. Use the raw HTTP pattern in 00.04 adapted to the current API; its whole SDK-first script is not the assigned runner. The [generation REST example](https://ai.google.dev/gemini-api/docs/text-generation) currently uses `POST /v1beta/interactions`, an API-key header and model/input fields. The [embedding REST example](https://ai.google.dev/gemini-api/docs/embeddings) uses `embedContent`; embed each document separately and verify task formatting. Confirm both against current docs before coding. The live gate needs an HTTP success, a parsed nonempty text response or finite vector as appropriate, and the dated model ID; a status code alone is insufficient. [Pricing](https://ai.google.dev/gemini-api/docs/pricing), [regions](https://ai.google.dev/gemini-api/docs/available-regions), [rate limits](https://ai.google.dev/gemini-api/docs/rate-limits).

Use public/synthetic data because the free-tier pricing page allows submitted content to improve products. Keep keys in the local environment and out of replies, logs and tracked files. Cache successful embeddings/outputs to reduce calls. A saved fixture is useful for deterministic checks; it does not prove a successful live request. If free access is blocked, record the blocker and do independent work within the next slot. Recheck another genuinely free option using official documentation. Keep the live-call gates pending and do not enable billing as a fallback.

Library work stays small: Chroma receives precomputed embeddings with `embedding_function=None`; LCEL wraps existing callables with `RunnableLambda`; LangGraph uses a bounded `StateGraph`. The API runs on `127.0.0.1` and a trusted synthetic caller scope. External authentication, public hosting and process-restart recovery for agents are not established by these exercises.

Current implementation references: [FastAPI request bodies](https://fastapi.tiangolo.com/tutorial/body/), [Uvicorn settings](https://uvicorn.dev/settings), [RunnableLambda](https://reference.langchain.com/python/langchain-core/runnables/base/RunnableLambda), [LangGraph graph API](https://docs.langchain.com/oss/python/langgraph/graph-api), [Chroma collections](https://docs.trychroma.com/docs/collections/manage-collections) and [caller-provided embeddings](https://docs.trychroma.com/docs/collections/add-data).

## Tutor contract for a fresh Codex session

When the learner asks to start or resume this plan, follow these steps. This contract takes precedence over the generic phase-selection, warm-up and completion rules in `skills/learn/SKILL.md` for this plan only.

1. Read Resume state, the last Progress log entry and the Review queue. If a newer log entry conflicts with the cursor, reconcile the state from its recorded slot, minutes and evidence before teaching; missing evidence stays pending. Load the current row's lesson sections and relevant learner files, not the whole curriculum. Resume its pending action and remaining minutes. A new chat or a calendar gap does not advance the cursor.
2. For a previously learned prerequisite, ask one short explanation and one small practical/changed-case check without hints. Credit the tested concept only when the learner explains it and handles that case. One lucky multiple-choice answer does not establish a whole lesson. If the check passes, use released time on the next core task. If it fails, teach the missed concept and retest with a changed case; fix a blocking gap before dependent work.
3. For new material, show a small worked example, explain its purpose and actual output, then ask the learner for an independent change. Wait for their attempt. Give focused hints or a repair example as needed, followed by a new changed case. Tutor-written code alone is not learner evidence.
4. Use one language, normally Python. Inspect the stated runner/imports, run the relevant reference demo and available deterministic tests where useful, then work in the learner copy. A focused introduction is not a full advanced lesson. Record unavailable runtimes or broken reference commands rather than silently counting them as successful.
5. Inspect the available stored quiz: some files are top-level lists, others have a `questions` field, and stage counts vary. On S rows, use relevant pre/check questions during work and available relevant post questions at the final assigned practice row or a repair slot; record the actual N/M. If quiz.json is absent or has no relevant items, use the row's interview prompts and independent changed-case check, record quiz as unavailable and preserve the practical result; no invented stored-quiz score. Repeated rows share one record. Retrieve only assigned questions and keep keys private until answered. Below 70% creates a focused Review queue item. F/R checks credit only the tested sections/concepts; assigned excerpts do not imply full lesson mastery. Quiz scores alone do not pass live/lab gates.
6. Use the last five minutes to save evidence and update Resume state, Progress log and Review queue. Record minutes used, row/work IDs, mode, checks/quiz, learner change, exact runnable command/result, provider mode, pending action and any displaced work. Derive the next action from those records. End with a short progress statement and the saved next task.

Normal slot: 45 minutes of listed work (including recall or teaching checks), 10 minutes on the row's interview IDs or post quiz, 5 minutes to record. The same 10 minutes can hold a quiz and a short interview question; reduce questions to fit. Recall/repair slot: up to 30 minutes repair, 25 practice/quiz, 5 record; use more repair time when a prerequisite blocks progress. Mock rows use their full 60-minute format below, without an extra drill. Evidence rows use 55 minutes of listed work and 5 recording. Stop at the allotted hour.

An interrupted hour remains `in_progress`; carry its unused minutes into the next chat. A deliberately closed short hour records its actual minutes and unused allowance as forfeited, so there is no extra slot. Closing an hour marks the time slot closed, not the task mastered. Track task outcomes as `passed`, `partial`, `deferred` or `cut`.

## Repairs, absences and budget changes

The 12 recall/repair slots are 8, 16, 24, 32, 40, 48, 56, 64, 72, 80, 88 and 96. They are spaced practice, not a requirement to relearn passed material. If the queue is empty, retrieve earlier concepts and do an independent changed case or start the next core task; record that early task so its later row is used for further practice or another gap.

If core work is unfinished, preserve its next action. Use the next repair slot when the intervening tasks are independent; when the gap blocks them, continue immediately using the next slot's allowance. Record what that displaces. The tutor decides cuts in this order: the optional hybrid row, optional rollout breadth, redundant repeats of passed material, then the least relevant breadth for the target role. If those cuts are insufficient, up to four of the 12 dedicated mock hours may become essential lessons or repair, retaining at least eight mocks, daily interview practice, all 12 recall/repair slots and both application-material hours. Record the substitution; that allowance is not used in the current schedule. Keep displaced items visibly deferred/cut, without silently renumbering the schedule.

After at least seven calendar days since the last study date, use up to 10-15 minutes for a representative recall and practical re-entry check. Charge this to the remaining allowance of an open slot, or the next slot if none is open; an unfinished check continues within the following slot, with displaced work recorded. Repair only what failed. A passed check does not require cuts; a failure uses repair capacity or the cut order above. Missed days themselves consume no time. Validation, access controls, provider error handling, basic retrieval, evaluation and the live integration gates retain priority.

The schedule is a default allocation, not a claim that unfamiliar work will fit on the first attempt. Reallocate within its 100 slots. At the end, record unresolved gaps if the completion gates have not passed; more study would require a new budget agreed with the learner. Do not label those gaps mastered or quietly add a 101st hour.

## Budget and numbered schedule

| Work block | Hours including drills/notes |
|---|---:|
| Practical placement and live HTTP APIs | 8 |
| Prompting, structured outputs and tools | 10 |
| Embeddings, retrieval and grounded generation | 18 |
| Evaluation, reliability and access | 12 |
| Local API, framework practice and operation | 16 |
| Bounded agents and explicit state | 10 |
| Timed interview practice | 12 |
| Spaced recall and repair | 12 |
| Application materials from the same lab | 2 |
| Total | 100 |

S = study/practice; R = conditional revision; F = focused introduction. Library rows extend a repository concept in the approved learner copy. Each numbered row is one hour. These are learning slots, not dated days or full-lesson duration promises. Follow the pending task if progress has required reallocation.

### Practical placement and live HTTP APIs

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 1 | R/F: 00.01 [Dev Environment](phases/00-setup-and-tooling/01-dev-environment/docs/en.md)<br>00.06 [Python Environments](phases/00-setup-and-tooling/06-python-environments/docs/en.md)<br>00.09 [Data Management](phases/00-setup-and-tooling/09-data-management/docs/en.md)<br>14.47 [Define the Outcome Before You Choose the Output](phases/14-agent-engineering/47-outcomes-before-output/docs/en.md)<br>14.51 [Write Specifications That Preserve Judgment](phases/14-agent-engineering/51-write-specifications-that-preserve-judgment/docs/en.md) | Use up to 15 minutes on the environment/C1 check. In the remaining work block, seed the tiny corpus and write one short lab contract: user question, expected evidence, read-only scope, unsupported-answer behavior and non-goals. Use only the outcome/specification sections; full product-discovery labs are not assigned. | Q1-Q2 |
| 2 | S: 00.04 [APIs & Keys](phases/00-setup-and-tooling/04-apis-and-keys/docs/en.md) | Tutor shows a minimal raw-HTTP request. Verify current free generation access, then make an independent changed request and save a redacted successful response. Fixtures do not pass this gate. | Q5,Q7 |
| 3 | S: 00.04 [APIs & Keys](phases/00-setup-and-tooling/04-apis-and-keys/docs/en.md) | Test timeout, 401, 429 and malformed response using an injected request function. Save one successful live path and deterministic failure checks. | Q3,Q5,C6 |
| 4 | R: 00.02 [Git & Collaboration](phases/00-setup-and-tooling/02-git-and-collaboration/docs/en.md)<br>00.12 [Debugging and Profiling](phases/00-setup-and-tooling/12-debugging-and-profiling/docs/en.md) | Without hints, explain a Git diff and diagnose a short broken request. Credit prior knowledge; use released time to improve the provider adapter. | Q7,Q46 |
| 5 | R: 00.09 [Data Management](phases/00-setup-and-tooling/09-data-management/docs/en.md) | Use sqlite3 and the hypothetical Documents relation for C8 and a transaction rollback. If passed, move into the next core task; do not assign a full SQL course. | Q8-Q10,C8 |
| 6 | R, concepts only: 10.01 [Tokenizers: BPE, WordPiece, SentencePiece](phases/10-llms-from-scratch/01-tokenizers/docs/en.md)<br>01.14 [Norms and Distances](phases/01-math-foundations/14-norms-and-distances/docs/en.md)<br>07.02 [Self-Attention from Scratch](phases/07-transformers-deep-dive/02-self-attention-from-scratch/docs/en.md) | Check tokens/context, cosine with a zero vector, and Q13 with a 5-8 minute Q/K/V weighted-value and causal-mask trace. Repair only misses and retest with changed values. Save C3 and the attention check; full tokenizer/transformer implementations are not assigned. | Q11-Q14,Q18,C3 |
| 7 | R/S: 05.02 [Bag of Words, TF-IDF, and Text Representation](phases/05-nlp-foundations-to-advanced/02-bag-of-words-tfidf/docs/en.md)<br>11.04 [Embeddings & Vector Representations](phases/11-llm-engineering/04-embeddings/docs/en.md) | Check TF-IDF first, then run the lexical reference embedder. Rank a tiny corpus and save a misleading match; distinguish this from learned embeddings. | Q12,Q18 |
| 8 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 9 | R/F: 01.15 [Statistics for Machine Learning](phases/01-math-foundations/15-statistics-for-ml/docs/en.md)<br>02.09 [Model Evaluation](phases/02-ml-fundamentals/09-model-evaluation/docs/en.md)<br>14.52 [Design Success Metrics Before the Result Exists](phases/14-agent-engineering/52-design-success-metrics/docs/en.md) | Use up to 15 minutes for leakage, precision/recall, a train/validation curve, one gradient update and training-versus-inference checks. Use 15 minutes to freeze metric definitions, cases/window, thresholds and fail/ambiguous decisions before baseline outputs. Use 15 minutes to freeze a compact T01-T08 tuning and H01-H04 reserved manifest: short questions plus expected source IDs, not detailed output fixtures. Unfinished work uses repair capacity. | Q29,Q37-Q40 |

### Prompting, structured outputs and tools

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 10 | S: 11.01 [Prompt Engineering: Techniques & Patterns](phases/11-llm-engineering/01-prompt-engineering/docs/en.md) | Reuse the live provider adapter on three fixed Q&A prompts with supplied evidence. Save the actual outputs, model ID and template version as a baseline. | Q14-Q16 |
| 11 | S: 11.01 [Prompt Engineering: Techniques & Patterns](phases/11-llm-engineering/01-prompt-engineering/docs/en.md) | Compare the baseline with one controlled prompt change, such as one short example demonstrating answer/citation/abstention format. Keep tuning cases/model settings fixed, inspect support and relevance by hand, and save a failure as well as any improvement. | Q6,Q16,Q44 |
| 12 | S: 11.03 [Structured Outputs: JSON, Schema Validation, Constrained Decoding](phases/11-llm-engineering/03-structured-outputs/docs/en.md) | Build a stdlib validator for answer, citations and abstention. Independently reject wrong types, missing fields and invalid citation IDs. | Q6,C2 |
| 13 | S: 11.03 [Structured Outputs: JSON, Schema Validation, Constrained Decoding](phases/11-llm-engineering/03-structured-outputs/docs/en.md) | Connect live generation to parsing and validation. Check that quoted evidence supports the answer; syntactically valid JSON is insufficient. | Q6,Q16 |
| 14 | S: 11.03 [Structured Outputs: JSON, Schema Validation, Constrained Decoding](phases/11-llm-engineering/03-structured-outputs/docs/en.md) | Add deterministic malformed-output, empty-evidence and unsupported-claim cases. Bound any repair attempt and make failure visible to the caller. | Q6,Q7 |
| 15 | S: 11.09 [Function Calling & Tool Use](phases/11-llm-engineering/09-function-calling/docs/en.md) | Build a read-only document lookup tool with an allowlist, narrow argument schema and explicit error result. Trace a fixed successful call. | Q25 |
| 16 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 17 | S: 11.09 [Function Calling & Tool Use](phases/11-llm-engineering/09-function-calling/docs/en.md) | Use current provider documentation to request one real model-selected lookup call; validate, execute and return the result. A scripted proposer stays labeled scripted. | Q24-Q25 |
| 18 | S: 11.09 [Function Calling & Tool Use](phases/11-llm-engineering/09-function-calling/docs/en.md) | Try an unknown tool, invalid arguments, forbidden document and failed lookup. Save checks that stop execution before an unauthorized action. | Q23,Q25 |
| 19 | S: 11.12 [Guardrails, Safety & Content Filtering](phases/11-llm-engineering/12-guardrails/docs/en.md) | Separate instructions from untrusted document text. Demonstrate allowed, unsupported and hostile-input cases; keep authorization in code. | Q23,Q26 |
| 20 | S: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Create an evaluation callback that runs the actual learner generator on saved case IDs. Store schema and human-reviewed support outcomes; leave simulated judges labeled. | Q22,Q29-Q30 |

### Embeddings, retrieval and grounded generation

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 21 | S: 00.09 [Data Management](phases/00-setup-and-tooling/09-data-management/docs/en.md) | Ingest 8-12 tiny public/synthetic documents with stable IDs, source IDs and versions. Use json/csv/hashlib; check duplicates and malformed records. | Q1,Q43,C1 |
| 22 | S: 05.23 [Chunking Strategies for RAG](phases/05-nlp-foundations-to-advanced/23-chunking-strategies-rag/docs/en.md) | Tutor works a chunk boundary example, then learner builds a small chunker that keeps source IDs and spans. Save an independent changed document. | Q19,C4 |
| 23 | S: 05.23 [Chunking Strategies for RAG](phases/05-nlp-foundations-to-advanced/23-chunking-strategies-rag/docs/en.md) | Test empty text, final short chunk and invalid overlap; prove the loop terminates. Record one chunking choice with its tradeoff. | Q19,C4 |
| 24 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 25 | S: 05.14 [Information Retrieval and Search](phases/05-nlp-foundations-to-advanced/14-information-retrieval-search/docs/en.md)<br>11.04 [Embeddings & Vector Representations](phases/11-llm-engineering/04-embeddings/docs/en.md) | Build an exact lexical baseline and inspect ranked evidence for fixed query IDs. Save expected relevant document IDs before changing retrieval. | Q17,Q22 |
| 26 | S: 11.04 [Embeddings & Vector Representations](phases/11-llm-engineering/04-embeddings/docs/en.md) | Verify current free embedding access and obtain real learned embeddings for the tiny corpus and query. Cache vectors with model/version metadata. | Q12,Q18 |
| 27 | S: 11.04 [Embeddings & Vector Representations](phases/11-llm-engineering/04-embeddings/docs/en.md) | Validate dimensions, zero vectors and embedding-model consistency. Test a stale/mismatched index and fail clearly instead of comparing incompatible vectors. | Q18,Q54,C3 |
| 28 | S: 11.04 [Embeddings & Vector Representations](phases/11-llm-engineering/04-embeddings/docs/en.md) | Rank cached learned vectors with scratch exact cosine search. Compare relevant evidence against the lexical baseline on unchanged queries. | Q18,Q22 |
| 29 | S + library: 11.04 [Embeddings & Vector Representations](phases/11-llm-engineering/04-embeddings/docs/en.md)<br>11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Use Chroma PersistentClient in the learner copy with precomputed embeddings and embedding_function=None. Upsert stable IDs and query with query_embeddings; avoid default model downloads. | Q54 |
| 30 | S + library: 11.04 [Embeddings & Vector Representations](phases/11-llm-engineering/04-embeddings/docs/en.md)<br>11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Restart the process and verify persisted results. Keep embedding versions and corpus scopes separate; test stale data deletion or collection rebuild. | Q23,Q54 |
| 31 | S: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Measure retrieval hit and recall on human-labeled evidence for fixed tuning queries; distinguish a single relevant hit from recovering all required evidence. Explain small-sample limits and save a missed case. Slot 39 adds the precise metric exercise. | Q22,Q39 |
| 32 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 33 | S: 11.05 [Context Engineering: Windows, Budgets, Memory, and Retrieval](phases/11-llm-engineering/05-context-engineering/docs/en.md)<br>11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Build the context adapter: selected passages with source IDs, a bounded context and no instructions accepted from retrieved text. | Q11,Q17 |
| 34 | S: 11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Connect retrieval, the real provider adapter and output validation in one command. Save a supported answer, its citations and the request path. | Q16-Q17,Q41 |
| 35 | S: 11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Test an unanswerable question and irrelevant evidence. Demonstrate abstention and record any real-model failure rather than silently replacing it. | Q16,Q22 |
| 36 | S: 11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Handle conflicting sources and stale documents. Check source IDs and claim support; preserve uncertainty instead of forcing a single answer. | Q43 |
| 37 | S: 05.23 [Chunking Strategies for RAG](phases/05-nlp-foundations-to-advanced/23-chunking-strategies-rag/docs/en.md)<br>11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Compare two chunk/overlap settings with fixed queries and model settings. Keep both retrieval and answer results so the cause of a change is visible. | Q19,Q44 |
| 38 | F, optional: 11.07 [Advanced RAG (Chunking, Reranking, Hybrid Search)](phases/11-llm-engineering/07-advanced-rag/docs/en.md) | Try one tiny hybrid lexical/vector merge if the core path passes. Keep only a measured or explained benefit; this slot can fund repair. | Q20 |
| 39 | S, selected 45-minute metric exercise: 19.68 [RAG Evaluation: Precision, Recall, MRR, nDCG, Faithfulness, Answer Relevance](phases/19-capstone-projects/68-rag-eval-precision-recall/docs/en.md)<br>11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Replace the optional reranker survey with P@k, R@k and MRR on the same learner qrels. Use only its standalone stdlib metric functions, then independently score a changed ranked list; the full lesson and Phase 19 prerequisite route are not assigned. Compare a grounded-but-off-topic answer and a token-overlap judge false positive with human support/relevance labels. nDCG implementation stays reference; no second capstone or paid judge is assigned. | Q22,Q30,Q55,C11 |
| 40 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 41 | S: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Run reserved H01-H04 queries once, inspect evidence and answer failures separately, and save the retrieval/generation report. If their inspection informs a design change, label later H results exploratory or freeze new held-out cases; do not report reused H cases as untouched. | Q22,Q29,Q44 |

### Evaluation, reliability and access

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 42 | S: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Complete/version T01-T08 plus H01-H04 across normal, unsupported, conflict, stale-data, malformed-output and hostile-input categories. Preserve split IDs and the slot-9 measurement contract; if a new failure category needs a changed metric, record why before measuring. Use T cases for further tuning. | Q29,Q55,C5 |
| 43 | S: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md)<br>19.68 [RAG Evaluation: Precision, Recall, MRR, nDCG, Faithfulness, Answer Relevance](phases/19-capstone-projects/68-rag-eval-precision-recall/docs/en.md) | Run the actual Q&A generator on a small free subset of T cases and save redacted outputs. Keep inspected H outputs as the slot-41 report. Grade schema validity, claim support, answer relevance and abstention separately; deterministic word overlap is not a truth judge. Save per-case results against the frozen criteria. | Q22,Q30,Q55 |
| 44 | S: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Compare one controlled prompt or retrieval change on unchanged T cases. Report counts by category and which run used live calls versus cached successful outputs. | Q29,Q44,C5 |
| 45 | R/S: 01.15 [Statistics for Machine Learning](phases/01-math-foundations/15-statistics-for-ml/docs/en.md)<br>11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Explain uncertainty without unsupported significance claims. Repeat a small live T sample if quota permits; save nondeterminism or the quota blocker. | Q14,Q30,Q39 |
| 46 | S: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Provide one local regression command with meaningful boundary checks and a failing-case demonstration. Fixture runs establish plumbing, not live quality. | Q7,Q29 |
| 47 | S: 11.12 [Guardrails, Safety & Content Filtering](phases/11-llm-engineering/12-guardrails/docs/en.md)<br>14.27 [Prompt Injection and the PVE Defense](phases/14-agent-engineering/27-prompt-injection-defense/docs/en.md) | Put a hostile instruction inside a document and trace it through the actual app. Check that it cannot grant permissions or execute an unknown tool. | Q23,Q25 |
| 48 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 49 | S: 11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Use two synthetic caller scopes and authorize before retrieval. Test guessed document IDs and cross-scope queries; keep forbidden evidence out of the model context. | Q23 |
| 50 | S: 11.12 [Guardrails, Safety & Content Filtering](phases/11-llm-engineering/12-guardrails/docs/en.md)<br>11.09 [Function Calling & Tool Use](phases/11-llm-engineering/09-function-calling/docs/en.md) | Test permission failures before model/tool invocation and safe caller errors. The local trusted caller scope is a test boundary, not production authentication. | Q23,Q51 |
| 51 | S: 11.11 [Caching, Rate Limiting & Cost Optimization](phases/11-llm-engineering/11-caching-cost/docs/en.md)<br>11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Integrate bounded timeouts/backoff and rate-limit handling. Test 401 versus 429 and prove retries stop; a quota failure remains a visible failure. | Q3,Q34,C6 |
| 52 | S: 11.11 [Caching, Rate Limiting & Cost Optimization](phases/11-llm-engineering/11-caching-cost/docs/en.md)<br>11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Build a cache key with query, source versions, prompt/model/embedding version and caller scope. Check invalidation and forbidden cache reuse. | Q32,C7 |
| 53 | S: 17.13 [LLM Observability Stack Selection](phases/17-infrastructure-and-production/13-llm-observability/docs/en.md) | Instrument the learner request path with run ID, versions, retrieval IDs, measured latency and errors. Redact keys/text and label missing token/cost fields. | Q31,Q35 |
| 54 | S: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md)<br>11.12 [Guardrails, Safety & Content Filtering](phases/11-llm-engineering/12-guardrails/docs/en.md) | Save a safety/evaluation report with observed failures, passing boundary checks and unresolved gaps. Repair a blocking issue before app expansion. | Q22-Q23,Q44 |

### Local API, framework practice and operation

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 55 | S: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Inspect the simulated production reference and map its missing connections. Reuse the already connected learner path; identify unsafe cache and error behavior to replace. | Q41,Q45 |
| 56 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 57 | S: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Make one explicit ask function compose retrieval, model request, validation, errors and evaluation hooks. Exercise normal and denied calls through this shared path. | Q17,Q41 |
| 58 | S + library: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Wrap the shared path in a minimal FastAPI /ask endpoint and run Uvicorn bound to 127.0.0.1. Define typed request/response fields and size bounds. | Q33,Q51 |
| 59 | S + library: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Add HTTP-boundary checks for success, bad input, denied/missing document and provider failure using a stdlib client against the local server. No new test framework is required. | Q51,C9 |
| 60 | S: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Use a stdlib client to make a real request through /ask. Save a redacted response and failure example, then stop the server; a local API is not public deployment. | Q5,Q7,Q45 |
| 61 | S + library: 11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Build the equivalent small LangChain LCEL flow with RunnableLambda around existing retrieval/provider/validation functions. Keep the free HTTP adapter and the same corpus. | Q52 |
| 62 | S + library: 11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md)<br>11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Run the same cases through scratch and LCEL paths. Explain framework plumbing, record versions, and keep the simpler path as the default if results are equivalent. | Q47,Q52 |
| 63 | S: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Check blocking I/O inside the API and choose a sync endpoint or bounded offloading correctly. Test timeout and two simultaneous requests without unbounded concurrency. | Q4,Q34 |
| 64 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 65 | S: 11.11 [Caching, Rate Limiting & Cost Optimization](phases/11-llm-engineering/11-caching-cost/docs/en.md)<br>11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Bound request/context sizes and work per request. Check cancellation/error cleanup and make quota limits visible without promising unlimited free traffic. | Q11,Q26,Q34 |
| 66 | S/F: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>17.25 [Security  -  Secrets, API Key Rotation, Audit Logs, Guardrails](phases/17-infrastructure-and-production/25-security-secrets-audit/docs/en.md) | Separate environment config and secrets, add a small health check, and test missing configuration and a synthetic secret-like value absent from logs/errors/tracked fixtures. Read only relevant secrets/redaction sections; vault/gateway deployments and real key rotation are not assigned. Save exact local commands. | Q33,Q35,Q51 |
| 67 | R: 00.07 [Docker for AI](phases/00-setup-and-tooling/07-docker-for-ai/docs/en.md) | Check existing Docker knowledge, then package the local service if the runtime is available. No GPU image; if unavailable save the exact blocker and use the Python environment. | Q33 |
| 68 | S: 00.02 [Git & Collaboration](phases/00-setup-and-tooling/02-git-and-collaboration/docs/en.md)<br>11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Connect the deterministic regression command to repository-style CI in the learner lab or demonstrate it locally if remote CI is unavailable. Keep live free-provider tests manual. | Q7,Q33 |
| 69 | F, optional: 17.20 [Shadow Traffic, Canary Rollout, and Progressive Deployment for LLMs](phases/17-infrastructure-and-production/20-shadow-canary-progressive/docs/en.md) | Practice a local config/prompt rollback against a saved baseline. Public rollout infrastructure is not assigned; this slot can fund repair. | Q36 |
| 70 | S: 17.13 [LLM Observability Stack Selection](phases/17-infrastructure-and-production/13-llm-observability/docs/en.md) | Trace one failed answer from request to evidence, provider and validation. Save a diagnosis with measured data and a regression check. | Q35,Q46 |
| 71 | S: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Run the full local client path and regression checks from a clean process. Demonstrate persisted retrieval, a real answer, abstention and a denied/error case. | Q41,Q45 |
| 72 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 73 | S: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Without following a solution, make one changed-case app fix and explain the affected request path. Record learner versus tutor contributions and limitations. | Q42,Q46-Q48 |

### Bounded agents and explicit state

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 74 | S: 14.01 [The Agent Loop: Observe, Think, Act](phases/14-agent-engineering/01-the-agent-loop/docs/en.md) | Trace the reference scripted loop, then build a tiny read-only agent loop around the existing lookup tool. Define allowed actions and stop conditions first. | Q24-Q26 |
| 75 | S: 14.01 [The Agent Loop: Observe, Think, Act](phases/14-agent-engineering/01-the-agent-loop/docs/en.md)<br>11.09 [Function Calling & Tool Use](phases/11-llm-engineering/09-function-calling/docs/en.md) | Drive one lookup with actual model-selected tool arguments and return evidence. Save the real trace; a scripted fallback does not pass the live-tool gate. | Q25,Q41 |
| 76 | S: 14.26 [Failure Modes: Why Agents Break](phases/14-agent-engineering/26-failure-modes-agentic/docs/en.md) | Independently test repeated tool calls, unavailable tool and max-step termination. Keep retrieval-only actions and bounded time/model calls. | Q26 |
| 77 | S: 14.13 [Stateful Graph Orchestration  -  Durable Execution and Checkpoints](phases/14-agent-engineering/13-langgraph-stateful-graphs/docs/en.md) | Implement small explicit scratch state and trace transitions. Explain what survives in memory and what is lost on process restart. | Q27-Q28 |
| 78 | S + library: 14.13 [Stateful Graph Orchestration  -  Durable Execution and Checkpoints](phases/14-agent-engineering/13-langgraph-stateful-graphs/docs/en.md) | Use actual LangGraph StateGraph with named lookup, answer and validation nodes plus START/END. Reuse existing functions; keep state small and calls bounded. | Q28,Q53 |
| 79 | S + library: 14.13 [Stateful Graph Orchestration  -  Durable Execution and Checkpoints](phases/14-agent-engineering/13-langgraph-stateful-graphs/docs/en.md) | Add explicit failure/termination paths and a changed trace check. A fixed DAG needs no checkpoint service; do not claim durable recovery from this exercise. | Q27,Q53,C10 |
| 80 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 81 | S: 14.13 [Stateful Graph Orchestration  -  Durable Execution and Checkpoints](phases/14-agent-engineering/13-langgraph-stateful-graphs/docs/en.md) | Exercise graph step bounds and a failed lookup with deterministic providers. Inspect trace evidence and repair one transition independently. | Q26,Q53,C10 |
| 82 | S: 14.13 [Stateful Graph Orchestration  -  Durable Execution and Checkpoints](phases/14-agent-engineering/13-langgraph-stateful-graphs/docs/en.md)<br>14.27 [Prompt Injection and the PVE Defense](phases/14-agent-engineering/27-prompt-injection-defense/docs/en.md) | Keep caller scope and untrusted documents separate from agent instructions/state. Test cross-scope retrieval and hostile tool content. | Q23,Q27 |
| 83 | S: 14.30 [Eval-Driven Agent Development](phases/14-agent-engineering/30-eval-driven-agent-development/docs/en.md) | Evaluate recorded learner trajectories for tool choice, argument validity, evidence and termination. Use a small live subset; scripted reference scores remain separate. | Q25-Q26,Q29 |
| 84 | S: 14.01 [The Agent Loop: Observe, Think, Act](phases/14-agent-engineering/01-the-agent-loop/docs/en.md)<br>14.13 [Stateful Graph Orchestration  -  Durable Execution and Checkpoints](phases/14-agent-engineering/13-langgraph-stateful-graphs/docs/en.md) | Compare the fixed Q&A pipeline and bounded agent on unchanged tasks. Explain when dynamic tool choice helps and when the fixed flow is sufficient. | Q24,Q28,Q47 |

### Timed interview practice

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 85 | Mock: 00.09 [Data Management](phases/00-setup-and-tooling/09-data-management/docs/en.md) | Coding mock: C1 plus a changed streaming/missing-ID case. Use the coding format and record one concrete gap. | Q1-Q2,C1 |
| 86 | Mock: 11.03 [Structured Outputs: JSON, Schema Validation, Constrained Decoding](phases/11-llm-engineering/03-structured-outputs/docs/en.md)<br>11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Coding mock: C2 or C9 with a malformed HTTP/model result and useful safe errors. | Q6,Q51,C2,C9 |
| 87 | Mock: 00.09 [Data Management](phases/00-setup-and-tooling/09-data-management/docs/en.md) | Coding/SQL mock: C8 using sqlite3, duplicates, NULLs and a transaction failure; explain the result. | Q8-Q10,C8 |
| 88 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 89 | Mock: 11.04 [Embeddings & Vector Representations](phases/11-llm-engineering/04-embeddings/docs/en.md)<br>11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | Coding mock: C3 and a stale persistent collection or dimension mismatch. Explain expected work and the real learned-vector path. | Q18,Q54,C3 |
| 90 | Mock: 05.23 [Chunking Strategies for RAG](phases/05-nlp-foundations-to-advanced/23-chunking-strategies-rag/docs/en.md) | Coding mock: C4 with changed chunk boundaries and invalid overlap; prove it terminates. | Q19,C4 |
| 91 | Mock: 11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md)<br>19.68 [RAG Evaluation: Precision, Recall, MRR, nDCG, Faithfulness, Answer Relevance](phases/19-capstone-projects/68-rag-eval-precision-recall/docs/en.md) | Coding mock: C5 or C11 with missing case IDs, a misleading average, or a changed gold set. Explain retrieval versus supported/relevant answers and the held-out split. | Q22,Q29-Q30,Q55,C5,C11 |
| 92 | Mock: 11.06 [RAG (Retrieval-Augmented Generation)](phases/11-llm-engineering/06-rag/docs/en.md) | AI design mock: a document Q&A request, an unanswerable question, a restricted document and an answer that is supported but off-topic. Draw Mermaid/SVG only if useful. | Q15-Q23,Q55 |
| 93 | Mock: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>17.13 [LLM Observability Stack Selection](phases/17-infrastructure-and-production/13-llm-observability/docs/en.md) | AI design mock: provider timeout/429, config, logs and scoped cache. Use C6/C7 as a changed code case. | Q31-Q36,C6-C7 |
| 94 | Mock: 14.13 [Stateful Graph Orchestration  -  Durable Execution and Checkpoints](phases/14-agent-engineering/13-langgraph-stateful-graphs/docs/en.md)<br>14.30 [Eval-Driven Agent Development](phases/14-agent-engineering/30-eval-driven-agent-development/docs/en.md) | AI design/graph mock: a looping tool trace and failed lookup. Repair it while retaining scope and bounds. | Q24-Q28,Q53,C10 |
| 95 | Mock: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Project deep-dive mock: repeatable demo, baseline/change results, one bug, contribution boundaries and deployment status. | Q41-Q48,Q52 |
| 96 | Recall/repair; current Review queue and earlier S/R rows | Test a previously learned concept without hints; repair only misses and use a changed-case retest. Save evidence and clear only demonstrated gaps. If already passed, use the time for the next core task or independent practice. | Current gaps and assigned post quizzes |
| 97 | Mock: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Combined mock: a small app change, basic ML/LLM recall and behavioral examples grounded in actual work. | Q37-Q40,Q42,Q49-Q50 |
| 98 | Mock: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>14.13 [Stateful Graph Orchestration  -  Durable Execution and Checkpoints](phases/14-agent-engineering/13-langgraph-stateful-graphs/docs/en.md) | Final combined mock: choose unseen changed cases across API, RAG and graph work. Grade with the rubric and preserve any unresolved critical gap. | Q17,Q23,Q41,Q51-Q54 |

### Application materials from the same lab

| Slot | Mode and repository material | Work and evidence within 60 minutes | Interview/quiz focus |
|---|---|---|---|
| 99 | Evidence: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md)<br>11.10 [Evaluation & Testing LLM Applications](phases/11-llm-engineering/10-evaluation/docs/en.md) | Use this hour for the lab README, run/test commands, a short repeatable demo and a small baseline/change results table. State local/live/fixture status and remaining limits. | Q41,Q44-Q45 |
| 100 | Evidence: 11.13 [Building a Production LLM Application](phases/11-llm-engineering/13-production-app/docs/en.md) | Write accurate resume bullets from saved work and measurements, link the same lab, and check the completion gates below. Actual job searching and applications use separate time. | Q42,Q47,Q49-Q50 |

## Interview practice bank

These are plausible practice prompts, not known employer questions. Start with the current row's assigned IDs. Answer aloud in one to three minutes, then take a follow-up or a small changed-case task. Use the lesson quizzes only for assigned questions. Keep answer keys private until the learner responds, and fetch only the assigned questions. The criteria below describe evidence of a sound answer, not a script. Use the continuing document Q&A assistant and its focused repair as the main examples. State clearly when a feature is a local simulation or an unfinished deployment.

| ID | Area | Practice question | A sound answer should include |
|---|---|---|---|
| Q1 | Python/API | How would you deduplicate document records by `doc_id` while preserving order? | A set or dict for identity, an ordered result, explicit duplicate policy, expected O(n) work, and a policy for missing IDs. |
| Q2 | Python/API | When would you use a generator rather than a list? | Streaming versus materialization, bounded memory, one-pass behavior, and a document-processing example. |
| Q3 | Python/API | How would you handle exceptions and retry an API request? | Specific errors, timeouts, bounded retry/backoff, no retry for invalid credentials, and idempotency concerns. |
| Q4 | Python/API | What does async/await help with in a local LLM service? | Waiting on I/O, bounded concurrency, timeout/cancellation, and that it does not speed CPU-heavy work by itself. |
| Q5 | Python/API | What do 401, 403, 429, and 5xx mean, and what should the caller do? | Authentication versus authorization versus quota versus server failure, with a suitable retry policy and clear error response. |
| Q6 | Python/API | How would you validate JSON returned by a model? | Safe parsing, required fields/types/constraints, rejection or repair path, and that valid shape does not prove truth. |
| Q7 | Python/API | How do unit, integration, and real-provider tests differ? | Scope, mocks, deterministic assertions, cost/nondeterminism, and what a mock cannot verify. |
| Q8 | SQL/backend | How do INNER JOIN and LEFT JOIN differ in a document application? | Matching rows versus retaining unmatched left rows; explain nulls and duplicate rows from one-to-many joins. |
| Q9 | SQL/backend | With `Documents(doc_id, topic_id, source_id)`, how would you find topics supported by at least two distinct sources? | Group by `topic_id`, count distinct `source_id`, filter with HAVING, and explain null and duplicate handling. |
| Q10 | SQL/backend | When would an index or transaction help a document Q&A service? | A real filter/order access pattern; atomic related writes and failure handling; index/write tradeoffs. |
| Q11 | LLM | What is a token and why does the context limit matter? | Subword units, input/output budget, truncation, cost, and tokenizer/model dependence. |
| Q12 | LLM | How are embeddings different from generated text? | A representation for similarity/retrieval versus next-token generation; dimensions and model consistency. |
| Q13 | LLM | Explain attention at a basic level. | Query/key/value, relevance-weighted combination, causal masking for generation; trace shapes only if useful. |
| Q14 | LLM | What does temperature change? Does zero guarantee identical, correct answers? | Sampling distribution; lower randomness does not guarantee truth or absolute determinism. |
| Q15 | LLM | When would you choose prompting, RAG, or fine-tuning? | Instructions/examples; current or private evidence; behavior adaptation. Choose based on a measured failure. |
| Q16 | LLM | Why can a model hallucinate even with RAG? | Missing or irrelevant evidence, retrieval/generation errors, misleading sources; evaluation, source checks, and abstention. |
| Q17 | RAG | Explain one document Q&A request end to end. | Ingestion, extraction, chunking, embeddings/indexing, query filters and retrieval, context selection, generation, source references, validation, and logging. |
| Q18 | RAG | How does cosine similarity work? | Dot product divided by vector norms, direction rather than magnitude, zero-vector handling, and semantic limits. |
| Q19 | RAG | How would you choose chunk size and overlap for a document set? | Document structure and query types, boundary/context tradeoffs, repeated text and token cost; compare on fixed cases. |
| Q20 | RAG | Why combine keyword and vector search? | Exact terms and identifiers versus semantic matches; merge/rank candidates and compare against each baseline. |
| Q21 | RAG | What is reranking and when is it useful? | Score a retrieved candidate set more carefully; trade latency/cost against ordering and answer quality. |
| Q22 | RAG/evaluation | How would you evaluate retrieval separately from the generated answer? | Gold evidence and ranking metrics versus claim support, answer relevance and abstention. A supported answer can be off-topic; use fixed human-reviewed cases. |
| Q23 | RAG/security | How would you stop retrieval or caching from exposing a document outside the caller's access? | Authorize before retrieval, preserve scope through context and cache, reject guessed IDs, and test forbidden access. |
| Q24 | Agents | How does an agent differ from a fixed workflow? | Dynamic tool/action choices versus predefined control flow; choose the simpler system that meets the need. |
| Q25 | Agents | What happens after a model proposes a tool call? | Validate arguments and scope, enforce permissions, execute only allowed code, return a result, handle failure. |
| Q26 | Agents | How would you stop a looping or expensive agent? | Step/time/token/cost limits, failure handling, clear termination, and approval before risky side effects. |
| Q27 | Agents | What is the difference between context, memory, and persistent state? | Prompt inputs, retained information, and recoverable task state; an in-memory checkpoint is not restart recovery. |
| Q28 | Agents/LangGraph | What does graph state add to a document workflow, and when is a fixed pipeline enough? | Named state, bounded nodes/edges, explicit stop conditions, traceability, and the cost of unnecessary agent control flow. |
| Q29 | Evaluation | What belongs in an evaluation set, and how do you avoid leakage? | Representative normal/failure/abstention cases, versioned expected checks, and held-out cases not used for tuning. |
| Q30 | Evaluation | What can go wrong with an LLM judge? | Bias, inconsistency, rubric errors and false confidence; calibration, human review and deterministic checks. |
| Q31 | Operations | How would you measure answer quality, latency, and cost? | Task-specific quality checks, request/token latency where available, errors, cost per useful answer, and labeling simulated measurements. |
| Q32 | Operations | What should a document-answer cache key account for? | Document IDs/versions, source set, embedding/model/prompt configuration, caller access scope, expiry and invalidation. |
| Q33 | Operations | How do FastAPI, local containers, CI and deployment fit this assistant? | Reproducible local runtime, request validation, tests/review, config/secrets/health checks; distinguish a local endpoint from a deployed service. |
| Q34 | Operations | What would you do if a provider timed out or returned 429? | Bounded timeout/retry, backoff, rate limits/fallback, useful errors, and safe handling of side effects. |
| Q35 | Operations | Which logs help debug a bad answer without leaking document contents? | Request/run IDs, versions, retrieval/tool metadata, latency/errors/cost; redact or omit secrets and private text. |
| Q36 | Operations | How would you release a changed prompt, embedding model or retriever and roll back? | Offline comparison on fixed cases, limited exposure, observable criteria, versioned configuration, and a tested return to baseline. |
| Q37 | Degree ML | Explain overfitting, underfitting, and one remedy. | Train/validation behavior, capacity/data/regularization/early stopping; diagnose before choosing a remedy. |
| Q38 | Degree ML | Why use train, validation, and test splits? | Fit, tune and final-estimate roles; avoid duplicate/time/entity leakage and test-set misuse. |
| Q39 | Degree ML | When is accuracy misleading? Explain precision, recall and F1. | Imbalance and error costs; correct denominators and task-appropriate metrics. |
| Q40 | Degree ML | Explain gradient descent and training versus inference. | Loss gradients and parameter updates during fitting; forward computation with learned parameters at inference. |
| Q41 | Project deep dive | Walk through the document Q&A assistant request path. | A concrete question and source document, component/data flow, retrieval/context, answer checks, and one limitation. State which access controls are implemented or missing. |
| Q42 | Project deep dive | What did you build yourself, and where did AI assistance help? | Specific design/code/test ownership; explain and change it; do not claim generated code you cannot explain. |
| Q43 | Project deep dive | How does the assistant handle duplicate, stale, malformed or unsupported documents? | Stable identity/versioning, index refresh, provenance, validation, and failure cases; distinguish toy checks from guarantees. |
| Q44 | Project deep dive | What did you measure and improve? | Baseline, fixed cases, real versus simulated outputs, measured change, and remaining failure categories. |
| Q45 | Project deep dive | What is actually running or tested today? | Exact local components and commands, provider mode, access/error tests, deployment status, and honest gaps. |
| Q46 | Project deep dive | Tell me about a difficult bug or failed repair. | Symptom, evidence, root cause or uncertainty, focused fix, changed-case regression check, and result. |
| Q47 | Project deep dive | Why did you choose this stack and retrieval approach? | Existing skills and time limits, one considered alternative, practical or measured reason, and tradeoff. |
| Q48 | Project deep dive | What would you implement next and why? | A user or failure need, small scoped change, acceptance criteria, and priority over speculative features. |
| Q49 | Behavioral | Describe feedback that changed your implementation. | Concrete input, what you reconsidered, the change, and what happened; use a real example. |
| Q50 | Behavioral | How do you handle a task you cannot finish or a concept you do not know? | Clarify scope, investigate, communicate the blocker, seek focused help, and propose a manageable next step. |
| Q51 | FastAPI | How would you validate a `/ask` request and return useful errors without leaking provider or document details? | Request schema and size limits, explicit invalid-input versus not-found/denied/provider errors, safe status codes, and no private text/secrets in responses. |
| Q52 | Framework comparison | How would you compare a LangChain document Q&A chain with a small from-scratch equivalent? | Same documents, chunking, embedding model and test questions; identify framework plumbing versus retrieval/generation behavior; record version and one limitation. |
| Q53 | LangGraph | How would you keep a LangGraph document workflow bounded and inspectable? | Small explicit state, allowed transitions, step limit, terminal/error states, trace fields and a test for the stop condition. |
| Q54 | Chroma | What must be controlled when persisting Chroma data across runs or embedding-model changes? | Stable collection/document IDs, persistence path, embedding-model/version metadata, isolation between document sets, and rebuild/migration behavior. |
| Q55 | Evaluation | How would you judge an answer that cites true evidence but does not answer the question, and a retriever that finds only one of several needed passages? | Separate support from answer relevance; distinguish hit rate, precision@k, recall@k and MRR; state the gold labels, denominator, case split and frozen success criteria. |

## Coding and SQL practice

Use these in allocated interview or mock sessions, not as extra homework. Use the document Q&A assistant and existing coursework. State assumptions, write a small check, and explain edge cases and time/space cost. DSA continues separately; this list focuses on work close to an AI application's daily code.

| Task | What to implement or explain | Relevant scheduled material |
|---|---|---|
| C1 | Deduplicate document dictionaries by `doc_id` while preserving order; handle a missing ID and a duplicate. | Python data handling; existing knowledge |
| C2 | Validate a model result with required fields, types, allowed values and useful errors. | Structured outputs and provider integration |
| C3 | Compute cosine similarity and rank a small candidate set; handle a zero vector and dimension mismatch. | Embeddings and retrieval foundations |
| C4 | Implement a simple document chunker; ensure overlap cannot cause an infinite loop and preserve the final chunk. | Chunking and retrieval |
| C5 | Aggregate pass/fail results by category and compare two evaluation runs on the same case IDs. | Evaluation and regression checks |
| C6 | Implement bounded retry using an injected failing request function; do not retry authentication errors or unsafe side effects blindly. | HTTP and error handling |
| C7 | Explain or implement a scoped cache key with document version, configuration and caller scope, plus invalidation. | Retrieval, security and operations |
| C8 | With `Documents(doc_id, topic_id, source_id)`, find topic IDs with at least two distinct sources; explain JOIN/NULL/duplicate behavior. | Prior SQL/App Dev Lab knowledge; hypothetical document relation |
| C9 | Add a local FastAPI `/ask` endpoint with request validation and deterministic tests for success, malformed input, missing document and provider failure. Use a fake provider in tests; test the HTTP boundary without requiring a key or live provider. | Local application and API integration |
| C10 | Given a failing document Q&A trace, make one focused LangGraph state or transition repair. Keep the step bound, add one changed case, and verify the trace and result without changing unrelated behavior. | Bounded graph workflow and focused repair |
| C11 | Independently score a tiny ranked list against gold document IDs with precision@k, recall@k and reciprocal rank. Handle an empty gold set/abstention separately and explain duplicate-ID handling. Reject invalid k in the learner version; the reference precision function instead returns 0.0 for k <= 0. | 19.68, the same learner qrels and evaluation callback |

## Mock structure and readiness checks

Every mock is 60 minutes including feedback and recording. Do not add a separate review afterward.

| Mock | 60-minute structure |
|---|---|
| Coding | 5 minutes clarify, 25 implement, 12 test/debug, 8 explain, 5 feedback, 5 record. |
| AI design | 7 minutes clarify, 15 design the document Q&A flow, 13 discuss evaluation/errors/access, 10 handle a changed case, 10 feedback, 5 record. |
| Project deep dive | 5 minutes overview, 10 demo, 20 follow-ups, 10 focused changed-case repair, 10 feedback, 5 record. |
| Combined technical | 12 minutes coding/debugging, 12 AI concepts/design, 12 project follow-ups, 9 review, 10 feedback, 5 record. |

Score five areas from 0 to 2: correctness, explanation, testing/debugging, error/access handling, and project evidence. Total: 10. Use 7/10 with no zero in correctness or error/access handling as a personal repair signal only. It is not an employer cutoff or a hiring guarantee. Record one strength, one gap and the next changed case in the final five minutes. Repeat a weak task with a changed input instead of memorizing an answer.

By the final sessions, aim to explain the document Q&A flow, make a small code change, compare outputs against a baseline, diagnose a failure, and demonstrate a focused repair. A local endpoint and relevant tests are useful evidence; describe them as local unless actually deployed. A completed checklist or simulated provider response should be labeled that way. Role eligibility, project evidence and hiring outcomes remain separate from lesson completion.

## Reference shelf

Use these only for a demonstrated gap or a selected job specialization. They are not additional assignments inside the 100 hours. Deeper MCP, durable execution, self-hosting, fine-tuning and vendor platforms stay here unless a recorded reallocation funds them.

| ID | Repository reference |
|---|---|
| 00.10 | [Terminal & Shell](phases/00-setup-and-tooling/10-terminal-and-shell/docs/en.md) |
| 00.11 | [Linux for AI](phases/00-setup-and-tooling/11-linux-for-ai/docs/en.md) |
| 01.02 | [Vectors, Matrices & Operations](phases/01-math-foundations/02-vectors-matrices-operations/docs/en.md) |
| 01.06 | [Probability and Distributions](phases/01-math-foundations/06-probability-and-distributions/docs/en.md) |
| 01.12 | [Tensor Operations](phases/01-math-foundations/12-tensor-operations/docs/en.md) |
| 01.13 | [Numerical Stability](phases/01-math-foundations/13-numerical-stability/docs/en.md) |
| 03.05 | [Loss Functions](phases/03-deep-learning-core/05-loss-functions/docs/en.md) |
| 03.06 | [Optimizers](phases/03-deep-learning-core/06-optimizers/docs/en.md) |
| 03.11 | [Introduction to PyTorch](phases/03-deep-learning-core/11-intro-to-pytorch/docs/en.md) |
| 05.01 | [Text Processing : Tokenization, Stemming, Lemmatization](phases/05-nlp-foundations-to-advanced/01-text-processing/docs/en.md) |
| 05.20 | [Structured Outputs & Constrained Decoding](phases/05-nlp-foundations-to-advanced/20-structured-outputs-constrained-decoding/docs/en.md) |
| 05.28 | [Long-Context Evaluation : NIAH, RULER, LongBench, MRCR](phases/05-nlp-foundations-to-advanced/28-long-context-evaluation/docs/en.md) |
| 10.03 | [Data Pipelines for Pre-Training](phases/10-llms-from-scratch/03-data-pipelines/docs/en.md) |
| 10.06 | [Instruction Tuning (SFT)](phases/10-llms-from-scratch/06-instruction-tuning-sft/docs/en.md) |
| 10.10 | [Evaluation: Benchmarks, Evals, LM Harness](phases/10-llms-from-scratch/10-evaluation/docs/en.md) |
| 10.11 | [Quantization: Making Models Fit](phases/10-llms-from-scratch/11-quantization/docs/en.md) |
| 10.12 | [Inference Optimization](phases/10-llms-from-scratch/12-inference-optimization/docs/en.md) |
| 11.02 | [Few-Shot, Chain-of-Thought, Tree-of-Thought](phases/11-llm-engineering/02-few-shot-cot/docs/en.md) |
| 13.02 | [Function Calling Deep Dive : OpenAI, Anthropic, Gemini](phases/13-tools-and-protocols/02-function-calling-deep-dive/docs/en.md) |
| 13.03 | [Parallel Tool Calls and Streaming with Tools](phases/13-tools-and-protocols/03-parallel-and-streaming-tool-calls/docs/en.md) |
| 13.04 | [Structured Output : JSON Schema, Pydantic, Zod, Constrained Decoding](phases/13-tools-and-protocols/04-structured-output/docs/en.md) |
| 13.10 | [MCP Resources and Prompts: Addressable Context for Stateless Servers](phases/13-tools-and-protocols/10-mcp-resources-and-prompts/docs/en.md) |
| 13.16 | [MCP Authorization: CIMD, Issuer Binding, PKCE, and Step-Up](phases/13-tools-and-protocols/16-mcp-security-oauth-2-1/docs/en.md) |
| 13.18 | [MCP Auth in Production: Issuer-Bound Enrollment and Tokens](phases/13-tools-and-protocols/18-mcp-auth-production/docs/en.md) |
| 13.28 | [MCP Tool Contracts and Content](phases/13-tools-and-protocols/28-mcp-tool-contracts-and-content/docs/en.md) |
| 13.29 | [MCP Reliability, Cancellation, and Flow Control](phases/13-tools-and-protocols/29-mcp-reliability-cancellation-and-flow-control/docs/en.md) |
| 14.06 | [Tool Use and Function Calling](phases/14-agent-engineering/06-tool-use-and-function-calling/docs/en.md) |
| 14.23 | [OpenTelemetry GenAI Semantic Conventions](phases/14-agent-engineering/23-otel-genai-conventions/docs/en.md) |
| 14.24 | [Agent Observability: Langfuse, Phoenix, Opik](phases/14-agent-engineering/24-agent-observability-platforms/docs/en.md) |
| 14.28 | [Orchestration Patterns: Supervisor, Swarm, Hierarchical](phases/14-agent-engineering/28-orchestration-patterns/docs/en.md) |
| 14.29 | [Production Runtimes: Queue, Event, Cron](phases/14-agent-engineering/29-production-runtimes/docs/en.md) |
| 14.48 | [Discover the Workflow People Actually Perform](phases/14-agent-engineering/48-discover-the-real-workflow/docs/en.md) |
| 14.49 | [Map Assumptions and Resolve the Riskiest One First](phases/14-agent-engineering/49-map-assumptions-and-risk/docs/en.md) |
| 14.50 | [Choose the Smallest Slice That Can Change the Decision](phases/14-agent-engineering/50-choose-the-smallest-testable-slice/docs/en.md) |
| 14.53 | [Choose Prototype, Pilot, or Production Deliberately](phases/14-agent-engineering/53-prototype-pilot-or-production/docs/en.md) |
| 14.54 | [Build a Feedback Ratchet with Ownership and Retirement](phases/14-agent-engineering/54-build-the-feedback-ratchet/docs/en.md) |
| 15.12 | [Long-Running Background Agents: Durable Execution](phases/15-autonomous-systems/12-durable-execution/docs/en.md) |
| 15.14 | [Kill Switches, Circuit Breakers, and Canary Tokens](phases/15-autonomous-systems/14-kill-switches-canaries/docs/en.md) |
| 15.16 | [Checkpoints and Rollback](phases/15-autonomous-systems/16-checkpoints-rollback/docs/en.md) |
| 17.15 | [Batch APIs : the 50% Discount as Industry Standard](phases/17-infrastructure-and-production/15-batch-apis/docs/en.md) |
| 17.24 | [Chaos Engineering for LLM Production](phases/17-infrastructure-and-production/24-chaos-engineering-llm/docs/en.md) |
| 17.27 | [FinOps for LLMs : Unit Economics and Multi-Tenant Attribution](phases/17-infrastructure-and-production/27-finops-llms/docs/en.md) |
| 17.28 | [Self-Hosted Serving Selection : Matching Engine to Hardware and Scale](phases/17-infrastructure-and-production/28-self-hosted-serving-selection/docs/en.md) |
| 18.20 | [Bias and Representational Harm in LLMs](phases/18-ethics-safety-alignment/20-bias-representational-harm/docs/en.md) |
| 18.26 | [Model, System, and Dataset Cards](phases/18-ethics-safety-alignment/26-model-system-dataset-cards/docs/en.md) |

For remote MCP work, study and test full authorization before exposure. This plan does not assign a remote MCP server. General Python/SQL, DSA, system design and cloud study beyond these checks remain separate.

## Reference lab limitations

These limits describe the checked-in runners. The numbered learner exercises supply the missing live/library paths where assigned; only recorded runs establish that experience.

| Lesson | Limitation |
|---|---|
| 11.01 Prompting | Model responses, token counts, and latencies are simulated; request construction can be checked, but the runner does not measure real prompt effectiveness. |
| 11.04 Embeddings and 11.06 RAG | TF-IDF vectors and exact search in memory; the RAG generator selects text heuristically. These do not establish neural embedding API, ANN index, persistent vector database, or real LLM integration experience. |
| 00.09 Data management | The full runner imports dataset libraries outside the allowlist; only relevant reading and stdlib format/version examples are assigned. |
| 13.07/13.08 MCP | Use server --demo to avoid waiting on stdin. The client uses in-process transport callables; subprocess/network transport is not demonstrated by the assigned adapter. |
| 11.10 Evaluation | Outputs and judge scores are simulated/heuristic; prompt_version labels results without changing generation in the reference runner. |
| 11.13 Production application | A simulated async request pipeline, not a deployed authenticated web service. The cache omits context/template/user scope, and the streaming wrapper collects tokens before returning. |
| 14.01 Agent loop | Scripted ToyLLM actions; the learner must connect the live model-selected tool path before claiming real agent integration. |
| 13.05 Tool schemas | A registry/schema-design linter; validating runtime arguments and enforcing permission need separate checks. |
| 14.13 Stateful graph | An in-memory stdlib implementation; it does not establish process-restart recovery or real LangGraph library experience. |
| 19.68 RAG metrics | Retrieval metric functions are real deterministic math, but its pipeline and token-overlap judge are fixtures/heuristics; use learner qrels and human-reviewed support/relevance for real-output claims. Its post-stage count is one, not two. |
| 02.09 Model evaluation | The metadata says Python but the available main is Julia; the conditional ML check uses prior coursework or a tiny Python example rather than requiring that runner. |
| 17.13 Observability | Synthetic traces/counts/retention examples, not telemetry exported from a live service. |
| 14.30 Agent evaluation | Scripted proposer/judge cases and a supplied baseline, not recorded real agent trajectories or connected CI. |

Keep one evaluation set and one lab case study across the route. Lab/code explanations should identify actual contributions, AI assistance, reference implementations, mock providers, and unimplemented work.

## Completion gates

Use saved learner artifacts and checks, not elapsed time alone. Completion means:

- One actual free model request, learned embedding request and model-selected tool call are recorded with redacted outputs; fixture/simulation runs are labeled separately.
- The same document Q&A lab runs through the local API and client, cites supplied evidence, handles insufficient evidence, and demonstrates schema, error and synthetic access-boundary checks. Any remaining real-model support failures are reported, not replaced with invented passing outputs.
- A frozen measurement contract and versioned case set distinguish retrieval metrics, answer support, relevance, abstention and fixture versus live results. At least one failure has a learner-explained fix and changed-case check.
- Chroma persistence, FastAPI validation, LCEL comparison and a bounded LangGraph trace have actual learner-run evidence, or an explicit remaining gap. Unfinished core library practice prevents a claim of full route completion.
- The learner can explain and independently change the relevant code, pass a representative fresh technical check, and describe AI assistance and deployment limits. The mock rubric guides repair; it does not predict hiring.
- The README/demo and resume bullets match the observed lab evidence. No public deployment, production authentication, durable agent recovery or large-scale performance is implied.

## Resume state

Update these fields at the end of study; they are the authoritative cursor.

| Field | Current value |
|---|---|
| Current slot | 1 / 100 |
| Slot status | not_started |
| Minutes used in current slot | 0 / 60 |
| Closed slots | 0 / 100 |
| Total study minutes used | 0 / 6000 |
| Forfeited minutes in closed short slots | 0 |
| Last study date | None recorded |
| Current task | Slot 1: environment/Python check and bounded Q&A lab contract |
| Pending next action | Ask the unhinted existing-knowledge check, then seed the corpus and write its acceptance contract |
| Learner artifact directory | learning-artifacts/ai-engineering/ (create when study begins) |
| Last runnable evidence | None recorded |
| Provider access and live gates | Not yet verified |
| Displaced work | None |

On closing an hour, increment Closed slots, advance Current slot, reset open-slot minutes to 0 and set the next slot to `not_started`. `Current slot` advances only when its hour closes; `Closed slots` plus the open slot's allowance controls the remaining budget. Total used plus forfeited minutes equals 60 times closed slots plus minutes used in the open slot. After closing slot 100, set Current slot to `budget_exhausted` and open-slot minutes to 0. Stop and report passed gates and remaining gaps; the Progress log retains the final slot's evidence.

## Progress log

No task is completed merely by appearing in the plan. Append continuation entries for an interrupted slot; sum their minutes rather than counting a second hour.

| Date | Slot / work row IDs | Minutes this entry / slot state | Task outcome and unhinted check / quiz N/M | Learner artifact / command / result / live or fixture | Pending action / displaced work |
|---|---|---|---|---|---|

## Review queue

| Lesson / question / gate | Specific gap and prerequisite it blocks | Changed-case retest | Allocated repair slot or displaced row | Status |
|---|---|---|---|---|

## Earlier placement record

The 2026-09-28 placement recorded 9/10: Math & Statistics 1/2; Classical ML, Deep Learning, NLP & Transformers, Applied AI each 2/2. This is history, not proof of mastery. This personal 100-hour route replaces the earlier 112-hour schedule. No completed lessons or study time have been inferred from that placement.

## After the 100 hours

The additional repository lessons are in [LEARNING-AFTER-100.md](LEARNING-AFTER-100.md), a separate 40-hour follow-on plan. After closing these 100 hours, the next `learn` invocation selects that plan. Its schedule, completion checks and progress record are separate; closing slot 100 still ends the current session.
