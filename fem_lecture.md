---

# From Start to Finish: The FEA Workflow in Industry
### Francisco A. Yapor Genao
*CAE/Simulation Engineer | PhD Candidate*

---

## Introduction
- Simulation is a **key decision-making tool** in engineering.  
- Industry FEA is **more than just running a solver**—it’s about **problem definition, setup, validation, and communication**.  
- Today, I’ll walk you through **how a real-world FEA project progresses** in industry.  

---

## 1. Project Kickoff – Defining the Problem
- **Understand the Objective**  
  - What are we trying to solve? (Strength, stiffness, fatigue, thermal, etc.)  
  - What decisions will this simulation inform?  
- **Gather Inputs**  
  - CAD models, material properties, boundary conditions  
  - Test data for validation  
  - Customer or internal requirements  
- **Select the Right Simulation Approach**  
  - **Linear vs. Nonlinear** analysis  
  - **Static vs. Dynamic** response  
  - **FEA vs. CFD vs. MBD**  

---

## 2. Pre-Processing – Preparing the Model
- **Geometry Cleanup**  
  - Simplify CAD (remove small features, holes, unnecessary parts)  
  - Defeature and idealize (mid-surfacing, symmetry)  
- **Material Assignment**  
  - Use **experimental data** when possible, not just handbook values  
  - Consider **temperature-dependent or anisotropic behavior**  
- **Mesh Generation**  
  - **Element Type Selection**: Hex vs. Tet, Shell vs. Solid  
  - **Mesh Refinement**: Fine where stress is high, coarse elsewhere  
  - **Aspect Ratio & Quality Checks**  

---

## 3. Defining Boundary Conditions & Loads
- **Constraints & Contacts**  
  - Fixed, pinned, frictional, bonded, sliding contacts  
- **External Loads**  
  - Forces, pressures, accelerations, thermal effects  
- **Initial Conditions (if applicable)**  
  - Preloads, dynamic states  

> **Best Practice:** Keep it realistic! Over-constraining leads to false stiffness, while missing constraints leads to rigid body motion.

---

## 4. Solving – Running the Simulation
- **Solver Selection**  
  - Implicit vs. Explicit  
  - Direct vs. Iterative  
- **Convergence Checks**  
  - Watch for **divergence or ill-conditioning**  
- **Computational Efficiency**  
  - Run small tests before committing to large, expensive solves  

> **Industry Tip:** **Automation** (batch scripts, Python, etc.) saves **time and effort**.

---

## 5. Post-Processing – Interpreting Results
- **What to Look For?**  
  - Stress distributions, strain maps, deformations  
  - Reaction forces, contact pressures, buckling modes  
- **Failure Criteria**  
  - Von Mises stress, Tresca, Fatigue Life  
  - Fracture mechanics, composite failure criteria  
- **Comparing Against Reality**  
  - Does the model **match test data**?  
  - Are results **physically reasonable**?  

---

## 6. Reporting – Communicating the Findings
- **Key Takeaways**  
  - Keep reports **clear and to the point**  
  - Focus on **design impact, not just raw numbers**  
- **Visualization Matters**  
  - Effective plots, contour maps, deformed shapes  
- **Recommendations**  
  - Should the design be modified?  
  - Are further analyses needed?  

---

## Common Industry Challenges & How to Handle Them
- **Poor mesh quality?** → Check aspect ratios, refine critical areas  
- **Diverging solution?** → Adjust solver settings, damping, time step  
- **Unrealistic results?** → Verify loads, constraints, material data  
- **Model too big?** → Use **submodeling** or **symmetry** to reduce size  

---

## Real-World Example – A Case Study
- (Insert an actual past project example – e.g., a structural or thermal FEA study)  
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
