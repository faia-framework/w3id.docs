# FAIR AI Attribution (FAIA) framework ontology and vocabulary

Versioned ontology and vocabulary for the FAIA (Fair AI Attribution) framework. To generate a statement using the vocabulary and ontology, please see [FAIA statement generator](https://www.faia.io/statement-generator). For other semantic artifacts and integration with the Liccium platform, see [Liccium FAIA implementation](https://github.com/liccium/faia). 

## FAIA framework

The FAIA framework provides an ontology and vocabulary for machine-readable and persistent disclosure of AI involvement. It defines three complementary elements: high-level attribution flags (human-created, AI-assisted, AI-generated), activity codes describing the role AI played in the content lifecycle, and optional system attribution identifying the AI system and version involved.

FAIA is designed to support regulatory compliance with AI transparency requirements (including the EU AI Act and equivalent legislation) and to enable systematic identification of synthetic content for AI training data governance.

### faia_vocab folder content

Versioned FAIA vocabulary files in Turtle serialisation. The FAIA vocabulary covers three layers of AI involvement disclosure:

**FAIA Flags** signal the overall level of AI involvement at the content level:

- `hcc` — Human-Created Content: no AI involvement at any stage of creation or editing
- `aac` — AI-Assisted Content: human remains primary creator; AI contributed during the process
- `aig` — AI-Generated Content: AI is the primary creative agent; human input limited to prompting or selection

**Activity Codes** describe the specific operation performed, using either established domain vocabularies (STM AI Classification for academic manuscripts, IPTC Digital Source Type for visual media) or FAIA's own generic, media-independent codes: `coCreation`, `contribution`, `enhancement`, `refinement`, `transformation`, `analysis`.

### faia_ont folder content

Versioned FAIA ontology files in Turtle serialisation. The FAIA ontology defines the following data properties: `faiaFlag`, `activityCode`, `systemAttribution`, `systemVersion`.

---

## About

These artefacts are maintained by [Liccium B.V.](https://liccium.com) and the FAIA framework project team, and are published under the CC BY 4.0 licence. Persistent URLs are managed via [w3id.org](https://w3id.org), operated by the W3C Permanent Identifier Community Group.

For more information:

- Liccium: [https://liccium.com](https://liccium.com)
- FAIA documentation: [https://faia.liccium.com](https://faia.liccium.com)
- FAIA registry: [https://faia.io](https://faia.io)
