---
layout: post
title: "A Position Paper on Reproducibility and Credibility in Scientific Computing"
date: 2025-04-07
description: "Why reproducibility and VVUQ are essential for building credible, team-based scientific computing workflows."
tags: reproducibility, scientific-computing, vvuq, hpc, workflows
categories: position_paper
---

### Citation
Rodriguez, Paulina (2026). Reproducibility and Credibility Are the Foundations of Team-Based Scientific Computing. figshare. Online resource. <a href="https://doi.org/10.6084/m9.figshare.31956681.v1">https://doi.org/10.6084/m9.figshare.31956681.v1</a>

<hr> 

(Revised April 1, 2026)

High-consequence decisions cannot rely on models that no one can re-run, where plots cannot be regenerated, and where data is no longer interpretable. Reproducibility makes computational modeling and simulation (CM&S) evidence durable and portable across people, platforms, and time. Despite years of recognizing its necessity for quality science, it is still not systematically implemented. 

In CM&S, value leaks when code, data, software, environments, credibility assessments, and workflows are not captured for re-execution. Trust then shifts from the evidence to the analyst, and institutional memory fades. This challenge spans all modeling. Physics-based models are costly because each solver run can require large parallel resources; AI and machine-learning models are costly because training demands extensive computation and data. Both require not only code and data preservation but documentation of model context, limitations, and credibility assessments.

## Reproducibility Is Not Optional for Team Science 

<blockquote>
    Opaque modeling workflows isolate contributors and undermine collaboration, reproducibility must be built in from the start. 
</blockquote>

In team-based science, computational modeling often becomes a bottleneck, not because of lack of expertise, but because the modeling process is opaque, fragile, and siloed. I’ve experienced this firsthand: as the only CFD modeler on interdisciplinary teams, I was solely responsible for simulations using commercial solvers like ANSYS. These tools are quick to start with but difficult to transfer, reproduce, or scale across platforms and collaborators. 

After losing access to a decommissioned ANSYS workstation, I couldn’t reproduce prior results. Minimal configuration files didn’t translate between versions. This led me to OpenFOAM, an open-source alternative that enabled HPC use, reproducibility, and modularity though at the cost of a steeper learning curve. Still, it was worth it: transparent tools enabled rigorous verification and validation  and  uncertainty quantification (VVUQ), and ultimately building credible and trustworthy evidence. 

## Credibility Requires More Than Just Code 

<blockquote>
    Trustworthy simulations require rigorous VVUQ, not just shared code since credibility depends on both accuracy and reliability. 
</blockquote>

At the FDA, I learned that trust in computational models requires more than code sharing. It requires documented VVUQ. Credibility means asking: Was the code solving the right equations? Were results compared to reality? Are the uncertainties understood? Commercial solvers often obscure these steps, and even open tools require deliberate infrastructure to capture and communicate them. 
Reproducibility supports credibility, but it’s not enough. Without VVUQ, teams can’t confidently interpret results. Without reproducibility, VVUQ becomes impossible to repeat. In my graduate lab, we manage post-processing code, data, and solver configs with care. But reproducibility still hinges on versioning, storage, and workflow management. Containerization offers a solution, but adoption remains slow due to complexity leading to alternative options such as workflow orchestration tools.

## We Must Prioritize Infrastructure for Credibility and Collaboration

<blockquote>
    Without investment in reproducible infrastructure, team-based modeling will remain unsustainable and error-prone. 
</blockquote>

Scientific software practices lag behind the needs of modern science. Too many workflows are rebuilt from scratch in each lab, and too few incentives support sustainable, collaborative software development. Building credible models should not depend on the character or trustworthiness of the researcher. We need ecosystems that treat infrastructure such as versioning, containers, and VVUQ workflows as necessary scientific outputs. 

To enable trustworthy, team-based modeling, funding agencies and institutions must invest in reproducible infrastructure and train scientists to use it. VVUQ should be taught alongside modeling, and transparent workflows should be the norm. Otherwise, each lost machine or graduating student sets science back.

## Conclusion 

To scale scientific computing, we must treat reproducibility and credibility as core pillars, not afterthoughts. Credibility and reproducibility are inseparable. Scientific computing will not scale to meet future challenges if we rely on black-box tools, untracked workflows, or fragile individual knowledge. The next generation of team-based ecosystems must build trust by design, through open tools, reproducible practices, and rigorous VVUQ.

