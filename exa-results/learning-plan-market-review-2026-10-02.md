# Evidence for the personal 100-hour AI engineering plan

Checked 2026-10-02. This is a research note and allocation proposal, not a replacement for LEARNING.md or a list of confirmed vacancies.

The learner's agreed direction is junior/fresher LLM application engineering and basic agents, targeting India and remote employers that can hire someone based in India. The budget is 100 one-hour sessions, with no fixed completion date and free provider access only. New topics start with a worked example, followed by a learner-owned change. Revision starts with an unhinted check; a failure gets focused repair and a changed-case retest. The continuing lab is a document Q&A assistant over a small public or synthetic corpus. Tessera, degree work, DSA, and AWS preparation remain separate workloads.

## Research method and boundaries

Three research agents used Exa MCP for fresher/internship discovery, junior-role discovery, and India-eligible remote discovery. Exa Agent handled broad discovery; direct Exa search and page retrieval, plus browser checks of employer/ATS pages, checked the evidence. The fresher pass used two structured runs, the junior pass one, and the remote pass one. Requested direct-search result slots are a discovery metric, not a count of independently verified employers.

After deduplication, 17 employer descriptions not known to be unavailable were retained for the curriculum comparison. Their individual vacancy status is often unconfirmed. Six other descriptions have unavailable or closed primary pages, and are archived below. Restricted cohorts, a contest program, uncertain eligibility, and broader ownership roles are separate evidence. The original five employers in LEARNING.md are not the basis of the numerical table.

This is best-effort discovery, not an exhaustive market survey. Searches deliberately targeted LLM application work, so the sample cannot establish how common LLM requirements are across all AI jobs. Employers with searchable English careers pages and startups are easier to discover. An internship title alone does not establish that a candidate meets its degree, enrollment, location, or project requirements.

Required qualifications, responsibilities, and explicitly preferred skills are recorded separately. A duty is evidence of work the candidate should prepare for; it is not automatically a prior-experience hiring requirement. General LLM familiarity does not establish provider API experience. LLM orchestration libraries are separated from ML/data libraries. An accessible description does not prove an open vacancy.

## What the comparable junior descriptions say

This count table uses the 11-description junior cohort: CorroHealth, Anteriad, Soothsayer Analytics, L&T, RevRag AI, Brainwonders, Mobio Solutions, NeuLeap, HCLTech, Valura, and Drivetrain. Atlys and Dun & Bradstreet were removed from its original 13-description cohort after browser checks found their primary pages unavailable. Each employer counts once per column. Columns overlap: a skill can appear in both qualifications and duties, or at different levels in the same description.

These categories are research coding of the descriptions, not employer-defined standardized skill labels. Evaluation includes testing or comparing model/application behavior; it does not always mean an LLM judge. API/backend includes REST, microservices, and integrating applications. Git/testing combines collaboration and testing evidence. Read the individual descriptions when choosing a particular job.

| Skill category | Required qualifications | Responsibilities | Either required or a duty | Explicit preferences |
|---|---:|---:|---:|---:|
| Python | 9/11 | 3/11 | 9/11 | 0/11 |
| API/backend integration | 5/11 | 7/11 | 8/11 | 4/11 |
| Explicit LLM provider/API integration | 2/11 | 2/11 | 4/11 | 1/11 |
| Prompting or structured outputs | 5/11 | 6/11 | 9/11 | 0/11 |
| RAG | 4/11 | 8/11 | 8/11 | 3/11 |
| LLM framework libraries | 5/11 | 3/11 | 6/11 | 2/11 |
| Evaluation/testing of model or application behavior | 2/11 | 8/11 | 9/11 | 2/11 |
| Docker/cloud | 3/11 | 4/11 | 6/11 | 6/11 |
| Fine-tuning or model serving | 0/11 | 3/11 | 3/11 | 2/11 |

The five browser-accessible descriptions in the fresher pass are Drivetrain, NeuLeap, Abstrabit, DigitalXnode, and White Collar Realty. Two overlap with the junior cohort, so these counts must not be added together. In this small fresher cohort, RAG appears in duties in 5/5, evaluation/testing in 4/5, and agent workflows in 3/5. Named LLM API experience is not an explicit required qualification in these five, although some duties involve integrating models or APIs. Model-serving APIs and hosted-provider APIs are different evidence. [Drivetrain](https://jobs.lever.co/drivetrain/bc1c17bc-86ac-4f00-a1e3-0eb85aae4fdc), [NeuLeap](https://neuleap.ai/careers/4), [Abstrabit](https://jobs.smartrecruiters.com/abstrabittechnologiespvtltd/744000150288970), [DigitalXnode](https://digitalxnode.com/jobs/ai-ml-internship-llm-rag-agentic-ai-real-projects-apply-now/), [White Collar Realty](https://whitecollarrealty.com/career/llm-intern).

## Curriculum implications

The core should make the learner implement and explain a small application: Python and HTTP/JSON, model request/response handling, prompting and output validation, ingestion and retrieval, evidence-grounded generation, evaluation, and debugging. CorroHealth explicitly asks for LLM API experience alongside Python, REST, Git, and basic NLP. NeuLeap assigns LLM API and RAG work while accepting internships/projects in its 0-2-year range. These support a real integration requirement without relying on one employer. [CorroHealth](https://corrohealth.wd1.myworkdayjobs.com/en-US/CorroHealthIndia/job/Junior-AI---Engineer_JR104988), [NeuLeap](https://neuleap.ai/careers/4).

Evaluation belongs throughout the route. RevRag asks interns to test behavior, inspect edge cases, and improve response quality; Abstrabit assigns evaluation datasets, reproducible experiments, and failure investigation. The lab should retain unchanged cases, compare a baseline with a controlled change, and separately assess retrieval relevance and whether the answer is supported. [RevRag AI](https://www.revrag.ai/careers/ai-engineer-intern), [Abstrabit](https://jobs.smartrecruiters.com/abstrabittechnologiespvtltd/744000150288970).

Project evidence matters even for some internships. Drivetrain asks for demonstrated end-to-end projects; HCLTech names hands-on project portfolios; Abstrabit accepts meaningful projects through coursework or other practical work. One integrated learner lab can provide code and explanation evidence, while its deployment status and AI assistance still need clear attribution. [Drivetrain](https://jobs.lever.co/drivetrain/bc1c17bc-86ac-4f00-a1e3-0eb85aae4fdc), [HCLTech](https://careers.hcltech.com/job/Platform-Engineer-I/126027-en_US), [Abstrabit](https://jobs.smartrecruiters.com/abstrabittechnologiespvtltd/744000150288970).

Python, SQL, Git, ML fundamentals, and Docker knowledge can be credited when demonstrated. Credit should come from a small relevant task or explanation, rather than a course name or the historical ten-question placement score. DSA remains a separate workload, but ordinary collection handling, complexity, and debugging still belong in this route. Drivetrain explicitly asks for DSA and system-design fundamentals; that responsibility cannot be generalized away from one low mention count. [Soothsayer Analytics](https://soothsayeranalytics.com/careers/ai-intern-hyderabad), [Drivetrain](https://jobs.lever.co/drivetrain/bc1c17bc-86ac-4f00-a1e3-0eb85aae4fdc).

LLM frameworks should not automatically be called an extra. Anteriad explicitly requires experience with LangChain/LangGraph and FastAPI or Flask; Mobio also lists framework experience. The repository's dependency policy excludes those Python libraries. The learner subsequently approved a narrow exception for personal work: the final route adds bounded library exercises after scratch equivalents while checked-in lesson code retains the repository contract. [Anteriad](https://job-boards.greenhouse.io/anteriad/jobs/5386350004), [Mobio Solutions](https://mobiosolutions.freshteam.com/jobs/8O8aIBiTdyF-/generative-ai-engineer), [repository dependency policy](../AGENTS.md).

Some skills change level by employer. RevRag puts provider APIs, vector databases, and cloud exposure under preferences. Anteriad assigns cloud deployment as a duty, and other descriptions require some cloud knowledge. The plan should include basic packaging, configuration, logs, secrets, and failure handling, then use specific target jobs to decide deeper stack work. Fine-tuning/self-hosting, advanced routing and rollout infrastructure, broad vendor surveys, and protocol specialization should not displace a working core application. This prioritization follows the learner's goal and time budget; it does not mean those skills are optional in all jobs. [RevRag AI](https://www.revrag.ai/careers/ai-engineer-intern), [Anteriad](https://job-boards.greenhouse.io/anteriad/jobs/5386350004).

## Source ledger: 17 curriculum-comparison employers

Status below means a description was accessible or not known unavailable during the check, not a guarantee that applications are being accepted. Experience bands and internship eligibility remain separate. Movate's 1-3-year minimum is a stretch for a fresher; WonderBotz's 0-3 range includes zero experience. Neither is presented as an explicit 0-2-year posting.

| Employer / primary description | Experience / location | Relevant evidence and caveat |
|---|---|---|
| [CorroHealth](https://corrohealth.wd1.myworkdayjobs.com/en-US/CorroHealthIndia/job/Junior-AI---Engineer_JR104988) | 0-2 years; Noida | Python, hosted LLM APIs, REST/Git, ML/NLP basics; cloud and personal projects preferred. Hiring status unconfirmed. |
| [Anteriad](https://job-boards.greenhouse.io/anteriad/jobs/5386350004) | 1-2 years; Bangalore | Production LLM/RAG application and framework experience; cloud duties. Architecture scope is demanding for this plan. |
| [Soothsayer Analytics](https://soothsayeranalytics.com/careers/ai-intern-hyderabad) | 0-1 years; Hyderabad internship | Python, SQL/Git, ML basics, prompting; RAG/framework experimentation with mentorship. Enrollment requirements apply. |
| [L&T](https://larsentoubrocareers.peoplestrong.com/job/detail/LNT_GT_1820286) | 0-2 years; Powai trainee | Model/application work, prompt evaluation, RAG and deployment duties. Lists BTech and MTech; BS eligibility must not be assumed. |
| [RevRag AI](https://www.revrag.ai/careers/ai-engineer-intern) | Six-month internship; Bengaluru onsite | Python/API basics, prompt testing, response evaluation; provider APIs and vectors preferred. |
| [Brainwonders](https://jobs.smartrecruiters.com/Brainwonders/744000145653189-ai-intern-) | 0-1 years/freshers; Mumbai onsite | Agents, RAG, frameworks, AWS and evaluation. Broad scope despite internship title; 2026 graduate wording needs checking. |
| [Mobio Solutions](https://mobiosolutions.freshteam.com/jobs/8O8aIBiTdyF-/generative-ai-engineer) | 1-2 years; India | LLM/API, Python, RAG/vector, framework and backend work. Application visible; vacancy status unconfirmed. |
| [NeuLeap](https://neuleap.ai/careers/4) | 0-2 years; Pune | Internships/projects count; LLM APIs, RAG and model evaluation. Framework/cloud exposure can be preferred. |
| [HCLTech](https://careers.hcltech.com/job/Platform-Engineer-I/126027-en_US) | Zero years; graduate role | Project portfolio, Python, ML/NLP, framework/vector and SQL knowledge. Graduate timing and qualifications apply. |
| [Valura](https://careers.valura.ai/13ea5e17-ea6e-427d-ae37-0831cfdb8699) | Zero years; GIFT City / remote stated | API, Python, framework/vector and evaluation work. Page lists an unusual 36-month internship; verify before applying. |
| [Drivetrain](https://jobs.lever.co/drivetrain/bc1c17bc-86ac-4f00-a1e3-0eb85aae4fdc) | Internship; India | RAG/agent concepts, DSA, end-to-end project evidence; frameworks/cloud/API exposure preferred. Exact remote arrangement needs confirmation. |
| [Abstrabit](https://jobs.smartrecruiters.com/abstrabittechnologiespvtltd/744000150288970) | Internship; Bengaluru | Python/API/Git fundamentals and meaningful project; inference, RAG, evaluation and production-facing duties. No prior professional experience stated. |
| [DigitalXnode](https://digitalxnode.com/jobs/ai-ml-internship-llm-rag-agentic-ai-real-projects-apply-now/) | 0-1 years; Delhi onsite | RAG/agent/API integration duties; framework names preferred. June 2026 page remains; current vacancy unconfirmed. |
| [White Collar Realty](https://whitecollarrealty.com/career/llm-intern) | Students/freshers; Gurgaon onsite | Prompt/RAG/output evaluation in applied workflows. Page says two openings; unpaid internship, Python can be preferred. |
| [Movate](https://www.movate.com/jobs/ai-engineer-junior/) | 1-3 years; Bangalore/Chennai/Pune | LLM APIs, prompting, RAG, agents and evaluation. One-year minimum makes it a stretch for a fresher. |
| [WonderBotz](https://wonderbotz.applytojob.com/apply/RbPIL43iH6/Junior-AI-Engineer) | 0-3 years; Ahmedabad | Python/REST, cloud, Git/CI, LLM/RAG and agent/vector work. Its location is not worldwide remote. |
| [SwarmLens](https://swarmlens.com/jobs/ai-engineer-junior-ai-engineer/) | 1-2 years; Kochi | RAG, prompting, agents and evaluation. November 2025 description; current vacancy unconfirmed. |

## Archived, restricted, and other evidence

| Primary source | Why it is separate |
|---|---|
| [Mactores](https://jobs.lever.co/mactores/6ba73d45-b772-455b-92d2-b42544b3f729) | Browser returned 404 although another extraction/application check retained details. Conservatively archived; supervised Python, agent/retrieval/evaluation work and cloud foundations remain historical demand evidence. |
| [Atlys](https://jobs.ashbyhq.com/atlys/1a34deb8-3d14-4b7b-b1eb-cd302ce97223) | Browser said job not found. Cached conversational-AI build and evaluation requirements are archival only. |
| [Dun & Bradstreet](https://jobs.lever.co/dnb/f4e8ccf6-9d44-4bdf-9ed9-023c67cae440) | Browser returned 404. Cached agent/framework/cloud requirements are archival; internship title includes unusually broad ownership duties. |
| [Endpoint Clinical](https://jobs.lever.co/endpointclinical/820b0188-3545-4b1f-8624-56592b85f898) | Browser returned 404. Cached prompt-testing and business-workflow internship description is archival. |
| [Epifi](https://jobs.lever.co/epifi/4f5b7548-ea0a-4be0-816b-11d712853169) | Browser returned 404. Cached product-build/portfolio requirement is archival. |
| [ProArch](https://apply.workable.com/j/FC18E04C2D) | Page explicitly said no longer available. Its preferred stack is not a current application opportunity. |
| [Atlan](https://intern.at.atlan.com/) | Referral-only cohort; August referral deadline and September 2026 start have passed. BTech/graduation/NOC conditions apply. |
| [Sarvam AI](https://careers.kula.ai/sarvam-ai/17986/apply?applySuccess=true) | 1-3 years and customer-facing build assignment; stretch evidence, not a fresher baseline. URL parameter does not prove an application occurred. |
| [Fello](https://ats.rippling.com/fello-careers/jobs/c0748edd-5d3d-4e0c-95ba-6c2d8e7aabb4) | Explicit India remote, but expects previous builds and end-to-end ownership; not a verified junior opening. |
| [Gnani AI](https://www.gnani.ai/internship) | Student challenge/program with a dated October-November window and project-selection process; not a conventional vacancy or an assigned course task. |
| [Neural City](https://www.neuralcity.in/applied-genai-intern) | Browser navigation failed and remote applicant-country eligibility was not established. |
| [IQVIA](https://jobs.iqvia.com/en/jobs/R1566902-0) | Browser navigation failed; cached India internship details do not establish current acceptance. |

The global pass did not verify an explicitly worldwide-remote junior LLM application role. It found India-eligible remote descriptions and broader roles, plus country-restricted or more experienced alternatives. A worldwide opportunity may exist outside this sample. Do not present US-only, Europe-only, or Americas-only remote positions as eligible for an India-based applicant. International remote eligibility needs a fresh employer check when applying.

## Free live-model practice

Generation/embedding REST documentation and free pricing were rechecked through Exa on 2026-10-03 while finalizing the schedule. [Generation](https://ai.google.dev/gemini-api/docs/text-generation), [embeddings](https://ai.google.dev/gemini-api/docs/embeddings), [pricing](https://ai.google.dev/gemini-api/docs/pricing).

Google's current documentation lists free text generation and free embedding access; India is supported. Free-tier quotas and available models depend on the account and can change. The first API session should check account access and demonstrate one successful request before later work depends on it. Keep provider selection and model identifiers dated; do not promise a fixed quota for the full course. [Gemini pricing](https://ai.google.dev/gemini-api/docs/pricing), [available regions](https://ai.google.dev/gemini-api/docs/available-regions), [rate limits](https://ai.google.dev/gemini-api/docs/rate-limits).

The free tier's pricing page says content can be used to improve products. The assigned corpus should therefore be public or synthetic. Cache embeddings and saved successful outputs for repeatable local tests; label fixture-based runs separately. A replayed fixture is useful for deterministic error tests but does not count as a fresh live integration. Public deployment or unrestricted traffic is a separate decision from being able to call a real model locally.

## Decisions incorporated into the learning plan

After reviewing these findings, the learner accepted a 100-hour route with no fixed deadline, a continuing document Q&A lab, free provider access only and a small local HTTP API. Paid internships/trainee roles and junior full-time work are the application targets; unpaid descriptions remain supplementary research evidence.

The final [LEARNING.md](../LEARNING.md) owns the numbered schedule and budget. It includes scratch-first Chroma, FastAPI/Uvicorn, LangChain LCEL and LangGraph exercises in an isolated learner copy, twelve distributed recall/repair hours, and two hours for README/demo/evaluation evidence and accurate resume bullets. Applications themselves stay outside study time. The source ledger above remains research checked on 2026-10-02; this decision note was updated on 2026-10-03.

Fresh-session routing now points to the plan's tutor contract and saved cursor in [AGENTS.md](../AGENTS.md) and [the learn skill](../skills/learn/SKILL.md). Missed days leave the cursor intact. Failed checks require focused repair and a changed-case retest, with cuts recorded inside the same budget. The checked-in simulations are not counted as live provider or framework experience.
