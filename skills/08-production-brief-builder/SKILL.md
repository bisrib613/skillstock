# Prompt Template Builder — Layer 1

## Purpose
Take the resolved commercial/creative brief and fill the selected user-supplied prompt template while preserving the template's original structure.

## Template fidelity
- Treat the source template as authoritative.
- Preserve the role statement.
- Preserve every field name and field order.
- Preserve populated defaults unless explicitly overridden by the user.
- Fill intentionally blank placeholders.
- Preserve all fixed visual, motion, and code instruction blocks.
- Do not summarize or shorten.
- Do not redesign the template.
- Do not add unrelated instructions.
- Do not generate the downstream code.

## Placeholder rule
An empty placeholder means the system must infer and insert the appropriate value using the research and creative-intelligence skills.

A populated placeholder/default is already intentional. Keep it unchanged unless the user explicitly changes it.

## Prompt output
The result must be a complete ready-to-use prompt for the downstream generator.

## QA
Before returning the prompt, verify that no required placeholder remains unresolved, fixed defaults were preserved, the original instructions remain intact, and the result is internally consistent with the requested topic.