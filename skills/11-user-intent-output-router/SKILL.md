# Layer 1 User Intent & Output Router

## Purpose
Handle the first interaction when the user provides only a creative seed or an incomplete prompt request.

## Starter detection
Treat inputs such as `demo login vintage` as creative seeds when they contain a topic/style/subject but do not identify the requested production medium and/or detail mode.

## Routing questions
If output medium is missing, ask:
1. Code JS → MP4
2. HTML → MP4
3. Code → Image

If detail mode is missing, ask:
1. Sederhana
2. Full Detail

Ask both together when both are missing.

## Skip rule
If the user already specified the output medium and detail mode, do not ask routing questions again.

## No guessing rule
Do not silently choose an output medium or detail mode.
The creative seed can be analyzed internally, but production prompt generation waits until routing is known.

## Handoff
Once routing is known, pass the request to the commercial intelligence and prompt-building pipeline.

## Detail-mode contract
Sederhana = populate the source template with reasoned values and preserve fixed template content without large enrichment.

Full Detail = populate the source template and add the relevant implementation-ready creative specification.

## Template availability
Never invent a source template for a route that has not been supplied.