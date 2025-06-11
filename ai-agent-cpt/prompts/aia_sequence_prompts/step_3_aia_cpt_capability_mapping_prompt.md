# AIA CPT HTML Visualization Generator

## Setup Instructions

**⚠️ IMPORTANT**: This prompt should be run from a project/conversation that contains the complete AIA CPT framework artifacts and your capability mapping output.

### Required Input:

This prompt requires the **complete output** from the **AIA CPT Capability Mapping Prompt**, including:

- Essential, Advanced, and Optional capabilities with justifications
- Priority classifications (High/Medium/Low)
- Implementation roadmap and business context
- Agent design details and use case description

---

## Prompt

````prompt
You are an expert web developer specializing in interactive data visualizations. Generate a complete, self-contained HTML file that creates a customized AI Agent Capabilities Periodic Table visualization based on the capability mapping provided.

## HTML Generation Requirements

### Visual Design Standards:

- **Professional Theme**: Use colors and styling appropriate for the business domain
- **Category Colors**: Apply standard AIA CPT category colors:
    - PK (Perception & Knowledge): background #D1DCEA, border #7A9BC4, text #13386D
    - CG (Cognition & Reasoning): background #FAEAD5, border #D4A571, text #945911
    - LA (Learning & Adaptation): background #E3DDEC, border #A18DB5, text #4E3D6F
    - AE (Action & Execution): background #EEEEEE, border #999999, text #404040
    - IC (Interaction & Collaboration): background #D5E3E1, border #7FA596, text #295548
    - GS (Governance & Safety): background #EDD9D5, border #C78275, text #792D21

### Header Section:

- **Title**: Use case name with relevant emoji
- **Subtitle**: "[Industry] Implementation Guide - AI Agent Capabilities Periodic Table"
- **Description**: Agent type, capability count, and brief value proposition
- **Theme**: Background gradient and colors appropriate to the industry/domain

### Interactive Controls:

Generate 4 filter buttons:

- **"All Capabilities"**: Shows complete 45-capability framework
- **"[Use Case Name]"**: Shows only capabilities from the mapping (Essential + Advanced)
- **"Essential Only"**: Shows only essential/must-have capabilities
- **"Advanced Features"**: Shows only advanced/should-have capabilities

### Periodic Table Grid:

- **Standard Layout**: Use exact 6x8 grid positioning from AIA CPT framework
- **Capability Selection**: Mark capabilities as selected/hidden based on mapping output
- **Priority Indicators**: Add colored dots for High (red), Medium (orange), Low (green) priority
- **Essential Marking**: Thicker borders for essential capabilities
- **Hover Effects**: Professional animations and interactions

### CRITICAL - Exact Grid Positioning Matrix:

Use these exact CSS grid positions for each capability:

**Perception & Knowledge (PK) - Column 1:**

- PK.OB "Environmental Sensing": `grid-column: 1; grid-row: 3;` (pos-3-1)
- PK.KB "Knowledge Access": `grid-column: 1; grid-row: 4;` (pos-4-1)
- PK.CX "Context & Memory": `grid-column: 1; grid-row: 5;` (pos-5-1)
- PK.MF "Multi-Modal Fusion": `grid-column: 1; grid-row: 6;` (pos-6-1)

**Cognition & Reasoning (CG) - Column 2:**

- CG.PL "Planning & Decomposition": `grid-column: 2; grid-row: 1;` (pos-1-2)
- CG.RS "Reasoning": `grid-column: 2; grid-row: 2;` (pos-2-2)
- CG.DC "Decision Making": `grid-column: 2; grid-row: 3;` (pos-3-2)
- CG.PS "Problem Solving": `grid-column: 2; grid-row: 4;` (pos-4-2)
- CG.PP "Formal Planning": `grid-column: 2; grid-row: 5;` (pos-5-2)
- CG.PA "Plan Adaptation": `grid-column: 2; grid-row: 6;` (pos-6-2)

**Learning & Adaptation (LA) - Column 3:**

- LA.MM "Memory Management": `grid-column: 3; grid-row: 1;` (pos-1-3)
- LA.RL "Reinforcement Learning": `grid-column: 3; grid-row: 2;` (pos-2-3)
- LA.AD "Self-Optimization": `grid-column: 3; grid-row: 3;` (pos-3-3)
- LA.SL "Supervised Learning": `grid-column: 3; grid-row: 4;` (pos-4-3)
- LA.VM "Vector Memory": `grid-column: 3; grid-row: 5;` (pos-5-3)
- LA.MS "Memory Scoring": `grid-column: 3; grid-row: 6;` (pos-6-3)

**Action & Execution (AE) - Column 4:**

- AE.TX "Task Execution & Implementation": `grid-column: 4; grid-row: 2;` (pos-2-4)
- AE.TL "Tool Usage & API Integration": `grid-column: 4; grid-row: 3;` (pos-3-4)
- AE.CG "Code Generation & Execution": `grid-column: 4; grid-row: 4;` (pos-4-4)
- AE.CX "Content Creation & Generation": `grid-column: 4; grid-row: 5;` (pos-5-4)
- AE.TM "Tool Lifecycle Management": `grid-column: 4; grid-row: 6;` (pos-6-4)
- AE.MC "MCP Integration": `grid-column: 4; grid-row: 7;` (pos-7-4)

**Interaction & Collaboration (IC) - Columns 5-6:**

- IC.NL "Natural Language": `grid-column: 5; grid-row: 1;` (pos-1-5)
- IC.DM "Dialogue Management": `grid-column: 5; grid-row: 2;` (pos-2-5)
- IC.HL "Human-in-Loop": `grid-column: 5; grid-row: 3;` (pos-3-5)
- IC.AC "Agent Communication": `grid-column: 5; grid-row: 4;` (pos-4-5)
- IC.CL "Collaboration": `grid-column: 5; grid-row: 5;` (pos-5-5)
- IC.RB "Role Behavior": `grid-column: 5; grid-row: 6;` (pos-6-5)
- IC.CS "Consensus Protocols": `grid-column: 6; grid-row: 1;` (pos-1-6)
- IC.CF "Conflict Resolution": `grid-column: 6; grid-row: 2;` (pos-2-6)
- IC.SI "Industrial Integration": `grid-column: 6; grid-row: 3;` (pos-3-6)
- IC.ES "Enterprise Integration": `grid-column: 6; grid-row: 4;` (pos-4-6)
- IC.MB "Message Brokers": `grid-column: 6; grid-row: 5;` (pos-5-6)
- IC.DS "Distributed Coordination": `grid-column: 6; grid-row: 6;` (pos-6-6)

**Governance & Safety (GS) - Rows 7-8:**

- GS.DL "Deployment Management": `grid-column: 1; grid-row: 7;` (pos-7-1)
- GS.MO "Monitoring": `grid-column: 2; grid-row: 7;` (pos-7-2)
- GS.EV "Evaluation": `grid-column: 3; grid-row: 7;` (pos-7-3)
- GS.ET "Ethics": `grid-column: 5; grid-row: 7;` (pos-7-5)
- GS.PR "Privacy": `grid-column: 6; grid-row: 7;` (pos-7-6)
- GS.SC "Scaling": `grid-column: 1; grid-row: 8;` (pos-8-1)
- GS.SF "Safety": `grid-column: 2; grid-row: 8;` (pos-8-2)
- GS.SE "Security": `grid-column: 3; grid-row: 8;` (pos-8-3)
- GS.EX "Explainability": `grid-column: 4; grid-row: 8;` (pos-8-4)
- GS.RL "Reliability": `grid-column: 5; grid-row: 8;` (pos-8-5)
- GS.TC "Trust Management": `grid-column: 6; grid-row: 8;` (pos-8-6)

**CSS Class Implementation:**

```css
.pos-X-Y { grid-column: Y; grid-row: X; }
```

**HTML Structure for Each Capability:**

```html
<div class="capability [category] pos-X-Y [selected/hidden] [essential]" data-code="[CAP.ID]" data-priority="[high/medium/low]">
    <div class="capability-code">[CAP.ID]</div>
    <div class="capability-name">[Capability Name]</div>
    <div class="priority-indicator priority-[high/medium/low]"></div>
</div>
```

### Content Sections:

#### 1. Challenge Overview Section:

**Title**: "🎯 The [Domain] Challenge" Generate 2-3 subsections explaining:

- **Critical Decision Problem**: What specific business problem this solves
- **Multi-Agent Conflicts** (if Type 4): Realistic conflict scenarios requiring consensus
- **Complex Integration** (if Type 2+): Systems and data sources that must be integrated

#### 2. Architecture Rationale Section (if Type 2+):

**Title**: "🤖 Why Type [X] [Architecture Type]?" Generate subsections explaining:

- **Specialized Roles** (if Type 4): Individual agent responsibilities
- **Decision Timeframes**: Different time horizons for different decisions
- **Coordination Requirements**: Why this type of sophistication is needed

#### 3. Implementation Guidance Section:

**Title**: "🎯 Implementation Guidance for [Use Case]" Generate 4-6 implementation guide cards covering:

- **Critical Safety/Governance**: Essential GS capabilities and why they matter
- **[Level]-Specific Architecture**: Key capabilities for the identified level
- **Data Integration**: PK and IC capabilities for system connectivity
- **Decision Intelligence**: CG and LA capabilities for smart automation
- **System Control**: AE capabilities for execution and control
- **Measurable Impact**: Quantified business benefits and KPIs

### Detailed Capability Descriptions:

For each capability in the mapping, generate contextual descriptions explaining:

- **Specific Application**: How this capability applies to this exact use case
- **Business Value**: Quantified impact (costs saved, efficiency gained, risks mitigated)
- **Implementation Context**: Technical details about how it works in this domain
- **Integration Points**: How it connects with other systems and capabilities

### JavaScript Functionality:

- **View Switching**: Smooth transitions between capability sets
- **Priority Indicators**: Visual priority dots on each capability
- **Click Interactions**: Detailed popups with capability explanations
- **Responsive Design**: Mobile-friendly layout adaptation

### Footer:

- **Attribution**: "Powered by Digital Twin Consortium - AI Agent Capabilities Framework"
- **Professional Styling**: Clean, understated design

---

## Content Generation Guidelines:

### Industry-Specific Theming:

Apply subtle, professional theming appropriate to the business domain:

- **Manufacturing**: Subtle steel blues `linear-gradient(135deg, #2c3e50 0%, #34495e 100%)`, 🏭⚙️🔧 emojis, SCADA/OT focus
- **Healthcare**: Soft medical blues `linear-gradient(135deg, #2980b9 0%, #3498db 100%)`, 🏥⚕️🩺 emojis, patient safety focus
- **Finance**: Professional navy/grays `linear-gradient(135deg, #2c3e50 0%, #2980b9 100%)`, 💰📊💳 emojis, risk management focus
- **Energy**: Understated energy tones `linear-gradient(135deg, #27ae60 0%, #2ecc71 100%)`, ⚡🔋🌱 emojis, grid/sustainability focus
- **Transportation**: Muted movement blues `linear-gradient(135deg, #2980b9 0%, #16a085 100%)`, 🚛✈️🚢 emojis, logistics focus
- **Water/Utilities**: Deep water blues `linear-gradient(135deg, #003952 0%, #004f6b 100%)`, 🌊💧⚡ emojis, infrastructure focus
- **Smart Cities**: Urban grays/blues `linear-gradient(135deg, #34495e 0%, #2c3e50 100%)`, 🏙️🌐📡 emojis, urban systems focus
- **Default**: Clean professional `linear-gradient(135deg, #2c3e50 0%, #3498db 100%)`, 🤖⚙️📊 emojis, technology focus

**Color Guidelines**:

- Use subtle gradients that don't overpower the content
- Maintain high contrast for readability
- Keep backgrounds professional and understated
- Ensure capability blocks remain clearly visible
- Use industry emojis sparingly in titles and section headers only

### Realistic Business Context:

- **Quantified Metrics**: Include specific dollar amounts, percentages, timeframes
- **Real Systems**: Reference actual technologies (SCADA, SAP, APIs, protocols)
- **Actual Constraints**: Regulatory requirements, safety standards, performance targets
- **Measurable Outcomes**: ROI calculations, efficiency improvements, risk reduction

### Technical Depth:

- **Integration Details**: Specific protocols, APIs, and system connections
- **Performance Specs**: Response times, accuracy requirements, reliability targets
- **Scaling Requirements**: User counts, transaction volumes, system capacity
- **Compliance Needs**: Industry regulations, security standards, audit requirements

### Type-Appropriate Complexity:

- **T1**: Focus on conversation design, knowledge access, basic safety
- **T2**: Emphasize workflow coordination, tool integration, process management
- **T3**: Highlight autonomous reasoning, learning, sophisticated decision-making
- **T4**: Detail multi-agent coordination, consensus protocols, distributed intelligence

---

## Quality Requirements:

### Technical Excellence:

- **Single HTML File**: Complete, self-contained with embedded CSS/JavaScript
- **No Dependencies**: Works offline, no external CDN links or resources
- **Cross-Browser Compatible**: Functions in all modern browsers
- **Mobile Responsive**: Adapts to different screen sizes
- **Fast Loading**: Optimized performance and smooth animations

### Content Quality:

- **Accurate Mapping**: All capabilities from input mapping correctly represented
- **Business Relevance**: Content directly addresses the specific use case requirements
- **Technical Credibility**: Realistic technical details and implementation context
- **Professional Presentation**: Suitable for executive and stakeholder presentations

### Visual Polish:

- **Consistent Design**: Professional appearance throughout
- **Smooth Interactions**: High-quality animations and transitions
- **Clear Information Hierarchy**: Easy to scan and understand
- **Appropriate Complexity**: Matches the sophistication level of the use case

Generate a complete, professional HTML file that transforms the capability mapping into an engaging, interactive visualization that clearly communicates the value and implementation approach for this specific AI agent use case.
````
