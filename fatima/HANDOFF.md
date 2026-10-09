# Fatima: coordination

Status: Chapters 3 and 5 drafted on 5 October 2026 for Fatima's assigned report work. Abstract remains template/unfinished.

## Completed work

Chapter 3 now replaces the template examples with Zeest-specific related work. It reviews clinical decision support and EMR systems, medical and biomedical language models, imaging and multimodal learning, retrieval/evidence grounding, agentic orchestration, and candidate datasets/synthetic cases. The chapter includes a summary table with 17 relevant reviewed items.

Chapter 5 now describes the proposed methodology as a planned R&D procedure. It covers case preparation, hybrid memory, the proposed agent pipeline, dataset/model/resource register, evidence retrieval, planned ablation protocol and methodological traceability to Chapter 2 objectives and Chapter 4 requirements. The user requested sample-style numbered headings in Chapter 5, so numbered sections were added for readability while keeping the same methodology content.

## Decisions and stable IDs

Fatima citation keys use the `zeestB:` prefix. Chapter 3 also cites Kashaf-owned shared keys `zeestA:noriMedical`, `zeestA:rag` and `zeestA:mimicIV` where those sources were already present in the shared bibliography flow.

New diagram sources:

- `diagrams/fatima_D04_method_pipeline.puml`
- `diagrams/fatima_D05_ablation_protocol.puml`
- `diagrams/fatima_D06_evidence_retrieval.puml`

Rendered report assets:

- `../Report template/Figures/fatima_D04_method_pipeline.png`
- `../Report template/Figures/fatima_D05_ablation_protocol.png`
- `../Report template/Figures/fatima_D06_evidence_retrieval.png`

The PNG diagrams were generated locally as static report assets because the environment blocked downloading PlantUML after the usage/approval limit was reached. The `.puml` files remain the editable source of record and can be re-rendered later with PlantUML if desired.

## Dependencies and open questions

The prototype is unbuilt. Chapter 5 now keeps planned implementation, resource selection, retrieval evaluation and input validation in normal prose after the user requested removal of the red planned text from Chapter 5. No results, dataset access, clinical deployment or model integration are claimed.

Unresolved dependencies remain: clinical domain, final dataset access, selected imaging classifier, transcription component, embedding model, evidence corpus, medication knowledge resource, LLM configuration, LangGraph/ADK responsibility split, reference judgement process, reviewer roles, sample size, scoring rubric and numeric thresholds.

Esha should align Chapter 6 to the current Chapter 4 requirement IDs and to the Chapter 5 processing responsibilities. Kashaf's Chapter 4 now uses FR01 through FR38 and RR01 through RR04; Chapter 5 traces methodology stages to those current IDs.

## Approved current assignment

Chapters 3 and 5; Abstract. All owners maintain their own references. Current submission is six-chapter R&D Deliverable II; Chapters 7 through 10 are excluded. No other owner files, shared assembly files, class files or root documentation were edited during this work.

## Approved final integration, 10 October 2026

Final integration preserved the completed Chapters 3/5 and wrote the Abstract from the agreed design status. Prose is one 150-word paragraph per substantive heading. Literature uses numbered Research Overview, Critical Assessment and Relevance to Zeest headings; common terms are not repeatedly redefined. Seventeen distinct systems/models/datasets/methods remain in the summary. The unverified Huang citation was removed rather than represented as verified evidence. Med-PaLM 2 now cites its published Nature Medicine article; MedRAG has its full ACL Findings venue.

Methodology FR identifiers match FR01--FR44: memory FR23--FR25, inputs FR14--FR22, specialists FR26--FR30, drafting/evidence/critic FR31--FR37 and physician review FR38--FR43. Approved-decision viewing remains FR44. The comparison diagram/table includes the three primary variants and critic/multimodal contrasts. The extra evidence contrast was removed. Case preparation precedes specialist analysis. Resource permissions and measurements remain outstanding execution dependencies.

No commit or push was performed. main.tex is frozen again after this integration. Degree BS(CS) and date 10 October 2026 are assumptions to confirm before submission; signature spaces were preserved.
