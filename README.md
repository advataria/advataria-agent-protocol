# Advataria: Autonomous AI Advertising Swarm

### 🏗 Architecture Overview
Advataria operates as a multi-agent system designed to automate the entire lifecycle of video advertising—from initial brand research to final client delivery.

We have digitized the core roles of a creative studio. Unlike linear automation scripts, our architecture utilizes **5 Specialized Autonomous Agents** that act as a cohesive workforce, effectively replacing the traditional agency headcount with software.

### 🤖 The "Agency in a Box" Architecture

```mermaid
graph TD
    %% Styles
    classDef startend fill:#98fb98,stroke:#333,stroke-width:2px,color:black;
    classDef agent fill:#fffacd,stroke:#d4af37,stroke-width:2px,color:black,font-weight:bold;

    %% Nodes
    S((START)):::startend
    A1["Agent 01:<br/>THE STRATEGIST<br/>(Research)"]:::agent
    A2["Agent 02:<br/>CREATIVE DIRECTOR<br/>(Strategy)"]:::agent
    A3["Agent 03:<br/>LEAD COPYWRITER<br/>(Scripting)"]:::agent
    A4["Agent 04:<br/>EXECUTIVE PRODUCER<br/>(Video Gen)"]:::agent
    A5["Agent 05:<br/>ACCOUNT DIRECTOR<br/>(Sales)"]:::agent
    E((END)):::startend

    %% Connections
    S -->|URL Data| A1
    A1 -->|Market Insights| A2
    A2 -->|Creative Brief| A3
    A3 -->|Final Script| A4
    A4 -->|Rendered Ad| A5
    A5 --> E

