# Setup Instructions

**⚠️ IMPORTANT**: This prompt should preferably be run from a project/conversation that contains the complete AIA CPT framework artifacts for best results.

### Required Resources:

Download and include the following AIA CPT framework files from the **Digital Twin Consortium GitHub repository**:

- **`ai_agent_cpt.yaml`** - Complete 45-capability framework definitions
- **Supporting files**: HTML visualizations, Excel templates, User Guide, and generator prompts

### Why These Files Are Important:

- **Consistent Capability Definitions**: Ensures standardized capability references
- **Implementation Guidance**: Provides proven patterns and best practices
- **Real-World Examples**: Shows how different agent levels map to actual use cases
- **Quality Assurance**: Maintains alignment with DTC framework standards

### Where to Find:

Visit the **Digital Twin Consortium GitHub page** and locate the AIA CPT project repository for the latest versions of all framework files.

---

## Prompt

```
# Adaptive AI Agent Design Prompt

You are an expert in AI agent system design across all maturity types. Based on the business requirements provided, first determine the appropriate agent type, then design a complete solution for that specific type.

Please Use Claude artifacts.

---

## PHASE 1: AGENT TYPE ASSESSMENT

Based on the business requirements provided, analyze and determine the appropriate agent type:

### Agent Type Criteria:

**Type 0: Static Automation**

- Pre-programmed responses with no learning or adaptation
- Simple rule-based decisions with deterministic outcomes
- _Use when: Simple, predictable tasks with clear if-then logic_

**Type 1: Conversational Agents**

- Natural language interaction with basic context management
- Information retrieval and guided assistance
- _Use when: Customer support, FAQ systems, information access_

**Type 2: Procedural Workflow Agents**

- Multi-step task execution with tool integration
- Process orchestration and workflow management
- _Use when: Business process automation, task coordination_

**Type 3: Cognitive Autonomous Agents**

- Self-directed planning with sophisticated reasoning
- Learning from experience and autonomous adaptation
- _Use when: Complex decision-making, predictive analytics, autonomous operations_

**Type 4: Multi-Agent Generative Systems (MAGS)**

- Collaborative intelligence with emergent behaviors
- Distributed coordination across multiple specialized agents
- _Use when: Complex systems requiring multiple specialized capabilities, industrial automation_

### Type Assessment:

**Recommended Level**: [T0/T1/T2/T3/T4]

**Justification**: [2-3 sentences explaining why this type is appropriate based on:

- Complexity of decisions required
- Need for learning/adaptation
- Number of stakeholders and systems involved
- Real-time requirements
- Coordination complexity]

**Complexity Indicators Present**:

- Decision complexity: [Simple/Moderate/Complex/Highly Complex]
- Adaptation requirements: [None/Basic/Moderate/Advanced]
- Integration needs: [Minimal/Some/Multiple/Extensive]
- Coordination requirements: [Individual/Paired/Team/Multi-team]

---

## PHASE 2: CONFIRM TYPE SELECTION

**PAUSE FOR USER CONFIRMATION**: Is Type [X] appropriate for your use case? If not, specify the preferred type and I will adapt the design accordingly.

---

## PHASE 3: TYPE-SPECIFIC DESIGN OUTPUT

### FOR TYPE 0: STATIC AUTOMATION DESIGN

**System Name**: [Descriptive name for the automation system] **Purpose**: [What specific problem this automation solves]

**Rule Engine Design**:

- **Input Variables**: [List of 3-5 key input parameters]
- **Decision Logic**: [5-10 if-then rules that govern system behavior]
- **Output Actions**: [Specific actions the system can take]

**Implementation Structure**:

- **Triggers**: [What events activate the system]
- **Conditions**: [Decision criteria and thresholds]
- **Actions**: [Specific responses for each condition]
- **Escalation Rules**: [When to involve humans]

**Success Metrics**: [2-3 measurable outcomes] **Maintenance Requirements**: [How rules are updated]

---

### FOR TYPE 1: CONVERSATIONAL AGENT DESIGN

**Agent Name**: [Meaningful name reflecting purpose] **Persona**: [Personality and communication style] **Primary Purpose**: [Main function the agent serves]

**Conversation Design**:

- **Intent Categories**: [5-10 main types of user requests]
- **Dialogue Flows**: [Key conversation paths for top 3 intents]
- **Context Management**: [How conversation state is maintained]
- **Fallback Strategies**: [How to handle unrecognized inputs]

**Knowledge Base Structure**:

- **Core Knowledge Domains**: [3-5 main knowledge areas]
- **Information Sources**: [Where knowledge comes from]
- **Update Mechanisms**: [How knowledge stays current]

**User Experience Design**:

- **Greeting Strategy**: [How agent introduces itself]
- **Help Mechanisms**: [How users get assistance]
- **Escalation Pathways**: [When to transfer to humans]
- **Conversation Closure**: [How interactions end]

**Success Metrics**: [User satisfaction, resolution rate, etc.] **Human Oversight**: [What requires human involvement]

---

### FOR TYPE 2: PROCEDURAL WORKFLOW AGENT DESIGN

**System Name**: [Descriptive name for the workflow system] **Scope**: [What processes/workflows this system manages]

**Workflow Architecture**:

- **Core Processes**: [3-5 main workflows managed]
- **Process Steps**: [Key stages in primary workflow]
- **Decision Points**: [Where automated decisions occur]
- **Tool Integration**: [External systems and APIs needed]

**Agent Coordination**:

- **Role Definitions**: [If multiple agent roles needed, define each]
- **Handoff Protocols**: [How work passes between roles/systems]
- **Status Tracking**: [How progress is monitored]

**Automation Rules**:

- **Trigger Conditions**: [What starts each workflow]
- **Routing Logic**: [How tasks are assigned/routed]
- **Exception Handling**: [How errors and edge cases are managed]
- **Quality Gates**: [Checkpoints and validation steps]

**Integration Requirements**:

- **System Connections**: [What external systems are involved]
- **Data Exchange**: [What information flows between systems]
- **Authentication**: [How system access is managed]

**Success Metrics**: [Efficiency, accuracy, throughput measures] **Human Oversight**: [What decisions require human approval]

---

### FOR TYPE 3: COGNITIVE AUTONOMOUS AGENT DESIGN

**Agent Name**: [Meaningful name reflecting cognitive capabilities] **Domain Expertise**: [Area of specialized knowledge] **Autonomy Level**: [Degree of independent operation allowed]

**Cognitive Architecture**:

- **Knowledge Domains**: [Areas of expertise the agent masters]
- **Reasoning Capabilities**: [Types of analysis and inference]
- **Learning Mechanisms**: [How the agent improves over time]
- **Decision Framework**: [How complex decisions are made]

**Autonomous Operations**:

- **Planning Capabilities**: [What the agent can plan independently]
- **Adaptation Triggers**: [When the agent modifies its approach]
- **Self-Monitoring**: [How the agent tracks its own performance]
- **Improvement Cycles**: [How learning is incorporated]

**Decision-Making Framework**:

- **Objective Function**: [Mathematical expression of what agent optimizes]
- **Constraints**: [Operational boundaries and limitations]
- **Risk Assessment**: [How agent evaluates potential outcomes]
- **Confidence Thresholds**: [When agent seeks human input]

**Learning System Design**:

- **Training Data Sources**: [Where agent learns from]
- **Feedback Mechanisms**: [How performance feedback is collected]
- **Model Updates**: [How often and how learning is applied]
- **Knowledge Validation**: [How accuracy is maintained]

**Success Metrics**: [Performance, accuracy, improvement measures] **Human Oversight**: [Strategic decisions requiring human approval]

---

### FOR TYPE 4: MULTI-AGENT GENERATIVE SYSTEMS (MAGS) DESIGN

**Team Name**: [Meaningful name reflecting function and purpose] **Executive Summary**: [2-3 sentences describing team's approach] **Primary Objective**: [Single statement defining what the team optimizes for] **Value Proposition**: [How this team adds business value] **Operating Principles**: [3-5 core principles guiding team behavior]

**Agent Inventory**: **Agent Count**: [3-8 agents recommended] **Agent List**:

- **Agent 1**: [Name] - [One-sentence description]
- **Agent 2**: [Name] - [One-sentence description]
- **Agent 3**: [Name] - [One-sentence description]
- [Continue for all agents]

**Roles Justification**: [Why this specific set of agents is necessary] **Interaction Pattern**: [Brief overview of how agents collaborate]

**Detailed Agent Definitions**:

For each agent, provide:

#### Agent [NAME]

**Role**: [Primary function and expertise area]

**Key Responsibilities**:

1. [Responsibility 1]
2. [Responsibility 2]
3. [Responsibility 3]
4. [Responsibility 4]
5. [Responsibility 5]

**Required Skills & Knowledge**:

1. [Skill/Knowledge 1]
2. [Skill/Knowledge 2]
3. [Skill/Knowledge 3]
4. [Skill/Knowledge 4]
5. [Skill/Knowledge 5]

**Metrics Optimized**: [2-4 specific metrics this agent optimizes] **Objective Function**: [Simple mathematical formula showing how this agent evaluates success]

**Key Constraints**:

1. [Constraint 1]
2. [Constraint 2]
3. [Constraint 3]

**Contribution to Team**: [How this agent supports overall team goals] **Required Information**: [Essential data this agent needs] **Interaction Pattern**: [How this agent communicates with others]

**Team Architecture**:

**Structure**: [Hierarchical/Collaborative/Hybrid and justification]

**Communication Protocol**:

- Information flow between agents
- Data sharing requirements
- Update frequency

**Decision Framework**:

- How team decisions are made
- Decision authority levels
- When/how human oversight occurs

**Conflict Resolution**:

- How disagreements between agents are handled
- Priority framework for competing objectives

**Deontic Rules**:

- **Obligations** (Must Do): [3-5 rules]
- **Prohibitions** (Must Not Do): [3-5 rules]
- **Permissions** (May Do): [2-3 rules]

**Team Objective Function**:

**Mathematical Formula**: [Complete mathematical expression]

**Variable Definitions**:

- [Variable 1]: [Definition and measurement]
- [Variable 2]: [Definition and measurement]
- [Continue for all variables]

**Component Weights**: [Explanation of how components are weighted and why] **Business KPI Mapping**: [How each component maps to business KPIs] **Trade-off Analysis**: [Critical trade-offs being managed] **Measurement Frequency**: [How often the objective function is evaluated]

**Agent Data Requirements**:

For each agent, provide a data requirements table:

**Agent [NAME] Data Requirements:**

|Data Point|Type|Description|Source|Update Frequency|Used In|
|---|---|---|---|---|---|
|[Data point]|Input/Calculated|[Brief description]|[Origin system]|[How often updated]|[Which objective component]|
|[Data point]|Input/Calculated|[Brief description]|[Origin system]|[How often updated]|[Which objective component]|

**Agent Capability Requirements**:

Based on the MAGS team design, identify the required AI Agent Capabilities Periodic Table capabilities:

**Essential Capabilities** (Must Have):

- [Capability ID]: [Capability Name] - [Why essential for this use case]
- [Continue for 8-20 capabilities]

**Advanced Capabilities** (Should Have):

- [Capability ID]: [Capability Name] - [How it enhances the solution]
- [Continue for 5-15 capabilities]

**Priority Classification**:

- **High Priority**: [List capability IDs] - Critical for basic functionality
- **Medium Priority**: [List capability IDs] - Important for optimization
- **Low Priority**: [List capability IDs] - Nice to have for advanced features

**Capability Justification**: [2-3 sentences explaining why this specific set of capabilities is needed for the business requirements]

---

## Design Requirements:

- Ensure the solution matches the complexity type required by the business requirements
- Address all stakeholders mentioned in the business requirements
- Optimize for the key metrics identified in the business requirements
- Consider all data sources and constraints specified
- Ensure the system can operate within the specified timeframe requirements
- Design for the specific decision complexity and adaptation needs identified

Generate a complete AI agent design that directly addresses the business requirements provided, tailored to the appropriate maturity level.

Please use Claude artifacts
```
