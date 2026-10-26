# PROPOSED — Verify a Local-First Workflow Before Replacing Subscriptions

**Status:** PROPOSED educational workflow  
**Prepared and source-checked:** October 25, 2026  
**Evidence level:** Documentation and selected source inspection; no learner hardware benchmark or completed migration is demonstrated by this artifact.  
**Purpose:** Help a learner reduce unnecessary service dependence through useful project work, measured costs, recoverability, and lawful deployment choices.

Read the repository [disclaimer](../DISCLAIMER.md). Tool capabilities, licenses, prices and legal requirements change; date and verify consequential claims.

## Capability to develop

Given an existing project and equipment, the learner can identify its external dependencies, reproduce one useful task without them where feasible, restore the result, measure the tradeoffs, and justify a service decision using evidence.

The outcome is a tested capability. Installing software, downloading a model, or receiving a polished AI-generated plan does not demonstrate that capability.

## 1. Separate the independence questions

| Property | Question to answer | Evidence |
| --- | --- | --- |
| Local ownership | Can the learner access and export authoritative work without the original provider? | Readable source files, original assets and completed data exports. |
| Offline operation | Does the selected task start, finish, save and reopen with WAN unavailable? | Dated restart and task result, with remaining dependencies listed. |
| Self-hosting | Can the service and its data move to another compatible host? | Versioned configuration and a demonstrated recovery or migration. |
| Energy autonomy | Can the actual devices operate and recharge for the intended interval? | Device-specific measurements and an appropriate existing power path. |
| Legal deployment | Is the intended activity permitted under applicable rules and contracts? | Current primary sources, jurisdiction, covered activity and effective dates. |

These properties vary independently. A local web interface may call a cloud model. Local inference does not supply fresh web search while disconnected. A battery-powered server still needs an upstream network for remote users. Treat public delivery as a separate dependency from local content production.

## 2. Give humans and AI different responsibilities

| AI may assist with | Learner must demonstrate |
| --- | --- |
| Draft a dependency inventory or compare documentation | Identify the actual installed environment and correct unsupported assumptions. |
| Suggest test cases and explain errors | Explain the data/request path and choose meaningful success criteria. |
| Draft a migration plan or propose changes | Protect original data, authorize consequential actions and inspect results. |
| Summarize measurements and sources | Reproduce the calculation, verify important claims and justify the decision. |

Keep the private equipment inventory, billing, credentials and unpublished project data out of public exercise submissions. A sanitized result can teach the method without exposing the working environment.

## 3. Establish a small baseline

Choose one task that already matters: a documentation update, a software build, a narration, an image export or a short video edit. Use existing equipment before choosing new products.

Record the host OS, CPU, RAM, GPU/VRAM where relevant, free disk, software versions, model/configuration, input data owner and output destination. Distinguish owned-and-accessible hardware from borrowed or rented compute. A cloud GPU used previously does not establish a local GPU capability.

Use clear states: **reported**, **observed**, **source-documented**, **tested for this task**, **proposed**, and **unknown**. A feature described in a README remains source-documented until it is exercised in the actual environment.

## 4. Protect and restore before changing the workflow

Identify the authoritative working copy. Protect the selected source, assets, configuration and completed application-data exports on a separate physical destination. Restore into a clean location and inspect or build the restored project.

Git history, synchronization, replication and versioned backup serve different purposes. A repository may omit unsaved buffers, ignored files, large assets and application databases. A second folder on the same failing device does not protect against that device's loss. Copying live database files is not a universally consistent backup method; use the application's documented export/backup process.

Preserve the prior working installation and a rollback path. Test new tools on copied inputs until their behavior is understood. Keep secrets out of project commits, reusable prompts, screenshots and ordinary public exports.

## 5. Classify candidate tools by their actual path

The following examples were checked against upstream documentation on the date above. They are candidates rather than endorsements, installed configurations or evidence of parity with paid products. Read application, model, dependency and output terms separately. Repository links in the table identify inspected README snapshots; they are not recommended release pins.

| Candidate | Documented use | Dependency or limitation to verify |
| --- | --- | --- |
| [VoiceStudio](https://github.com/debpalash/VoiceStudio/blob/ac390561174372322cf44c1375bbdd344ddc8bd1/README.md) | Local voice/TTS and related audio workflows | CPU speed and selected engines vary; translation or remote features may add services. AGPL application terms do not settle model/voice rights. |
| [Odysseus](https://github.com/odysseus-dev/odysseus/blob/9d0d3720f4ca181d87bef94da826d730acc6d483/README.md) | Local/API assistant workspace | Research and integrations remain network-dependent. Default `dev` and more curated `main` are different baselines; evaluate a tested immutable build. |
| [FreeLLMAPI](https://github.com/tashfeenahmed/freellmapi/blob/5646971602a89436ce4921b0f04b99ac7bcc3728/README.md) | Route requests across remote free tiers or configured custom endpoints | Remote routing still sends data upstream and depends on provider terms/quotas. The project describes the free-tier approach as experimentation rather than production infrastructure. |
| [Vane](https://github.com/ItzCrazyKns/Vane/blob/348feca3e378fb4157b217724ed508dc707f853f/README.md) | Research frontend with local model support | Internet search through SearxNG remains online; local history and fresh results are different capabilities. |
| [InvokeAI](https://github.com/invoke-ai/InvokeAI/blob/6af20578bce65177ff9da43df0e82c788a2e14ae/README.md) | Local image generation and editing | Model/resolution-specific RAM, GPU and storage requirements; optional external models remain remote. Compare with existing tools before adding another manager. |
| [ACE-Step 1.5](https://github.com/ace-step/ACE-Step-1.5/blob/ca1e85fe9430179831e6bc6be790c332190a3866/README.md) | Local music generation | Small/offloaded and XL configurations have different resource needs. CPU availability does not establish useful speed or production quality. |
| [OpenShorts](https://github.com/mutonby/openshorts/blob/baf66a1fa327ecbde384334544a2df579317d0f9/README.md) | Local transcript-based clipping through a compatible model endpoint | Some visual analysis, generated media, dubbing and posting retain external services. MIT core and optional `cloud/` licensing differ. Export retained results explicitly. |
| [Dyad](https://github.com/dyad-sh/dyad/blob/1be2b4b6d2c70a4550db7b96e26fc75c50bf5bc0/README.md) | App-building with local model options | Linux support is documented as experimental; generated applications may still require hosted services. Licensing differs inside `src/pro`. |
| [OpenManus](https://github.com/FoundationAgents/OpenManus/blob/3309bf4e416fb1c74b008f3e86494439a31bad53/README.md) | Agent framework with a documented Ollama configuration | Tool/model behavior and permissions require testing. Browsing needs connectivity; framework installation does not demonstrate safe autonomous execution. |
| [Upscayl](https://github.com/upscayl/upscayl/blob/a00d55fee90e0f9435d5eaa86e76700df8199af8/README.md) | Bounded local image upscaling | Vulkan-compatible GPU required. Inspect lettering, lineart and faces; estimated detail is not proof of authentic missing detail. |

For a selected candidate, record the exact release/commit, source URL, required downloads, model license, provider endpoints, optional cloud switches, expected output and data-retention behavior. Cache the installers, dependencies, models and documentation needed for that task where permitted. An entire model library or package registry is not required to prove one useful workflow.

Ollama's [official FAQ](https://docs.ollama.com/faq) documents local-only mode through `OLLAMA_NO_CLOUD=1`, a restart and a log confirmation; it binds its API to localhost by default. That is one runtime option, not a requirement. Configuration is evidence to inspect, and the complete client workflow still needs testing.

## 6. Run one useful offline proof

Prepare required dependencies while connected. With work protected and the relevant devices available, test WAN unavailability while retaining a local connection if the task needs it. Restart the selected app, perform the task, save/export the result and reopen it. Repeat after a suitable host restart when practical.

Record whether startup requires a login, model download, package fetch, remote asset, cloud fallback or license check. Check whether the chosen provider setting applies to all relevant components, including embeddings, transcription, translation or vision. A successful connected request can conceal dependencies that appear only after restart or cache expiry.

Use task-specific quality criteria selected beforehand:

- **Code:** the intended change and existing relevant checks succeed; unrelated files remain intact.
- **Voice:** authorized inputs, understandable pronunciation and acceptable consistency; exported audio reopens.
- **Images:** useful output without unacceptable invented markings, altered lettering or damaged subject details.
- **Music:** acceptable musical result with reviewed inputs and preserved audio/configuration.
- **Video:** correct cuts/captions, retained masters and an exported clip that survives application cleanup.

If the task fails, keep the evidence and identify the smallest failing dependency. Retry a scoped correction rather than adding several frameworks at once. A manual export or ordinary editor can be a valid continuity path while an AI feature is unavailable.

## 7. Measure complete costs

Record actual billing and renewal terms before claiming subscription savings. Separate current cash savings, avoided future renewals and sunk annual payments. Track remaining remote/API costs and the human time needed to maintain the local option.

`Monthly cash saving = avoided bill − incremental power − remaining API/hosting − incremental backup/maintenance.`

Fictional example: avoiding $24/month while adding $4/month in recurring costs yields $20/month before valuing time. A later $200 purchase would take ten such months to recover its acquisition cost, before other costs or failures. These are teaching inputs, not product prices or an investment recommendation.

Use **W** for power and **Wh** for energy:

`Energy (Wh) = average power (W) × operating hours.`

An illustrative 15 W always-on load uses 360 Wh/day. Measure the full relevant host, storage, display, network and charging path; do not infer wall power from a CPU/GPU label. Phone battery percentage can support an observation but is not calibrated total system energy, especially while charging.

Compare running a heavy service only when needed with leaving it resident continuously. Keep useful work, runtime, memory, temperature and energy in the same record. Equipment sizing, permanent electrical work and household backup design require their own applicable technical and local review.

## 8. Check legal claims without assuming a universal ban or exemption

Start with the actual jurisdiction and activity. Separate model operation, model development, public/commercial deployment, chip export, electrical installation, property occupancy, water/sewer requirements and carrier contracts. Record an official identifier, current status, covered actor/activity, threshold, effective date and any unresolved interpretation.

The following examples illustrate the classification method as checked October 25, 2026:

| Primary record | What the checked record establishes | Limit on the conclusion |
| --- | --- | --- |
| [NYC Int. 1100-2026](https://legistar.council.nyc.gov/LegislationDetail.aspx?GUID=A927E066-C669-4F66-8E5A-4B610FA321E5&ID=8239233) | Committee-stage proposal concerning AI validation and human-operated shutdown capability. | Broad deployment wording needs review; private/offline use is not an assumed exemption. This record does not establish enacted nationwide law. |
| [California SB 1047 veto](https://www.gov.ca.gov/2024/09/29/governor-newsom-announces-new-initiatives-to-advance-safe-and-responsible-ai-protect-californians/) and [SB 53 signing](https://www.gov.ca.gov/2025/09/29/governor-newsom-signs-sb-53-advancing-californias-world-leading-artificial-intelligence-industry/) | Different measures with different outcomes: a 2024 veto and a 2025 frontier-developer law. | Do not combine old proposals and enacted obligations into a generic local-computing prohibition. |
| [CBO analysis of H.R. 3447](https://www.cbo.gov/publication/62310) | May 2026 analysis of an advanced-chip export-security proposal. | Analysis of a proposal does not establish current enactment or a universal consumer-GPU restriction; the retrieved action records had a freshness gap. |
| [Santa Cruz County off-grid solar route](https://cdi.santacruzcountyca.gov/UPC/BuildingPermitsSafety/ApplyforaBuildingPermit/Solar(PV)SystemBatteryPermits/Off-GridSolarDesign.aspx) | An explicit local design/permit route for off-grid systems. | It does not grant permission for another parcel or jurisdiction. |
| [Bedford archived sewer notice](https://bedfordny.gov/CivicAlerts.asp?AID=279&ARC=977) | A 2025 district-specific mandatory connection notice. | An archived example is not current property advice; sanitation and electrical autonomy are separate. |

Treat unresolved scope or stale records as an open dependency. Recheck primary sources before affected purchases or public deployment. A pending bill, an enacted law, a private service contract and a technical limitation require different responses.

Prepare lawful continuity: replace or disable an affected feature, use an applicable permitted/compliant path, retain required connections, or evaluate a genuine lawful operating arrangement. Modular architecture makes adaptation easier but creates no legal exemption. A VPN, changed label or old download does not establish different jurisdiction or grandfathered permission. This exercise teaches source evaluation rather than a conclusion for an unidentified property or business.

## 9. Decide, preserve and review

Choose **retain**, **reduce**, **replace**, or **defer** for the actual service. Tie the choice to quality, recurring cost, recovery and the tasks performed. A free application can still be unsuitable; a limited paid fallback can still be a deliberate decision.

For a later purchase, write the observed failure, required capability, complete acquisition/operating cost, available budget, migration/rollback method and continuing use for old equipment. Revenue projections alone do not establish money available today.

### Compact evidence record

| Field | Learner's record |
| --- | --- |
| Real project/task and success criteria | Record privately; submit only sanitized details. |
| Installed versions, candidate and model/configuration | Include a stable reference and relevant license. |
| Network/dependency path | Name local, remote, optional and unknown components. |
| Backup and actual restore result | Record destination class and outcome without exposing secrets. |
| Offline startup/task/export/reopen result | Date, observed result and failures. |
| Quality, runtime, storage and power observations | Distinguish measurements from estimates. |
| Recurring cost and maintenance comparison | Use actual private billing or clearly fictional public figures. |
| Legal/contract dependency | Primary source, jurisdiction, status, review date and unresolved scope. |
| Decision and remaining learning debt | State what is proven and what still needs work. |

## 10. Explain, reproduce, adapt and teach

Use the completed task for a [live-project assessment](../assessment/live-project-assessment.md). The learner should explain the complete request/data path, reproduce one successful operation, diagnose an observed failure, justify the service decision and demonstrate recovery. Record which parts were AI-generated, learner-observed, learner-explained and independently reproduced.

Useful explain-back prompts:

1. Which part of this workflow still requires an outside provider, and how was that determined?
2. What does the restore protect that a successful Git push does not establish?
3. Which claim came only from documentation, and what test would strengthen it?
4. How would work continue if the selected model, provider or deployment became unavailable?

For a prompt-from-knowledge exercise, the learner writes the next scoped request using the objective, actual environment, known dependencies, private-data boundary, budget, acceptance checks and allowed AI actions. AI may critique the draft but should not secretly author the learner's assessed final prompt.

After demonstrated assessment, a [challenge](../challenge/live-project-challenge.md) can extend the same real project to a second environment or replacement tool. Agree a fair deadline and assistance limits first. Require the learner-authored advanced prompt and finished useful deliverable, and evaluate knowledge, product quality and workflow discipline separately.

Finish with a short teach-back showing the dependency map, one failed assumption, the verification result and the resulting decision. If slides help, use: problem → independence properties → dependency map → one trial → failure/correction → cost evidence → recovery → decision → learning debt. A text walkthrough is sufficient.

### Learning debt to preserve

This document establishes no installed service, measured savings, power runtime, legal determination, production uptime or learner mastery. A successful first task also leaves long-session stability, update recovery, complete backup coverage and unfamiliar failure diagnosis untested until demonstrated. Keep those gaps visible rather than converting documentation into claims of completion.

## Related resources

- [Verified Agent Evolution](verified-agent-evolution.md) — developing bounded local capabilities once their procedures are understood.
- [Evolving Local Agents Without Model Dependence](../docs/lessons/evolving-local-agents-without-model-dependence.md) — local knowledge, procedures and optional inference.
- [Portable AI Memory Foundations](../docs/lessons/portable-ai-memory-foundations.md) — provider-independent context and provenance.
- [Assessment learning debt](../assessment/learning-debt.md) — keeping untested understanding visible.

