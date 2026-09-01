---
title: "MOSAIC: A Modular Search-and-Rescue Testbed for Human-AI Collaboration Research"
tags:
  - Python
  - human-AI collaboration
  - human-AI teaming
  - search and rescue
  - reinforcement learning
  - Gymnasium
  - MiniGrid
  - human-subjects experimentation
authors:


- name: Author Name # TODO: confirm full author list, spelling, and order
    orcid: 0000-0000-0000-0000 # TODO: real ORCID
    corresponding: true # TODO: confirm corresponding author
    affiliation: 1
affiliations:
  - name: TODO institution, department, city, country
    index: 1
  
  - name: TODO institution, department, city, country
    index: 1
    
date: 1 September 2026 # TODO: update to the actual submission date
bibliography: paper.bib
---

# Summary

<!--
OUTLINE - 150-200 words. Do not draft yet.

  - Introduce human-AI collaboration for a non-specialist audience.
  - Explain the need for controlled and repeatable research environments.
  - Define MOSAIC and its search-and-rescue task.
  - State the roles of the human and the AI accurately (verify against the code
    before writing; do not overstate the AI's autonomy or authority).
  - Summarize the main software capabilities and the intended users.
  - -Clear and understandable

CONSTRAINT: no novelty comparisons in this section - those belong in
"State of the field".
-->

# Statement of need

<!--
OUTLINE - 180-250 words. Do not draft yet.

  - Explain the challenge of studying human-AI interaction under time pressure,
    uncertainty, workload, and incomplete information.
  - Explain the need to measure behavior, performance, communication, situation
    awareness, and physiological signals.
  - Explain the difficulty of combining simulation, GUI, AI, sensing, logging,
    and replay tooling independently.
  - Identify the target users: human-AI teaming, human-factors, HCI, and
    reinforcement-learning researchers conducting human studies.
  - End with the precise research gap that MOSAIC addresses.
-->

# State of the field

<!--Do not draft yet, and do not add citations in this pass.

Reserve comparisons with:
  - MiniGrid
  - Gymnasium
  - MATRX, including its urban search-and-rescue testbed
  - Overcooked-AI
  - PsychoPy
  - Lab Streaming Layer

The eventual comparison must consider:
  - purpose
  - human interaction
  - AI-agent or AI-advisor support
  - Gymnasium compatibility
  - SAR functionality
  - experimental instrumentation
  - physiological-data integration
  - reproducibility
  - extensibility

REQUIRED: an explicit "build versus contribute" justification - why MOSAIC was
built as a separate testbed rather than contributed as an extension to one of
the systems above.

TODO: add the corresponding BibTeX entries to paper.bib when the comparison is
written. paper.bib is currently empty by design.
-->

# Software design

<!--
OUTLINE - 300-400 words. Do not draft yet.

Organize the discussion around design decisions, not a module tour:

   1. Reusable Gymnasium/MiniGrid environment core.
   2. SAR mechanics and observations.
   3. Separation between reusable `mosaic` code and study-specific `experiment`
      code.
   4. Constructor-injected study components and neutral defaults.
   5. Human interaction through the GUI.
   6. Provider-independent AI-advisory interface.
   7. Experimental logging, sensing, and replay.
   8. Composition versus inheritance.
   9. Reusability versus study-specific calibration.
  10. Reproducibility and testability.

Grounding pointers for the drafter - verify each against the code before making
any claim about it:
  - src/mosaic/sar/env.py, src/mosaic/sar/observations.py, src/mosaic/sar/actions.py
  - src/mosaic/core/level.py, src/mosaic/core/camera.py, src/mosaic/core/placers.py
  - src/mosaic/gui/main.py (SAREnvGUI), src/mosaic/gui/chat.py,
    src/mosaic/gui/feedback.py
  - src/mosaic/llm/client.py, src/mosaic/llm/parser.py
  - src/experiment/experiment.py, src/experiment/replay.py
  - src/experiment/sensors/eye_tracker/
  - tests/
-->

<!--
RESERVED - one optional architecture figure. NOT CREATED YET.

Intended content:

    Human / AI
        |
    GUI and advisory interface
        |
    MOSAIC SAR environment
        |
    Observations, events and measurements
        |
    Logging, sensing and replay

When the figure exists, place it in paper/figures/ and reference it as:
    ![Caption.\label{fig:architecture}](figures/architecture.png)
-->

# Research impact statement

<!--
OUTLINE - 150-250 words. Do not draft yet.

AWAITING AUTHOR CONFIRMATION. Request verified evidence only:
  - Completed or ongoing studies that used MOSAIC.
  - Pilot-study use and approved participant information.
  - Data streams actually collected and the research questions they enabled.
  - Publications, preprints, posters, presentations, theses, or datasets.
  - Use by collaborators or other research groups.
  - Reproducible demonstrations or benchmarks.

CONSTRAINT: projected or planned future applications are NOT evidence of impact
and must not be presented as such. Do not invent studies, participant counts,
or results.
-->

# AI usage disclosure

<!--
OUTLINE - 60-100 words. Do not draft yet.

AWAITING AUTHOR CONFIRMATION of:
  - Which generative-AI tools were used in the software, the documentation, or
    the manuscript.
  - What those tools contributed.
  - What the human authors reviewed and decided.
  - How tests, code review, and manual verification checked correctness.

Do not write the final disclosure until the authors confirm these facts.
-->

# Acknowledgements

<!--
OUTLINE - 40-80 words. Do not draft yet.

AWAITING AUTHOR CONFIRMATION of:
  - Funding agencies and grant numbers.
  - Institutional and laboratory support.
  - Non-author contributors.
  - Equipment support.

Do not invent acknowledgements, funders, or grant numbers.
-->

# References

<!--
Leave empty. JOSS generates this section from paper.bib.
-->
