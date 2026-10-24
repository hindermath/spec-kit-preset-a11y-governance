# A11Y Governance Preset

<!-- current-package: 0.4.6 -->

Paketkennung: **v0.4.6**. [Vorbereitung und Veröffentlichungsgrenze](docs/release-0.4.6-validation.md). Die Release-Seite und der externe Archivnachweis belegen die Veröffentlichung, nicht dieser Vorbereitungsstand. Frühere Versionsnachweise unten bleiben historisch.

<span lang="en">Package identity: v0.4.6. The release page and external archive evidence prove publication, not this preparation snapshot. Earlier version records below remain historical.</span>

[Release-Abschluss und Verbesserungsprofil / Publication closeout and improvement profile](docs/release-0.4.5-validation.md).

Der unten verlinkte Basispaket-Nachweis bleibt historisch; dieses Paket nimmt die Quellenkorrekturen als neue Version auf.

<span lang="en">The linked base-package evidence remains historical; this package includes the source corrections as a new version.</span>

**Leserpfad / Reader path:** [Deutsch: Einstieg, Begriffe und Fehlerhilfe](docs/user-guide.md) · [English: start, terms and troubleshooting](docs/user-guide.EN.md).

Historisches Basispaket **v0.4.5**. Der [Release-Stand](https://github.com/hindermath/spec-kit-preset-a11y-governance/releases) wird getrennt geprüft; ein Commit auf main ist noch keine Veröffentlichung oder Installation.

*Historical base package v0.4.5. The release page records actual publication separately; a main-branch commit is not publication or installation.*


Patch **0.4.5** liefert die verbesserte zweisprachige Einstiegs- und
Kompositionsdokumentation. Verhalten und Berechtigungsgrenzen bleiben erhalten.
[Release-Nachweis / Release record](docs/release-0.4.5-validation.md).

*Patch 0.4.5 packages the improved bilingual getting-started and composition
guide. Behavior and authority boundaries remain unchanged.*

Version: `0.4.6`
Status: Veröffentlichung über die Release-Seite prüfen / verify publication on the release page
Priority: `40`
Requires: Spec-Kit `>=0.8.0` (uses the `wrap` and `append` composition
strategies introduced in `0.8.x`).

Version `0.4.2` ergänzt einen portablen Zielgruppenvertrag: Das Projekt
deklariert Zielgruppe und Vorwissen. Lernmaterial erklärt Fach- und
Spec-Kit-Begriffe beim ersten Auftreten und stellt Abhängigkeiten, Status,
Entscheidungen und nächste Schritte immer auch als geordneten Text bereit.

*Version `0.4.2` adds a portable audience contract: the project declares its
audience and assumed prior knowledge. Learning material explains domain and
Spec Kit terms on first use and always provides dependencies, status,
decisions, and next actions as ordered text.*

## Zweck / Purpose

### Einstieg und Arbeitsweise / Getting Started and Workflow

Nach Installation im initialisierten Zielprojekt bindet das
[Manifest](preset.yml) `wrap`-Anweisungen für Specify/Plan/Tasks und
`append`-Ergänzungen ihrer Dokumentvorlagen und Constitution ein. Es startet
keinen Screenreader, Scanner oder Übersetzungsreview. Separate Starter und
das Agent-Guidance-Addendum sind Hilfsmittel, keine automatisch ausgefüllten
Nachweise oder Garantie der Übernahme in jede Agenten-Datei.

*After installation in an initialized target project, the [manifest](preset.yml)
integrates wrap instructions for Specify/Plan/Tasks and append contributions
for their templates and constitution. It starts no screen reader, scanner or
translation review. Separate starters and the agent-guidance addendum are
aids, not completed evidence or guaranteed inclusion in every agent file.*

Beispiel für einen CLI-Statusbefehl: Wähle `cli-a11y-review-template` und
`bilingual-content-check-template`. Plane konkrete Prüfungen für Textausgabe,
Tastatur-/Hilfsmittelnutzung, Sprache und verständliche Statusbezeichnungen;
halte Ergebnisse etwa in `docs/accessibility/cli-status-review.md` fest.
Specify benennt Zielgruppe und Anforderungen, Plan die Prüfmethoden, Tasks
die verbleibenden Schritte und Nachweisdateien. Tests und fachliche Abnahme
müssen tatsächlich erfolgen; Beispielpfade belegen keinen Erfolg.

*For a CLI status command, select `cli-a11y-review-template` and
`bilingual-content-check-template`. Plan text output, keyboard/assistive
technology, language and clear status-label checks; record results, for
example, in `docs/accessibility/cli-status-review.md`. Specify defines audience
and requirements, Plan the methods, Tasks remaining steps and evidence files.
Actual tests and acceptance are still necessary; example paths prove no pass.*

Bestehende Evidence wiederverwenden und auf Aktualität prüfen. `Applicable`
ist keine WCAG-Abnahme; `N/A` braucht Begründung und Trigger, `Open` Owner
und Folgeaktion. Ein grüner technischer Check ersetzt keine Hilfsmittelprüfung.

*Reuse existing evidence after checking freshness. Applicable is not WCAG
acceptance; justify N/A and its trigger, assign an owner and follow-up to Open.
A successful technical check does not replace assistive-technology testing.*

Priorität ist keine zeitliche Testreihenfolge: kleinere Zahlen bedeuten höhere
Auflösungspriorität. `append` ergänzt und `wrap` verschachtelt; gleichnamige
`replace`-Beiträge oder Projekt-Overrides können Inhalte verdrängen. Eigene
Reihenfolgen nicht als pauschal geprüft behandeln. Kontrolliere
`specify preset resolve plan-template` und erzeugte Agentenflächen.

*Priority is not a test schedule: lower numbers mean higher precedence.
Append adds and wrap nests; same-name replace layers or project overrides may
hide content. Custom orderings are not universally tested. Inspect
plan-template resolution and generated agent surfaces.*

Leserpfad / Reader path: [Installation](#installation--install) →
[Evidenzvorlagen / Evidence Templates](#evidenzvorlagen--evidence-templates) →
[Prüfung / Verification](#prüfung--verification) →
[Fehlersuche / Troubleshooting](#fehlersuche--troubleshooting).

Dieses Standard-Preset bringt Barrierefreiheit, DE-first/EN-second
Auslieferung, CEFR-B2-Lesbarkeit und didaktische Inline-Kommentarprüfung in
Spec-Kit-Workflows. Es macht `Programmierung #include<everyone>` als
wiederverwendbare Governance sichtbar, statt diese Regel nur lokal in einem
Repository zu halten.

*This standard preset injects accessibility, DE-first/EN-second delivery,
CEFR-B2 readability, and didactic inline-comment review into Spec-Kit
workflows. It preserves `Programmierung #include<everyone>` as reusable
governance instead of keeping it as a local-only policy.*

Das Qualitätsziel ist, dass nutzerseitige Artefakte auch mit Tastatur,
Screenreader, Braille-Zeile, Textbrowser und klarer Sprache nutzbar bleiben.
Das gilt für CLI-Ausgaben, Dokumentation, HTML, UI und generierte Templates.

*The quality goal is that user-facing artifacts remain usable with keyboard,
screen readers, Braille displays, text browsers, and clear language. This
applies to CLI output, documentation, HTML, UI, and generated templates.*

## Zielgruppen / Audience

Dieses Preset eignet sich, wenn:

- ein Projekt nutzerseitige CLI-, Dokumentations-, HTML-, UI- oder
  Template-Artefakte erzeugt;
- Lernende aller vier IHK-IT-Berufe mit verständlichen DE-first/EN-second
  Materialien arbeiten sollen: Fachinformatiker*innen aller vier Fachrichtungen,
  IT-System-Elektroniker*innen, Kaufleute für Digitalisierungsmanagement
  (KDM) und Kaufleute für IT-System-Management (KITSM);
- WCAG 2.2 Level AA und CEFR B2 früh in Spec, Plan und Tasks sichtbar sein
  sollen;
- nicht-triviale Logik didaktische Kommentare braucht, damit Wartung und
  Ausbildung nicht am Codeverständnis scheitern.

*Use this preset for user-facing CLI, documentation, HTML, UI, or template
artifacts; for all four IHK IT occupations, including all four IT-specialist
tracks, IT systems electronics technicians, digitalisation management and
IT systems management specialists; for DE-first/EN-second learning material;
when WCAG 2.2 Level AA
and CEFR B2 should be visible early in specs, plans, and tasks; and when
non-trivial logic needs didactic comments for maintainability and learning.*

## Lieferumfang / What It Provides

- Addenda für Constitution, Spec, Plan, Tasks und Agent-Guidance
- Wrapper für `speckit.specify`, `speckit.plan` und `speckit.tasks`
- Templates für A11Y-Review, bilinguale Inhaltsprüfung, CLI-A11Y,
  A11Y-Evidence und didaktische Code-Kommentarprüfung
- auditfähige Spec-Kit-Run-Evidence-Felder für Anwendbarkeit, `N/A`-Begründung,
  Reviewer, Evidence-Pfad, Restrisiko und Follow-up

*The preset provides addenda for the main Spec-Kit artifacts and agent
guidance, wraps the normal Specify/Plan/Tasks flow, and supplies templates for
accessibility review, bilingual content checks, CLI accessibility, evidence,
and didactic code-comment review.*

## Nicht enthalten / What It Does Not Provide

Das Preset führt keine Accessibility-Scanner, Screenreader-Tests,
Übersetzungsprüfung oder UI-Automation selbst aus. Es ersetzt keine Prüfung
durch betroffene Nutzergruppen und erteilt keine Repository-, Merge-,
Deployment- oder Provider-Administrationsrechte.

*The preset does not run accessibility scanners, screen-reader tests,
translation review, or UI automation by itself. It does not replace review
with affected user groups and grants no repository, merge, deployment, or
provider-administration authority.*

## Voraussetzungen / Prerequisites

1. kompatible GitHub Spec-Kit CLI;
2. gültige Spec-Kit-Integration im Ziel-Repository;
3. versionierte Constitution und Agent-Guidance;
4. geklärter Evidence-Ort, standardmäßig `docs/accessibility/`;
5. bekannte Zielgruppen, Artefakttypen und Sprachebene.

*Before installation, use a compatible GitHub Spec-Kit CLI, a valid Spec-Kit
integration, versioned constitution and agent guidance, a clear evidence
location, and known target audiences, artifact types, and language level.*

## Installation / Install

### Veröffentlichter Tag / Published Tag

```bash
specify preset add --from https://github.com/hindermath/spec-kit-preset-a11y-governance/archive/refs/tags/v0.4.6.zip --priority 40
specify preset info a11y-governance
```

### Entwicklungs-Checkout / Development Checkout

```bash
specify preset add --dev /path/to/a11y-governance --priority 40
specify preset info a11y-governance
```

### Empfohlene Kombination / Recommended Composition

| Priority | Preset |
|---:|---|
| 10 | [security-governance](https://github.com/hindermath/spec-kit-preset-security-governance) |
| 20 | [architecture-governance](https://github.com/hindermath/spec-kit-preset-architecture-governance) |
| 30 | [isaqb-architecture-governance](https://github.com/hindermath/spec-kit-preset-isaqb-architecture-governance) |
| 40 | [a11y-governance](https://github.com/hindermath/spec-kit-preset-a11y-governance) |
| 50 | [cross-platform-governance](https://github.com/hindermath/spec-kit-preset-cross-platform-governance) |
| 60 | [agent-parity-governance](https://github.com/hindermath/spec-kit-preset-agent-parity-governance) |

Priorität 40 ordnet dieses Preset in die empfohlene Komposition mit Security
und Architektur ein; sie startet keine zeitlich nachgelagerte Prüfung.

*Priority 40 places accessibility alongside security and architecture in the
recommended composition; it does not schedule or execute a later review.*

## Quellkapitel / Source Chapters

- `VII. Programmierung #include<everyone> — Inclusion & Accessibility By
  Default`
- `VIII. DE-First / EN-Second Bilingual Delivery`

## Standards und Regeln / Standards and Rules

- `WCAG 2.2 Level AA` baseline for every user-facing artifact
- `DE first, EN second` delivery; bilingual `DE / EN` headings or a
  synchronised `*.EN.md` companion
- `CEFR Level B2` readability target for user-facing prose
- German orthographic correctness (umlauts and `ß`, no ASCII fallbacks)
- Code-block language tagging discipline (no bare ` ``` ` fences)
- Didactic inline-code comments for non-trivial logic when learning
  comprehension or maintainability benefits
- Agent-file parity across `AGENTS.md`, `CLAUDE.md`, `GEMINI.md`, and
  `.github/copilot-instructions.md`
- A11Y coverage for `CLI`, `documentation`, `HTML`, `UI`, and generated
  templates

## Preset-Strategie / Preset Strategy

- append accessibility governance to `constitution-template`,
  `spec-template`, `plan-template`, and `tasks-template`
- provide a standalone agent-guidance addendum template for projects that
  maintain agent instruction files
- wrap `speckit.specify`, `speckit.plan`, and `speckit.tasks` with a
  shared accessibility workflow
- provide starter templates for A11Y review, bilingual content review,
  CLI accessibility review, and accessibility evidence

## Evidenzvorlagen / Evidence Templates

- Spec-Kit run evidence fields are embedded in the evidence templates to support
  audit-ready applicability, `N/A` rationale, reviewer, and follow-up records.
- `a11y-checklist-template` (WCAG 2.2 AA criteria coverage)
- `bilingual-content-check-template` (DE/EN headings, German
  orthography, CEFR-B2 readability, `*.EN.md` companion guidance)
- `cli-a11y-review-template` (text mode, `NO_COLOR`, screen reader,
  Braille)
- `a11y-evidence-template`
- `didactic-code-comment-check-template` (comment-needed review for
  non-trivial code logic)

Default evidence location: `docs/accessibility/`.

## Prüfung / Verification

```bash
specify preset list
specify preset info a11y-governance
specify preset resolve cli-a11y-review-template
specify check
```

Prüfe zusätzlich, ob nutzerseitige Artefakte im Plan benannt sind und ob N/A
für WCAG, Bilingualität oder CEFR B2 begründet wurde.

*Also verify that user-facing artifacts are named in the plan and that N/A
decisions for WCAG, bilingual delivery, or CEFR B2 are justified.*

## Einsatz / When to Use

- any project that produces user-facing `CLI`, `documentation`, `HTML`,
  `UI`, or generated templates
- teams that want accessibility, bilingual delivery, and readability
  treated as first-class planning concerns
- learning, training, or reference projects where non-trivial code logic
  should remain understandable for apprentices and future maintainers

## Nicht verwenden / When Not to Use

- purely internal artifacts with no user-facing surface at all
- teams that do not want DE-first / EN-second guidance

## Fehlersuche / Troubleshooting

### Kein UI vorhanden / No UI Exists

Prüfe CLI-Ausgaben, Dokumentation und Templates trotzdem. Diese Artefakte sind
nutzerseitig, wenn Menschen sie lesen, bedienen oder bearbeiten.

### N/A ist zu pauschal / N/A Is Too Broad

Trenne Artefakttypen. Ein Projekt ohne HTML-UI kann trotzdem CLI- und
Dokumentations-A11Y brauchen.

### Kommentare fehlen / Comments Are Missing

Bewerte nicht jede öffentliche Funktion mechanisch gleich. Kommentare sind
erforderlich, wenn nicht-triviale Logik, Lernkontext, Randbedingungen oder
Trade-offs sonst schwer verständlich bleiben.

## Sicherheit und Grenzen / Safety and Boundaries

- Installation adds governance prompts, templates, and wrapped Spec-Kit
  command guidance; it does not run accessibility tooling by itself.
- The preset does not grant repository, remote, merge, deployment, or
  provider-administration authority.
- WCAG, bilingual, readability, and evidence decisions remain auditable
  project decisions and must be recorded when declared `N/A`.

## Abdeckung / Coverage

- generated templates count as user-facing when humans are expected to
  read or edit them
- CLI output, review checklists, and bilingual delivery all belong to
  the preset's scope

## Versionshinweise / Release Notes

- `v0.4.3` publishes the agent-neutral `model-routing.json` contract for
  composition with Model Routing Governance; A11Y behavior is unchanged.
- `v0.4.2` adds the project-declared audience, prior-knowledge, first-use
  terminology, and text-first information contract.
- `v0.4.1` adds accessible text/JSON status parity, stable labelled ordering,
  and understandable repeated status/resume output.
- `v0.4.0` adds audit-ready Spec-Kit run evidence fields so generated Markdown
  documents and checklists can record applicability, `N/A` rationale, reviewer,
  evidence path, residual risk, and follow-up per standards-relevant Spec-Kit
  run.

## Kompatibilitäts- und Sicherheitsübersicht / Compatibility and Safety Summary

- kompatibel mit Spec-Kit `>=0.8.0`
- priorisiert als Stufe `40`
- deckt CLI, Dokumentation, HTML, UI und generierte Templates ab
- keine automatischen Scanner-, Remote-, Merge- oder Provider-Aktionen
- WCAG-, CEFR-, Bilingualitäts- und Kommentarentscheidungen bleiben
  projektbezogene Evidence

## License

MIT. See `LICENSE`.
