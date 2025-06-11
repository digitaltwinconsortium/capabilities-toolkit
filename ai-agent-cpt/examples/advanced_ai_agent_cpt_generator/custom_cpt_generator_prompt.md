# Custom AI Agent CPT Generator Prompt

## Instructions for User

This prompt helps you create a customized AI Agent Capabilities Periodic Table for your specific use case. First, define your requirements using the questions below, then use the generated prompt with any AI assistant.

---

## STEP 1: DEFINE YOUR USE CASE

### Basic Information
**Answer these questions to customize your CPT:**

1. **What is your use case name?** (e.g., "Supply Chain Optimization", "Customer Service Automation", "Predictive Maintenance")

2. **What industry/domain?** (e.g., Manufacturing, Healthcare, Finance, Retail, Energy, Transportation)

3. **What maturity level are you targeting?**
   - L1: Conversational Agents (8-12 capabilities)
   - L2: Procedural Workflow (12-18 capabilities) 
   - L3: Cognitive Autonomous (18-25 capabilities)
   - L4: Multi-Agent Systems (25+ capabilities)

4. **What are your main objectives?** (e.g., reduce costs, improve efficiency, enhance safety, automate processes)

5. **Do you have specific capabilities in mind?** (Optional - see suggestions below)

### Capability Suggestions by Common Use Cases

**If you're unsure which capabilities you need, here are proven combinations:**

#### 🏭 **Smart Manufacturing**
*Suggested capabilities (22):* PK.OB, PK.MF, PK.CX, IC.SI, IC.MB, IC.ES, CG.DC, CG.RS, CG.PL, LA.SL, LA.AD, LA.VM, AE.TX, AE.TL, IC.AC, IC.CL, GS.SF, GS.RL, GS.MO, GS.SE, GS.EV, GS.DL

#### 🩺 **Healthcare Assistant**
*Suggested capabilities (18):* IC.NL, IC.DM, IC.HL, PK.KB, PK.CX, PK.MF, CG.RS, CG.DC, LA.MM, LA.SL, AE.CX, AE.TX, GS.SF, GS.PR, GS.ET, GS.EX, GS.RL, GS.SE

#### 💰 **Financial Planning**
*Suggested capabilities (16):* IC.NL, IC.DM, PK.KB, PK.CX, CG.RS, CG.PS, CG.DC, LA.SL, LA.MM, AE.CX, AE.TL, GS.SE, GS.PR, GS.ET, GS.EX, GS.TC

#### 🚛 **Supply Chain Optimization**
*Suggested capabilities (20):* PK.OB, PK.KB, PK.CX, CG.PL, CG.DC, CG.PS, LA.SL, LA.AD, LA.VM, AE.TX, AE.TL, IC.ES, IC.MB, IC.CL, GS.MO, GS.EV, GS.RL, GS.SE, GS.DL, GS.SC

#### 🎯 **Customer Experience**
*Suggested capabilities (14):* IC.NL, IC.DM, IC.HL, PK.KB, PK.CX, CG.DC, CG.RS, LA.MM, LA.RL, AE.CX, AE.TL, GS.PR, GS.ET, GS.EX

#### 🔒 **Cybersecurity Operations**
*Suggested capabilities (17):* PK.OB, PK.MF, CG.RS, CG.DC, CG.PS, LA.SL, LA.AD, LA.MM, AE.TX, AE.TL, IC.AC, IC.ES, GS.SE, GS.MO, GS.EV, GS.RL, GS.TC

#### 🏢 **Smart Building Management**
*Suggested capabilities (15):* PK.OB, PK.CX, IC.SI, IC.ES, CG.DC, CG.PL, LA.AD, LA.MM, AE.TX, AE.TL, IC.NL, GS.SF, GS.MO, GS.RL, GS.SE

#### 📊 **Business Intelligence**
*Suggested capabilities (19):* PK.KB, PK.OB, PK.CX, PK.MF, CG.RS, CG.PS, CG.DC, LA.SL, LA.VM, LA.MS, AE.CG, AE.CX, AE.TL, IC.NL, IC.DM, GS.EX, GS.EV, GS.PR, GS.TC

---

## STEP 2: UNIVERSAL CUSTOM CPT GENERATOR PROMPT

**Copy this prompt and replace the [BRACKETS] with your specific information:**

```
You are an expert web developer. Generate a complete, self-contained HTML file for a customized AI Agent Capabilities Periodic Table focused on [YOUR_USE_CASE_NAME]. The output should include embedded CSS and JavaScript with no external dependencies.

## CUSTOMIZATION REQUIREMENTS:

### Use Case Information:
- **Primary Use Case**: [YOUR_USE_CASE_NAME]
- **Industry/Domain**: [YOUR_INDUSTRY]
- **Target Maturity Level**: [YOUR_MATURITY_LEVEL]
- **Main Objectives**: [YOUR_OBJECTIVES]

### Visual Standards:
- Use the exact 45-capability framework with proper positioning
- Apply these category colors exactly:
  - PK (Perception & Knowledge): background #D1DCEA, border #7A9BC4, text #13386D
  - CG (Cognition & Reasoning): background #FAEAD5, border #D4A571, text #945911  
  - LA (Learning & Adaptation): background #E3DDEC, border #A18DB5, text #4E3D6F
  - AE (Action & Execution): background #EEEEEE, border #999999, text #404040
  - IC (Interaction & Collaboration): background #D5E3E1, border #7FA596, text #295548
  - GS (Governance & Safety): background #EDD9D5, border #C78275, text #792D21

### Custom Capability Selection:
**Required Capabilities for [YOUR_USE_CASE_NAME]:**
[LIST_YOUR_SPECIFIC_CAPABILITIES_HERE]

*If you didn't specify capabilities, use this suggested set: [SUGGESTED_CAPABILITIES_FROM_STEP_1]*

### Interactive Features:
- Include 4 view buttons: "All Capabilities", "[YOUR_USE_CASE_NAME]", "Essential Only", "Advanced Features"
- Essential Only: Show the 8-12 most critical capabilities for basic implementation
- Advanced Features: Show additional capabilities for sophisticated implementation
- Smooth CSS transitions (0.3s ease-in-out) for capability filtering
- Non-selected capabilities fade to 25% opacity
- Selected capabilities remain at 100% opacity with subtle highlight

### Content Requirements:
- Page title: "[YOUR_USE_CASE_NAME] - AI Agent CPT"
- Subtitle: "[YOUR_INDUSTRY] Implementation Guide"
- Include info section explaining why each capability is needed for your use case
- Add implementation priority indicators (High/Medium/Low) for each required capability

### CRITICAL - Use Standard Grid Positioning:
Follow the exact 45-capability positioning as in the standard framework:

**Perception & Knowledge (PK) - Column 1:**
- PK.OB "Environmental Sensing" at row 3, column 1
- PK.KB "Knowledge Access" at row 4, column 1
- PK.CX "Context & Memory" at row 5, column 1
- PK.MF "Multi-Modal Fusion" at row 6, column 1

**Cognition & Reasoning (CG) - Column 2:**
- CG.PL "Planning & Decomposition" at row 1, column 2
- CG.RS "Reasoning" at row 2, column 2
- CG.DC "Decision Making" at row 3, column 2
- CG.PS "Problem Solving" at row 4, column 2
- CG.PP "Formal Planning" at row 5, column 2
- CG.PA "Plan Adaptation" at row 6, column 2

**Learning & Adaptation (LA) - Column 3:**
- LA.MM "Memory Management" at row 1, column 3
- LA.RL "Reinforcement Learning" at row 2, column 3
- LA.AD "Self-Optimization" at row 3, column 3
- LA.SL "Supervised Learning" at row 4, column 3
- LA.VM "Vector Memory" at row 5, column 3
- LA.MS "Memory Scoring" at row 6, column 3

**Action & Execution (AE) - Column 4:**
- AE.TX "Task Execution & Implementation" at row 2, column 4
- AE.TL "Tool Usage & API Integration" at row 3, column 4
- AE.CG "Code Generation & Execution" at row 4, column 4
- AE.CX "Content Creation & Generation" at row 5, column 4
- AE.TM "Tool Lifecycle Management" at row 6, column 4
- AE.MC "MCP Integration" at row 7, column 4

**Interaction & Collaboration (IC) - Columns 5-6:**
- IC.NL "Natural Language" at row 1, column 5
- IC.DM "Dialogue Management" at row 2, column 5
- IC.HL "Human-in-Loop" at row 3, column 5
- IC.AC "Agent Communication" at row 4, column 5
- IC.CL "Collaboration" at row 5, column 5
- IC.RB "Role Behavior" at row 6, column 5
- IC.CS "Consensus Protocols" at row 1, column 6
- IC.CF "Conflict Resolution" at row 2, column 6
- IC.SI "Industrial Integration" at row 3, column 6
- IC.ES "Enterprise Integration" at row 4, column 6
- IC.MB "Message Brokers" at row 5, column 6
- IC.DS "Distributed Coordination" at row 6, column 6

**Governance & Safety (GS) - Rows 7-8:**
- GS.DL "Deployment Management" at row 7, column 1
- GS.MO "Monitoring" at row 7, column 2
- GS.EV "Evaluation" at row 7, column 3
- GS.ET "Ethics" at row 7, column 5
- GS.PR "Privacy" at row 7, column 6
- GS.SC "Scaling" at row 8, column 1
- GS.SF "Safety" at row 8, column 2
- GS.SE "Security" at row 8, column 3
- GS.EX "Explainability" at row 8, column 4
- GS.RL "Reliability" at row 8, column 5
- GS.TC "Trust Management" at row 8, column 6

### Use Case-Specific Features:
Add these custom elements:

**Implementation Guidance Panel:**
- Show why each required capability is needed for [YOUR_USE_CASE_NAME]
- Include implementation priority levels (High/Medium/Low)
- Add estimated complexity scores for each capability
- Provide next steps and recommendations

**Custom Filtering Views:**
- **All Capabilities**: Show complete 45-capability framework
- **[YOUR_USE_CASE_NAME]**: Show only capabilities needed for your use case
- **Essential Only**: Show minimum viable capabilities (8-12 most critical)
- **Advanced Features**: Show additional capabilities for enhanced implementation

### Custom Descriptions:
For each required capability, explain specifically how it applies to [YOUR_USE_CASE_NAME]. For example:
- If IC.NL is required: "Natural Language processing enables [specific application in your use case]"
- If PK.OB is required: "Environmental Sensing allows [specific monitoring/detection needs]"
- If GS.SF is required: "Safety Management ensures [specific safety requirements]"

### Technical Requirements:
- Single HTML file with embedded CSS and JavaScript
- Professional appearance suitable for business presentations
- Mobile responsive design
- Fast loading and smooth animations
- No external dependencies
- Compatible with all modern browsers

Generate a complete, customized HTML file that creates an interactive periodic table specifically focused on [YOUR_USE_CASE_NAME] with relevant capability selection, implementation guidance, and industry-specific context.
```

---

## STEP 3: EXAMPLE COMPLETED PROMPTS

### Example A: Smart Manufacturing
```
[Replace with your specifics]
- Primary Use Case: Predictive Equipment Maintenance
- Industry/Domain: Manufacturing
- Target Maturity Level: L3 - Cognitive Autonomous
- Main Objectives: Reduce downtime, optimize maintenance schedules, improve equipment reliability
- Required Capabilities: PK.OB, PK.MF, PK.CX, IC.SI, IC.ES, CG.RS, CG.DC, CG.PS, LA.SL, LA.AD, LA.MM, AE.TX, AE.TL, GS.SF, GS.RL, GS.MO, GS.SE, GS.EV
```

### Example B: Healthcare
```
[Replace with your specifics]
- Primary Use Case: Clinical Decision Support
- Industry/Domain: Healthcare
- Target Maturity Level: L2 - Procedural Workflow
- Main Objectives: Improve diagnostic accuracy, reduce medical errors, enhance patient safety
- Required Capabilities: IC.NL, IC.DM, IC.HL, PK.KB, PK.CX, CG.RS, CG.DC, LA.MM, LA.SL, AE.CX, GS.SF, GS.PR, GS.ET, GS.EX, GS.RL, GS.SE
```

---

## CUSTOMIZATION OPTIONS

### Visual Customization:
- Add your company logo and branding colors
- Include industry-specific icons or imagery
- Customize the color scheme while maintaining readability
- Add your company's implementation methodology

### Content Customization:
- Include your specific business requirements
- Add regulatory compliance needs for your industry
- Include integration requirements with your existing systems
- Add ROI calculations and business case information

### Functional Customization:
- Add capability priority scoring based on your needs
- Include implementation timeline and phases
- Add cost estimates for each capability
- Include vendor evaluation criteria

This prompt generator creates a **tailored, business-ready CPT** that speaks directly to your specific use case, industry requirements, and implementation goals!