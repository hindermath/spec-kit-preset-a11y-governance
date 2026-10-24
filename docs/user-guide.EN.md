# User guide: a11y-governance

<!-- current-package: 0.4.6 -->

Package identity: **v0.4.6**. [Preparation and publication boundary](release-0.4.6-validation.md). The release page, not this preparation snapshot, proves publication and the external archive hash. Earlier version records below remain historical.

[Release-Abschluss und Verbesserungsprofil / Publication closeout and improvement profile](release-0.4.5-validation.md).

The linked base-package evidence remains historical; this package includes the source corrections as a new version.

[Deutsch](user-guide.md) · [Preset reference](../README.md)

Historical base package **v0.4.5**. Verify the actually published version on the [release page](https://github.com/hindermath/spec-kit-preset-a11y-governance/releases). This guide grants no merge, release or project authority.

Contents: [Start](#start) · [Example](#example) · [Terms](#terms) · [Routing](#routing) · [Troubleshooting](#help) · [References](#references)

<a id="start"></a>

## Start and audience

Plan usable interfaces and understandable bilingual documentation from the start.

For apprentices in all four IHK IT occupations: IT specialists (application development, systems integration, data/process analysis, digital networking), IT systems electronics technicians, digitalisation management specialists and IT systems management specialists. Also for developers without specialist governance knowledge. You do not need to edit hashes or invent model IDs to ask for the next step. Ask the maintainer to check technical bindings.

Use an already initialized Spec Kit target repository. Read the prerequisites and installation instructions in the preset reference first; replace example paths. A template is a starter, not completed evidence. Installation adds instructions and files; it does not start a feature or grant approval.

Input: Name CLI, documentation or UI, the audience and available assistive technology.

<a id="example"></a>

## One complete example

1. Describe the bounded task and existing files. Do not silently widen scope.
2. Use the following example in the agent chat. It is a prompt, not a shell command:

~~~text
Use cli-a11y-review-template and bilingual-content-check-template for my status CLI. Plan docs/accessibility/status-review.md with keyboard, text and screen-reader checks; leave untested cases open.
~~~

3. Applicable criteria, DE/EN content, actual tests and untested assistive technology remain traceable. No automatic AA claim.
4. Check the result and recorded next action. Changes, repair, feature execution and delivery each need their applicable authority. A passing technical check is not human acceptance.

Read-only installation check in the initialized target repository:

~~~text
specify preset info a11y-governance
specify preset resolve bilingual-content-check-template
~~~

Resolve reports the selected template source; it does not fill in or execute that template.

<a id="terms"></a>

## Terms and evidence

- **WCAG 2.2 AA:** Accessibility criteria; record applicable criteria and actual verification.
- **CEFR B2:** Target for understandable language, not an automatically awarded certificate.
- **Textalternative:** Equivalent important information in understandable text, not only colour or images.

Where the existing contract uses these values: Applicable means relevant, not passed; N/A needs a reason; Open needs the recorded next action and responsible person. This explanation adds no fields to existing schemas. Keep genuine historical evidence; never edit a hash or approval just to make a check pass.

<a id="routing"></a>

## Stable routing and explicit actions

| Command | Declared role |
|---|---|
| `speckit.specify` | `frontier-reasoning` |
| `speckit.plan` | `frontier-reasoning` |
| `speckit.tasks` | `frontier-reasoning` |

Roles describe tasks, not a model name or quality guarantee. Read the actual model-routing.json contract; generic examples such as coding-review do not override a stronger command requirement. The existing autonomous runner retains the strongest overlapping role, independently of installation priority. Merely installing a role contract does not switch a live chat or configure personal profiles.

A model-free script check and an agent assessment are different activities. Model calls, including model-access preflights, can consume quota even when they are read-only. No probe or provider switch is authorized by this documentation. No new dynamic-routing implementation is included.

Package version, schema version and historical field test are different facts. Earlier acceptance applies only to its recorded scope and source state.

<a id="help"></a>

## Troubleshooting and safe next action

No graphical UI does not mean no accessibility scope. CLI and documentation also face users. Mark unperformed screen-reader checks as open.

If a command or template is missing, inspect preset info and the manifest below. Check the documented minimum tools and enabled installation. Resolve ambiguity with the maintainer; do not change policy, disable validators or claim an unperformed test. A safety blocker remains a blocker.

This language/accessibility pass targets CEFR B2 and applicable WCAG 2.2 AA. Static tests do not certify that target. Screen-reader, Braille and representative-user tests not actually performed remain unverified.

<a id="references"></a>

## Templates and deeper reference

- [`a11y-checklist-template`](../templates/a11y-checklist-template.md)
- [`bilingual-content-check-template`](../templates/bilingual-content-check-template.md)
- [`cli-a11y-review-template`](../templates/cli-a11y-review-template.md)
- [`a11y-evidence-template`](../templates/a11y-evidence-template.md)
- [`didactic-code-comment-check-template`](../templates/didactic-code-comment-check-template.md)

These names identify available starters; they are not an instruction to create every file. Reuse existing suitable evidence. JSON field names remain technical identifiers, not translated keys.

- [Manifest and prerequisites](../preset.yml)
- [Stable command-role contract](../model-routing.json)
- [Documentation scope, review and test limits](documentation-closeout.md)
