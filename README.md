You are designing and implementing XP.2Flow, a modular architecture for continuous agent improvement.

XP.2Flow means Experience Processing through a declarative Flow.

Its canonical lifecycle is:

Experience → Consolidation → Knowledge → Capability → Behavior → Experience

The lifecycle MUST be treated as a configurable directed flow, not as a hard-coded pipeline.

The objective is to allow any stage to be:

* added
* removed
* replaced
* reordered when semantically valid
* duplicated when useful
* independently implemented
* independently evaluated
* independently versioned

The system MUST NOT assume that one particular implementation of a stage is universally correct.

The canonical concepts are:

1. Experience
2. Consolidation
3. Knowledge
4. Capability
5. Behavior
6. Evaluation
7. Skill/Capability Selection
8. Trajectory
9. Outcome
10. Evidence
11. Confidence
12. Version

The canonical feedback loop is:

Experience
→ Consolidation
→ Knowledge
→ Capability
→ Behavior
→ Outcome
→ Experience

Evaluation may observe any transition.

Selection may occur between Knowledge and Capability or between Capability and Behavior.

The system MUST distinguish:

* raw experience
* derived knowledge
* hypotheses
* capabilities
* executable behavior
* observations
* evaluations
* outcomes

Do not collapse these concepts into generic "memory".

XP.2Flow is not a second-brain application.

It is a framework for turning accumulated experience into progressively better agent behavior.

The system MUST be:

* local-first
* file-readable
* Git-friendly
* model-provider agnostic
* skill-provider agnostic
* auditable
* experimentally configurable
* deterministic where possible
* probabilistic where necessary
* capable of operating without a database
* capable of later adding a database without changing the semantic model

Do not hard-code OpenRouter, Ollama, any proprietary provider, or any particular inference runtime into the semantic layer.

Model execution MUST be an adapter concern.

Do not make the framework depend on a specific LLM.

Create a formal specification before implementation.

The specification must define:

* terminology
* entities
* stage contracts
* input/output contracts
* evidence requirements
* confidence semantics
* lifecycle
* versioning
* flow configuration
* failure behavior
* validation
* rollback
* experimentation
* provenance
* training-data generation
* model evaluation
* skill evolution
* capability activation

The design must explicitly distinguish:

Skill Discovery
Skill Selection
Skill Execution
Skill Evaluation
Skill Evolution

These are different problems and MUST NOT be represented as one operation.

Do not copy COG, WikiSkill, or any existing second-brain implementation.

Use them as conceptual inputs only.

COG contributes:

* file-first knowledge
* human-readable Markdown
* Git versioning
* skills
* specialized agents
* knowledge consolidation
* memory hygiene
* verification
* separation of system instructions from user knowledge

WikiSkill contributes:

* raw experience
* persistent knowledge
* executable skills
* experience-to-knowledge compilation
* skill evolution
* validation gates
* cross-model skill transfer

The final architecture must be an independent model.

Name the specification:

XP.2Flow Specification.

Create a concise README explaining the model before writing implementation code.
