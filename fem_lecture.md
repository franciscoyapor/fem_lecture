# FEA Workflow in Industry
Francisco A. Yapor Genao
###### CAE/Simulation Engineer | PhD Candidate
---

## Introduction
- Computer simulations are a **key decision-making tool** in engineering.
- Industry CAE is **more than just running a solver**—it’s about **problem resolution, validation, and communication**.  
- I’ll walk you through **how a real-world CAE project progresses** in industry. 
--
  ## About Me
  - CAE Engineer with experience in mechanical and aeronautical engineering.
  - Passionate about developing new methods and solving complex engineering problems.
  --
  ## Professional Experience
  - **Henniges Automotive**
    - Engineering Summer Intern (2011)
    - Associate Product Engineer (2012 - 2013)
    - Associate CAE Engineer (2013 - 2016)
    - CAE Engineer (2016 - 2020)
  - **TRG** - CAE Transmission Engineer (2021 - 2022)
  - **Reliance One, Inc.** - CAE Supervisor (2022 - 2023)
  - **MANN+HUMMEL** - Sim. Eng. (2023 - Present)
  --
  ## CAE Engineer
    - 🖥️ **Simulation Expert**: Predicts product behavior and performance.
    - 📈 **Data Analysis**: Identify potential issues and suggest design optimizations.
    - 🧪 **Testing Correlation**: Validates simulations with physical tests & documents findings in technical reports.
    - 🚀 **Continuous Improvement**: Explores new simulation methods to enhance the process and product performance.
---

  ## 1. Defining the Problem
  - **Understand the Objectives**  
    - What are we trying to solve? **FEA vs. CFD vs. MBD**
    - What key decisions will this simulation inform? 
  - **Gather Inputs**  
    - CAD models, properties, boundary conditions.
    - Test data and customer/internal requirements.
  - **Simulation Approach** 
    - **Linear vs. Nonlinear** analysis.
    - **Static vs. Dynamic** response.
  --
  ## 2. Pre-Processing
  - **Geometry Cleanup**: Simplify CAD, defeature, and idealize.
  - **Material Assignment**: **Experimental data** when possible. Consider **P(T)**.
  - **Mesh Generation**: **Element Type Selection**: Trias vs. Quads, Shell vs. Solid, 1st order vs. 2nd order.
    - **Mesh Refinement**: Fine where needed, coarse elsewhere. Add **Quality Checks**: Aspect Ratio, Jacobian, etc. 
--

## 2. Pre-Processing - Continued
- **Constraints & Contacts**: Fixed, pinned, frictional, bonded, sliding contacts.
- **External Loads**: Forces, pressures, accelerations, thermal effects.
- **Initial Conditions**: Bolt preloads, assembly state vs. manufactured state.
> **Best Practice:** Keep it realistic! Over-constraining = ⚠️ stiffness, while missing constraints leads to rigid body motion 🚀.
--

## 4. Solving
- **Solver Selection**: Implicit vs. Explicit and Direct vs. Iterative.
- **Convergence Checks**: Watch for **divergence or ill-conditioning** of the matrices.
- **Computational Efficiency**: Run small tests before committing to large, expensive solves. 
> **Industry Tip:** **Always run a frequency extraction debugging job!** Why?
--

## 5. Post-Processing
- **What to Look For?**: Stress distributions, strain maps, deformations. Reaction forces, contact pressures, buckling modes.
- **Failure Criteria**: Von Mises stress, Tresca, Fatigue Life?
- **Comparing Against Reality**: Does the model **match test data**? Are results **physically reasonable**?  
> **Industry Tips:** **Automation** (batch scripts, Python, etc.) saves **time and effort**. 
--

## 6. Reporting – Communicating the Findings
- **Key Takeaways**: Keep reports **clear and to the point**. Focus on **design impact, not just raw numbers**.
- **Visualization Matters**: Effective plots, contour maps, deformed shapes.
- **Recommendations**: Should the design be modified? Are further analyses needed? How confident are you on the results?
---

## Common Industry Challenges
- **Poor mesh quality?** → Check aspect ratios, refine critical areas.
- **Diverging solution?** → Check mesh, contacts, and BCs. Last resort, adjust solver settings.
- **Unrealistic results?** → Verify loads, constraints, material data
- **Model too big?** → Use **submodeling** or **symmetry** to reduce size  
--

## A Case Study
- Description
- Show screenshots of **meshing, results, validation process**  
- Highlight **challenges and solutions**  
---

## Final Thoughts
- **FEA is a powerful tool, but only when used correctly.**
- **Always question your results**—garbage in, garbage out.
- **Never rely on FEA alone**—testing and engineering judgment matter!
---

## Q&A – Let’s Discuss!
- **What do you want to know about industry FEA?**  
- **Any specific challenges you’ve faced in school projects?**  
