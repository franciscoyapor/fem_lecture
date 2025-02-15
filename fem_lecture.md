# FEA Workflow in Industry
Francisco A. Yapor Genao
###CAE/Simulation Engineer | PhD Candidate
---

## Introduction
- Computer simulations are a **key decision-making tool** in engineering.
- Industry CAE is **more than just running a solver**—it’s about **problem resolution, validation, and communication**.  
- I’ll walk you through **how a real-world CAE project progresses** in industry.  
---

## About Me
- I am a CAE Engineer with experience in mechanical and aeronautical engineering.
- Passionate about developing new methods and solving complex engineering problems.
--
## Educational Journey
- **B.Sc. in Aeronautical Engineering**  (2008 - 2012)
- **M.Sc. in Mechanical Engineering**    (2016 - 2018)
- **Ph.D. in Mechanical Engineering**    (In Progress)

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
## Product Engineer
- Owns the product and defines product specifications
- Provides manufacturing support and testing/validation
- Continuous improvement and product management
- Documentation and compliance
--
## CAE Engineer

- 🖥️ **Simulation Expert**: Performs computer simulations to predict product behavior and performance.
- 📈 **Data Analysis**: Analyzes simulation results to identify potential issues and suggest design optimization.
- 🧪 **Testing Correlation**: Validates simulations by comparing them with physical test data to ensure model accuracy.
--
- 🛠 **Design Support**: Collaborates with product engineers to integrate simulation feedback into design improvements.
- 📋 **Detailed Reporting**: Documents findings in technical reports, highlighting critical insights and recommendations for product development.
- 🚀 **Continuous Improvement**: Researches new simulation tools and methods to enhance the simulation process and product performance.

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
