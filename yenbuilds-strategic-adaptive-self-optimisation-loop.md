Ask LLM about what it knows about your previous interactions, and let it tell you based on what it knows, how you can improve.

# Technical Actions You Repeat (and Could Turn Into Shortcuts)

## 1. Re-asking for specific markdown formatting
You frequently request:
- “Markdown pls”
- “Single markdown block”
- “No breaks”
- “All text inside one block”

**Shortcut:** `/md`  
Ensures the response is in one clean markdown block with no extras.

---

## 2. Rewriting or refactoring code modules
You often ask ChatGPT to:
- Rewrite `stability-runner.js`
- Rewrite `stability.js`
- Rewrite scoring logic
- Reorganise HUD Legacy / HUD New components

**Shortcut:** `/rewrite <module>`  
Produces a full, clean rewrite of the module.

---

## 3. Migration plans between systems
You repeatedly request:
- HUD Legacy → HUD New migration plan  
- Old logic → new architecture transitions

**Shortcut:** `/migrate <systemA> <systemB>`  
Generates a structured migration blueprint.

---

## 4. Explaining your dilemmas more clearly for others (e.g., Copilot)
You often ask:
- “Can you articulate the dilemma so I can pass to Copilot?”
- “Can you summarise this thread cleanly?”

**Shortcut:** `/handoff`  
Compresses your internal reasoning into a shareable external explanation.

---

## 5. Naming things (projects, workflows, spikes)
You frequently ask for:
- Names for isolated spike projects  
- Names for systems  
- Names for frameworks (ATSP)

**Shortcut:** `/name <concept>`  
Generates curated naming options with rationale.

---

## 6. Generating structured documents
You repeatedly ask for:
- Checklists  
- READMEs  
- Specs  
- Philosophical rule sets  
- Project overviews  

**Shortcut:** `/doc <topic>`  
Creates a formal structured document.

---

## 7. Bundling a multi-file output into a “zip-style” structure
Examples:
- HUD overlays  
- Node/JS multi-file sets  
- Tauri setups

**Shortcut:** `/bundle <project>`  
Outputs folder tree + files + README in one block.

---

## 8. Architecture restatements and snapshots
You often re-explain:
- HUD architecture  
- Stability scoring pipeline  
- Speed reference logic  
- SimBridge / telemetry pipeline

**Shortcut:** `/snapshot`  
Provides a concise architecture summary based on current context.

---

## 9. Repeatedly asking for correctness checks
Examples:
- ALT INTV behaviour  
- FLCH pressurisation  
- Proxy VREF logic  
- Stability scoring thresholds

**Shortcut:** `/verify <concept>`  
Runs a correctness sweep and outputs the authoritative summary.

---

## 10. Requesting design decisions or strategy calls
You frequently ask:
- “Is this crucial?”  
- “Should I fix this ASAP?”  
- “How to know when to begin scoring?”  
- “What runway should I consider?”  

**Shortcut:** `/design <topic>`  
Outputs a clear decision tree and a recommendation.

---

# The 7 Most Valuable Shortcuts
If you implemented only these:

1. `/md`  
2. `/rewrite <module>`  
3. `/migrate <A> <B>`  
4. `/handoff`  
5. `/bundle <project>`  
6. `/snapshot`  
7. `/verify <concept>`

---

# Optional: Your Personal Command Palette
You could standardise:

```
/md
/rewrite
/refactor
/migrate
/name
/doc
/bundle
/handoff
/snapshot
/verify
/design
```
