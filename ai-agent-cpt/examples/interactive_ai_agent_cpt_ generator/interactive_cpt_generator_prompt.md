# Interactive AI Agent CPT Generator Prompt

## Instructions for User

Copy the entire prompt below and send it to any AI assistant (Claude, ChatGPT, Gemini, Llama, etc.) to generate an interactive AI Agent Capabilities Periodic Table HTML file with multiple use case examples and smooth filtering animations.

---

## UNIVERSAL PROMPT TO COPY:

```
You are an expert web developer. Generate a complete, self-contained HTML file for an interactive AI Agent Capabilities Periodic Table v1.0 that shows different use cases with smooth filtering animations. The output should include embedded CSS and JavaScript with no external dependencies.

## REQUIREMENTS:

### Visual Standards:
- Use the exact 45-capability framework with proper positioning
- Apply these category colors exactly:
  - PK (Perception & Knowledge): background #D1DCEA, border #7A9BC4, text #13386D
  - CG (Cognition & Reasoning): background #FAEAD5, border #D4A571, text #945911  
  - LA (Learning & Adaptation): background #E3DDEC, border #A18DB5, text #4E3D6F
  - AE (Action & Execution): background #EEEEEE, border #999999, text #404040
  - IC (Interaction & Collaboration): background #D5E3E1, border #7FA596, text #295548
  - GS (Governance & Safety): background #EDD9D5, border #C78275, text #792D21

### Interactive Features:
- Include 5 buttons: "All Capabilities", "Customer Service Bot", "Industrial MAGS", "Research Assistant", "Workflow Automation"
- Use smooth CSS transitions (0.3s ease-in-out) for capability show/hide
- Non-selected capabilities should fade to 20% opacity and scale to 95%
- Selected capabilities remain at 100% opacity and normal scale
- Buttons should have active/inactive states with blue highlighting for active button

### Layout Requirements:
- Use CSS Grid with 6 columns and 8 rows
- Include proper capability positioning as specified below
- Add legend showing all 6 categories with color samples
- Make responsive for mobile devices (stack to 3 columns on mobile)
- Center the content on the page
- Professional typography using system fonts

### Content Requirements:
- Page title: "AI Agent Capabilities Periodic Table v1.0"
- Interactive button row above the grid
- Include all 45 capability blocks with correct IDs and names
- Clean spacing and modern design

### CRITICAL - Exact Grid Positioning:
Use these exact positions for each capability:

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

### Use Case Capability Requirements:
Define these exact capability sets for each use case button:

**All Capabilities**: Show all 45 capabilities

**Customer Service Bot** (20 capabilities):
IC.NL, IC.DM, IC.HL, PK.KB, PK.CX, PK.MF, AE.CX, AE.TL, LA.MM, LA.RL, LA.SL, CG.DC, CG.RS, GS.SE, GS.PR, GS.EX, GS.MO, GS.ET, GS.RL, GS.DL

**Industrial MAGS** (24 capabilities):
IC.SI, IC.MB, IC.ES, IC.DS, IC.CS, IC.CF, IC.AC, IC.CL, PK.OB, PK.MF, PK.CX, CG.DC, CG.RS, CG.PS, CG.PL, LA.SL, LA.AD, LA.MM, LA.VM, AE.TX, AE.TL, AE.CG, GS.SF, GS.RL, GS.MO, GS.EV, GS.SE, GS.DL, GS.SC, GS.TC

**Research Assistant** (22 capabilities):
PK.KB, PK.OB, PK.CX, PK.MF, CG.RS, CG.PS, CG.PL, CG.DC, LA.MM, LA.SL, LA.VM, LA.MS, LA.AD, AE.CG, AE.CX, AE.TL, AE.TX, IC.NL, IC.DM, IC.HL, IC.AC, GS.EX, GS.ET, GS.RL, GS.MO, GS.EV, GS.PR

**Workflow Automation** (18 capabilities):
CG.PL, CG.PS, CG.DC, CG.PA, AE.TX, AE.TL, AE.TM, AE.MC, IC.AC, IC.CL, IC.RB, IC.ES, LA.MM, LA.RL, LA.AD, PK.KB, PK.CX, GS.MO, GS.EV, GS.DL, GS.SE, GS.SC, GS.RL

### Technical Requirements:
- Single HTML file with embedded CSS and JavaScript
- Use CSS Grid for layout positioning
- No external dependencies, CDN links, or external files
- Fast loading and responsive design
- Works offline after download
- Compatible with all modern browsers (Chrome, Firefox, Safari, Edge)
- Include hover effects for better interactivity
- Smooth animations for capability filtering

### JavaScript Functionality:
- Populate grid dynamically from capability data array
- Handle button clicks to filter capabilities
- Update active button styling
- Apply/remove "hidden" class with smooth transitions
- Track current use case state
- Initialize on page load

### Structure Requirements:
- Use semantic HTML5 structure
- Include proper meta tags for viewport and charset
- Use CSS classes for styling categories and states
- Add event listeners for button interactions
- Include a comprehensive legend section at the bottom
- Clean, modern design with proper spacing

Generate the complete HTML file code that creates an interactive periodic table where users can click buttons to see different use case capability requirements with smooth visual transitions.
```

---

## What You'll Get

After sending this prompt to any AI assistant, you'll receive:

✅ **Complete Interactive HTML** - Ready to save and use immediately  
✅ **5 Use Case Filters** - All Capabilities, Customer Service, Industrial MAGS, Research Assistant, Workflow Automation  
✅ **Smooth Animations** - Professional transitions when switching between use cases  
✅ **Comprehensive Examples** - Realistic capability requirements for each use case (18-24 capabilities each)  
✅ **Professional Design** - Enterprise-quality appearance with proper color scheme  
✅ **Mobile Responsive** - Works perfectly on desktop and mobile devices  
✅ **Self-Contained** - No external dependencies, works offline  

## Compatible AI Assistants

This prompt works with:
- **Claude** (Anthropic)
- **ChatGPT** (OpenAI)
- **Gemini** (Google)
- **Llama** (Meta/Various providers)
- **Other LLMs** with web development capabilities

## Key Features

### **Interactive Elements:**
- **Button filtering** - Click to show/hide capabilities for each use case
- **Smooth animations** - 0.3s transitions with opacity and scaling effects
- **Active states** - Clear visual feedback for selected use case
- **Hover effects** - Enhanced interactivity for better user experience

### **Realistic Use Cases:**
- **Customer Service Bot** (20 capabilities) - L1-L2 conversational agent with governance
- **Industrial MAGS** (24 capabilities) - L4 multi-agent system with full safety/coordination
- **Research Assistant** (22 capabilities) - L3 autonomous agent with advanced reasoning
- **Workflow Automation** (18 capabilities) - L2 procedural workflow with enterprise integration

### **Technical Quality:**
- Professional visual design with proper color scheme
- Responsive layout that works on all devices
- Fast loading and smooth performance
- Clean, modern interface suitable for business presentations

## Perfect For

- **Interactive presentations** - Demonstrate capability requirements live
- **Stakeholder education** - Show progression from simple to complex use cases
- **Requirements gathering** - Visual tool for defining system needs
- **Vendor evaluation** - Compare solutions against capability requirements
- **Training materials** - Educational tool for understanding AI agent levels

## Customization Options

You can modify the prompt to:
- **Add more use cases** - Include additional examples
- **Adjust capability counts** - Modify requirements for each use case
- **Change visual styling** - Specify different colors or layouts
- **Include tooltips** - Add detailed capability descriptions

This prompt generates a professional, interactive tool that transforms the static AI Agent CPT into an engaging, educational experience perfect for business presentations and stakeholder engagement!