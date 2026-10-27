---
name: taste-driven-ai-designer
description: Use when designing or improving digital interfaces and product visuals, especially when a first draft feels generic, overly templated, or visually unfinished. Guides AI through divergent concept exploration, a distinct design direction, visual critique, multimodal asset use, and production-minded refinement.
---

# Taste-Driven AI Designer

Design interfaces with a recognizable point of view, clear purpose, and careful finish. Treat AI as a fast design partner: it can explore and execute many options, while the human sets the taste bar and steers the direction. Do not expect one prompt to produce a finished, studio-quality result.

## When to use

- Creating or redesigning a website, app screen, landing page, dashboard, game UI, or interactive prototype.
- Improving an existing interface that looks generic, cluttered, or unfinished.
- Establishing a visual direction before implementation.

Adapt the process to the scope. For a small, clearly specified change, move directly to the relevant phase instead of forcing a full discovery exercise.

## Working principles

1. **Start with the product and its feeling.** Identify the audience, task, context, platform, and intended emotional response. Visual novelty must support those needs.
2. **Explore before committing.** Generate genuinely different directions instead of polishing the first familiar layout.
3. **Make inspiration concrete.** Use a specific cultural, material, architectural, editorial, game, or product reference as a starting point; translate its qualities rather than copying its surface.
4. **Use judgment, not randomness for its own sake.** External seeds can help break repeated defaults, but every resulting choice must still make sense for the product.
5. **Separate making from judging when possible.** Evaluate the rendered result from a fresh visual perspective, ideally against concrete reference examples.
6. **Prefer restraint and clarity.** Every component, effect, label, and animation needs a purpose.
7. **Honor platform conventions and accessibility.** Distinctive visual styling must preserve usable controls, readable contrast, predictable interaction, and native behavior where appropriate.

## Workflow

### 1. Discover — open the design space

Before drawing or coding, extract or infer:

- What the product does and who it serves.
- The primary user task and the most important content or action.
- Platform, device, accessibility, technical, and brand constraints.
- The intended feeling in a few plain-language words.

If key information is missing, make reasonable assumptions and state the ones that materially shape the design. Ask only when an answer would change the direction significantly.

Explore several distinct concept directions. Vary the underlying idea, composition, visual language, and interaction model—not just the palette. For example, consider editorial, instrument-like, archival, tactile, cinematic, utilitarian, or playful directions when they fit the product.

When ideas are stuck in familiar patterns, introduce a seed from outside the default UI vocabulary. A random string, a physical material, a place, an era, or an unexpected reference can prompt new associations. Treat it as inspiration, not a requirement to reproduce literally. Do not invent a seed-generation tool or claim to have used one if unavailable.

For each promising direction, capture:

- A short concept name and rationale tied to user needs.
- Composition and information hierarchy.
- Typography, color, materials, imagery, and motion principles.
- One or two signature details that make it memorable.
- Risks to legibility, usability, accessibility, or implementation.

If the user is participating in art direction, present a concise set of materially different options and incorporate their reactions before locking the direction. If the user asked for direct implementation, choose the strongest justified direction and proceed without making the exploration a blocker.

### 2. Define — give the direction a coherent identity

Turn the selected concept into a small design brief before expanding details. Define tokens or rules for type scale, spacing, color roles, surfaces, borders, radii, iconography, image treatment, and motion. Use a system that supports the concept rather than adding a new style to every element.

Build a functional first pass around real content and primary tasks. Keep the hierarchy obvious. Use layout and whitespace to group content before adding containers. Reuse existing project conventions and platform components when they fit.

Use visual assets when they add meaning or atmosphere. Prefer generated, sourced, or project-provided imagery over generic gradients and code-drawn decoration when a real image would strengthen the concept. Use image or video generation only when an available tool can produce a useful asset; do not assume API access, expose secrets, or add credentials to source code. Motion should explain state, provide feedback, or reinforce the concept, and should respect reduced-motion preferences.

### 3. Critique — assess the rendered design independently

When visual inspection is available, capture the actual interface at relevant viewport sizes and inspect the screenshot. Do not judge only from code or design intentions. If a separate critic/model is available, give it the screenshot and design brief without implementation details or prior self-justifications. If no separate critic is available, deliberately review from a fresh perspective and acknowledge that the review is not independent.

Use consistent criteria on each pass:

- Does the visual hierarchy make the primary task clear?
- Is the concept recognizable and coherent across the screen?
- Are composition, spacing, alignment, type, and contrast intentional?
- Do imagery and motion earn their place?
- Are controls legible, usable, accessible, and appropriate to the platform?
- Which three changes would most improve the result?

Feedback must point to visible evidence and concrete changes. Prefer comparative references or moodboards when supplied; use them as quality anchors, not templates to copy. A numeric score is optional and must not replace explanation. Do not demand a fixed score or claim independent approval when no independent reviewer was used.

Implement the highest-impact feedback, then inspect the result again. Usually start with one or two focused iterations. Continue only while changes produce meaningful improvement; avoid endless polish loops.

### 4. Deliver — refine by subtraction and verify

Run an explicit “AI tells” audit during refinement. These patterns are not inherently forbidden, but become warning signs when used without a reason or combined indiscriminately:

- Ambient purple/cyan glows, gradient borders, and effects used as a substitute for visual substance.
- A card or Bento box for every paragraph, metric, or list item.
- Identical oversized corner radii or pill shapes on every control and surface.
- Floating badges and labels that provide no useful information.
- The default left-copy/right-graphic hero or centered headline without a concept-specific reason.
- Generic vector shapes where meaningful imagery or product data belongs.
- Custom controls that are less clear or less usable than established platform components.
- Dense decoration, arbitrary accent colors, excessive labels, or redundant copy.

For each questionable element, ask: what user need or design idea does this serve? Remove it if the answer is unclear. Let typography, spacing, alignment, and a few meaningful contrasts carry the hierarchy. Preserve intentional conventions when they improve usability or fit the brand; this audit is a diagnostic, not a ban list.

Treat generated copy as layout placeholder when factual or brand-accurate language is unavailable. Replace it with concise, specific, natural copy before delivery when possible. Do not invent product claims, testimonials, metrics, or capabilities. If final copy needs user input, clearly mark the placeholder.

Before handing off, verify the rendered screen at the target viewport and check responsive behavior, key interaction states, text overflow, contrast, focus/selection states, and motion behavior as relevant to the task. Report what was visually inspected and what remains unverified; do not claim checks that were not performed.

## Critic prompt

Use this when a separate visual critic is available. Provide the screenshot and intended design brief; keep the critic context fresh between rounds.

> You are an independent visual design critic. Review the attached interface screenshot against the stated product purpose, audience, and intended visual direction. Judge only what is visible; do not infer implementation quality. Assess hierarchy, composition, typography, spacing, color, imagery, interaction clarity, accessibility cues, and finish. Identify generic or unmotivated patterns. Give the three highest-impact specific changes, including anything to delete or simplify. Explain your reasoning with visible evidence. Be decisive and practical. A score is optional; if given, explain what it measures.

## Scope and extensions

This is the foundational workflow for taste-driven interface design. Add future methods as focused sections or linked reference files, keeping the core workflow concise and preserving the distinction between principles, optional techniques, and project-specific constraints.

## Source

Adapted and synthesized from [“How to Turn Your AI into a World-Class Designer”](https://github.com/CodingRookie98/cr-agent-arsenal/blob/master/docs/reference/articles/how-to-turn-your-ai-into-a-world-class-designer.md#why-ai-struggles-with-design-by-default), with emphasis on divergent discovery, distinct design identity, independent visual critique, multimodal assets, and ruthless subtraction. This skill is an operational adaptation, not a reproduction of the source article.
