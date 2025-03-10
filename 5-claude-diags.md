# Detailed Diagrams for the BARLI Experiment

## Diagram Descriptions

Following is a comprehensive set of diagrams to visualize the Bio-Artificial Reward Learning with Integrated Qualia Mapping (BARLI) framework. Each diagram captures different aspects of this complex experiment:

1. **BARLI Framework Overview**: Shows the main components of the experiment, including the biological system (rat), artificial system (AI), bi-directional interface, and experimental environment, along with their interconnections.

```mermaid
graph TD
    subgraph "Biological System (Rat)"
        BS1[Brain Regions of Interest]
        BS2[Neural Recording System]
        BS3[Neural Stimulation System]
        BS4[Behavioral Monitoring]
        
        BS1 --- BS2
        BS1 --- BS3
        BS1 --- BS4
    end
    
    subgraph "Artificial System (AI)"
        AS1[AI Agent Architecture]
        AS2[Simulated Pleasure Circuit]
        AS3[Quantum Sentience Platform]
        AS4[Internal State Representation]
        
        AS1 --- AS2
        AS1 --- AS3
        AS1 --- AS4
    end
    
    subgraph "Bi-Directional Interface"
        BDI1[Neural Decoder]
        BDI2[Neural Encoder]
        
        BDI1 --- BDI2
    end
    
    subgraph "Experimental Environment"
        EE1[Virtual Navigation Environment]
        EE2[Decision-Making Tasks]
        EE3[Reward Processing Tasks]
        
        EE1 --- EE2
        EE1 --- EE3
    end
    
    BS2 -->|Neural Activity| BDI1
    BDI1 -->|Reward Signal| AS1
    AS1 -->|AI State| BDI2
    BDI2 -->|Stimulation Parameters| BS3
    
    BS4 -->|Behavioral Data| DA1
    AS4 -->|Internal State Data| DA1
    
    subgraph "Data Analysis"
        DA1[Cross-System Comparison]
        DA2[Integrated Information Metrics]
        DA3[Neural Signatures Analysis]
        
        DA1 --- DA2
        DA1 --- DA3
    end
    
    EE1 -->|Task Environment| BS1
    EE1 -->|Virtual Environment| AS1
```



2. **Biological System: Rat Neural Circuits**: Illustrates the brain regions of interest (MFB, NAc, VTA, etc.), neural recording techniques, stimulation methods, neurochemical monitoring, and behavioral assessment approaches.


```mermaid
graph LR
    subgraph "Brain Regions of Interest"
        MFB[Medial Forebrain Bundle]
        NAc[Nucleus Accumbens]
        VTA[Ventral Tegmental Area]
        OFC[Orbitofrontal Cortex]
        ACC[Anterior Cingulate Cortex]
        IC[Insular Cortex]
        
        VTA -->|Dopaminergic Projections| NAc
        VTA --> MFB
        MFB --> NAc
        NAc --> OFC
        OFC --> NAc
        ACC --- NAc
        IC --- NAc
    end
    
    subgraph "Neural Recording"
        NR1[High-density Silicon Probes]
        NR2[384 Channels per Probe]
        NR3[30 kHz Sampling Rate]
        NR4[Single-Unit Activity]
        NR5[Local Field Potentials]
        
        NR1 --- NR2
        NR1 --- NR3
        NR1 --- NR4
        NR1 --- NR5
    end
    
    subgraph "Neural Stimulation"
        NS1[Optogenetic Stimulation]
        NS2[Chemogenetic Modulation]
        NS3[Electrical Microstimulation]
        
        NS1 -->|Blue Light 470nm| VTA
        NS2 -->|CNO Activation| NAc
        NS3 -->|Biphasic Pulses| MFB
    end
    
    subgraph "Neurochemical Monitoring"
        NCM1[Microdialysis]
        NCM2[Fiber Photometry]
        
        NCM1 -->|Dopamine, Serotonin, Endorphin Levels| NAc
        NCM2 -->|Fluorescent Monitoring| VTA
    end
    
    subgraph "Behavioral Monitoring"
        BM1[3D Video Tracking]
        BM2[Ultrasonic Vocalization Recording]
        BM3[Physiological Measures]
        BM4[Choice Behavior]
        
        BM1 --- BM2
        BM1 --- BM3
        BM1 --- BM4
    end
```


3. **Artificial System: AI Architecture**: Details the AI agent's structure, including value networks, policy networks, world models, simulated pleasure circuits, and internal state representations.


```mermaid
graph LR
    subgraph "Core AI Architecture"
        AI1[Value Network]
        AI2[Policy Network]
        AI3[World Model]
        AI4[Meta-Controller]
        
        AI1 <--> AI2
        AI1 <--> AI3
        AI2 <--> AI3
        AI4 -->|Controls| AI1
        AI4 -->|Controls| AI2
        AI4 -->|Controls| AI3
    end
    
    subgraph "Simulated Pleasure Circuit"
        SPC1[Neural Simulation]
        SPC2[Neurotransmitter Simulation]
        SPC3[Biophysical Models]
        
        SPC1 --- SPC2
        SPC1 --- SPC3
        
        SPC1_1[Hodgkin-Huxley Neuron Models]
        SPC1_2[Population Dynamics]
        SPC1_3[Inter-region Connectivity]
        
        SPC1 --- SPC1_1
        SPC1 --- SPC1_2
        SPC1 --- SPC1_3
        
        SPC2_1[Dopamine Dynamics]
        SPC2_2[Serotonergic Modulation]
        SPC2_3[Opioid System]
        SPC2_4[Glu/GABA Balance]
        
        SPC2 --- SPC2_1
        SPC2 --- SPC2_2
        SPC2 --- SPC2_3
        SPC2 --- SPC2_4
    end
    
    subgraph "Internal State Representation"
        ISR1[Reward Representation]
        ISR2[Memory Systems]
        ISR3[Temporal Integration]
        
        ISR1 --- ISR2
        ISR1 --- ISR3
        
        ISR1_1[Hedonic Value]
        ISR1_2[Arousal/Intensity]
        ISR1_3[Novelty/Surprise]
        ISR1_4[Social/Contextual Relevance]
        
        ISR1 --- ISR1_1
        ISR1 --- ISR1_2
        ISR1 --- ISR1_3
        ISR1 --- ISR1_4
        
        ISR2_1[Working Memory]
        ISR2_2[Episodic Memory]
        ISR2_3[Semantic Knowledge]
        
        ISR2 --- ISR2_1
        ISR2 --- ISR2_2
        ISR2 --- ISR2_3
    end
    
    subgraph "Training Algorithm"
        TA1[PPO]
        TA2[Intrinsic Motivation]
        
        TA1 --- TA2
    end
    
    SPC1 -->|Activation Patterns| AI1
    ISR1 -->|Reward Dimensions| AI1
    AI2 -->|Action Selection| ENV[Environment]
    ENV -->|State Observations| AI3
    AI1 -->|Value Estimation| AI2
```



4. **Bi-Directional Interface: Neural-AI Communication**: Shows the sequential flow of information between the rat brain and AI system through neural decoders and encoders, highlighting the closed-loop nature of the experiment.

```mermaid
sequenceDiagram
    participant R as Rat Brain
    participant ND as Neural Decoder
    participant AI as AI Agent
    participant NE as Neural Encoder
    participant S as Stimulation System
    
    Note over R,S: Bi-Directional Communication Cycle
    
    R->>ND: Neural activity from reward circuits
    Note right of ND: Signal preprocessing<br>Feature extraction<br>Spike sorting<br>LFP analysis
    
    ND->>ND: Apply ensemble decoding algorithms
    Note right of ND: Linear decoders<br>Non-linear decoders<br>Deep neural networks
    
    ND->>AI: Translated reward signal
    Note right of AI: Multi-dimensional reward representation<br>(valence, intensity, surprise, etc.)
    
    AI->>AI: Process reward and update internal state
    Note right of AI: Update value function<br>Adjust policy<br>Update world model
    
    AI->>NE: AI agent's internal state
    Note right of NE: State representation<br>Action values<br>Prediction errors
    
    NE->>NE: Convert to stimulation parameters
    Note right of NE: Stimulation pattern<br>Intensity<br>Frequency<br>Duration
    
    NE->>S: Stimulation commands
    S->>R: Deliver targeted stimulation
    Note left of S: Optogenetic<br>Electrical<br>Chemogenetic
    
    Note over R,S: Closed-loop cycle repeats with <10ms latency
```



5. **Experimental Protocol: Tasks and Phases**: Maps out the experimental phases from calibration through simple conditioning, decision-making tasks, and social/contextual tasks, showing how experimental conditions are applied.

```mermaid
flowchart LR
    subgraph "Phase 1: Calibration (2 weeks)"
        P1A[Present Known Rewarding Stimuli]
        P1B[Present Known Aversive Stimuli]
        P1C[Vary Reward Magnitude]
        P1D[Explore Stimulation Parameters]
        P1E[Train Neural Decoder]
        
        P1A --> P1C
        P1B --> P1C
        P1C --> P1D
        P1D --> P1E
    end
    
    subgraph "Phase 2: Simple Conditioning Tasks"
        P2A[Classical Conditioning]
        P2B[Operant Conditioning]
        
        P2A1[Predictable CS-US Pairings]
        P2A2[Reversal Learning]
        
        P2B1[Fixed/Variable Ratio Schedules]
        P2B2[Progressive Ratio]
        
        P2A --> P2A1
        P2A --> P2A2
        P2B --> P2B1
        P2B --> P2B2
    end
    
    subgraph "Phase 3: Decision-Making Tasks"
        P3A[Two-Armed Bandit Task]
        P3B[Temporal Discounting Task]
        P3C[Effort-Based Task]
        
        P3A1[Probabilistic Rewards]
        P3A2[Changing Contingencies]
        
        P3B1[Immediate vs. Delayed Rewards]
        
        P3C1[Effort-Reward Trade-offs]
        
        P3A --> P3A1
        P3A --> P3A2
        P3B --> P3B1
        P3C --> P3C1
    end
    
    subgraph "Phase 4: Social and Contextual Tasks"
        P4A[Observational Learning]
        P4B[Social Reward Processing]
        P4C[Context-Dependent Valuation]
        
        P4A --> P4B
        P4B --> P4C
    end
    
    P1E --> |Decoder Validated| P2A
    P1E --> |Decoder Validated| P2B
    P2A --> |Basic Learning Established| P3A
    P2B --> |Basic Learning Established| P3A
    P3A --> |Decision-Making Validated| P4A
    P3B --> |Decision-Making Validated| P4A
    P3C --> |Decision-Making Validated| P4A
    
    subgraph "Experimental Conditions"
        EC1[Bio-Integrated Condition]
        EC2[Simulation-Integrated Condition]
        
        EC1 --- EC2
    end
    
    EC1 --- P2A
    EC1 --- P2B
    EC1 --- P3A
    EC1 --- P3B
    EC1 --- P3C
    EC1 --- P4A
    EC1 --- P4B
    EC1 --- P4C
    
    EC2 --- P2A
    EC2 --- P2B
    EC2 --- P3A
    EC2 --- P3B
    EC2 --- P3C
    EC2 --- P4A
    EC2 --- P4B
    EC2 --- P4C
```

6. **Data Collection and Analysis Pipeline**: Visualizes how data flows from collection through processing and analysis, including the different types of data and analytical approaches.

```mermaid
flowchart LR
    subgraph "Data Collection"
        DC1[Neural Data]
        DC2[Behavioral Data]
        DC3[AI Internal States]
        DC4[Simulation States]
        
        DC1_1[Spike Trains]
        DC1_2[Local Field Potentials]
        DC1_3[Calcium Signals]
        DC1_4[Neurotransmitter Levels]
        
        DC1 --- DC1_1
        DC1 --- DC1_2
        DC1 --- DC1_3
        DC1 --- DC1_4
        
        DC2_1[Movement Trajectories]
        DC2_2[Response Times]
        DC2_3[Choices]
        DC2_4[Vocalizations]
        
        DC2 --- DC2_1
        DC2 --- DC2_2
        DC2 --- DC2_3
        DC2 --- DC2_4
        
        DC3_1[Value Estimates]
        DC3_2[Policy Parameters]
        DC3_3[Prediction Errors]
        DC3_4[Uncertainty Estimates]
        
        DC3 --- DC3_1
        DC3 --- DC3_2
        DC3 --- DC3_3
        DC3 --- DC3_4
        
        DC4_1[Simulated Neural Activity]
        DC4_2[Simulated Neurotransmitter Levels]
        DC4_3[Synaptic Weights]
        
        DC4 --- DC4_1
        DC4 --- DC4_2
        DC4 --- DC4_3
    end
    
    subgraph "Data Processing"
        DP1[Preprocessing]
        DP2[Feature Extraction]
        DP3[Quality Control]
        
        DP1_1[Artifact Removal]
        DP1_2[Filtering]
        DP1_3[Spike Sorting]
        DP1_4[Motion Correction]
        
        DP1 --- DP1_1
        DP1 --- DP1_2
        DP1 --- DP1_3
        DP1 --- DP1_4
        
        DP2_1[Time-Frequency Analysis]
        DP2_2[Dimensionality Reduction]
        DP2_3[Event-Related Averaging]
        DP2_4[Information-Theoretic Measures]
        
        DP2 --- DP2_1
        DP2 --- DP2_2
        DP2 --- DP2_3
        DP2 --- DP2_4
        
        DP3_1[Outlier Detection]
        DP3_2[Signal Quality Assessment]
        DP3_3[Metadata Logging]
        
        DP3 --- DP3_1
        DP3 --- DP3_2
        DP3 --- DP3_3
    end
    
    subgraph "Analysis"
        A1[Behavioral Comparison]
        A2[Neural Activity Comparison]
        A3[Subjective Experience Indicators]
        A4[Cross-System Analysis]
        
        A1_1[Performance Matching]
        A1_2[Strategy Analysis]
        A1_3[Adaptation Assessment]
        
        A1 --- A1_1
        A1 --- A1_2
        A1 --- A1_3
        
        A2_1[Pattern Similarity]
        A2_2[Temporal Dynamics]
        A2_3[Information Processing]
        
        A2 --- A2_1
        A2 --- A2_2
        A2 --- A2_3
        
        A3_1[Reward Sensitivity]
        A3_2[Hedonic Response]
        A3_3[Learning Signatures]
        
        A3 --- A3_1
        A3 --- A3_2
        A3 --- A3_3
        
        A4_1[Canonical Correlation Analysis]
        A4_2[Representational Similarity Comparison]
        A4_3[Divergence Metrics]
        
        A4 --- A4_1
        A4 --- A4_2
        A4 --- A4_3
    end
    
    DC1 --> DP1
    DC2 --> DP1
    DC3 --> DP1
    DC4 --> DP1
    
    DP1 --> DP2
    DP2 --> DP3
    DP3 --> A1
    DP3 --> A2
    DP3 --> A3
    DP3 --> A4
    
    A1 --> Results
    A2 --> Results
    A3 --> Results
    A4 --> Results
    
    Results[Results Interpretation and Publication]
```

7. **Hypothesis Testing Framework**: Outlines the four main hypotheses being tested, the metrics used to evaluate them, and the analytical methods applied.

```mermaid
graph LR
    subgraph "H1: Bio-AI Correlation"
        H1[AI agent coupled to rat pleasure circuits will develop reward learning patterns correlating with neural signatures of subjective experience]
        
        H1M1[Gamma power and coherence: r > 0.7, p < 0.01]
        H1M2[Approximated Φ: Significant increase during reward]
        H1M3[Dopamine/serotonin ratio: R > 1.5 for positive valence]
        H1M4[Approach/avoidance ratio: > 2:1]
        
        H1 --- H1M1
        H1 --- H1M2
        H1 --- H1M3
        H1 --- H1M4
        
        H1A1[Pearson correlation between neural signatures and AI signals]
        H1A2[Multiple regression predicting behavioral responses]
        H1A3[Time-lagged cross-correlation for temporal dynamics]
        
        H1 --- H1A1
        H1 --- H1A2
        H1 --- H1A3
    end
    
    subgraph "H2: Functional Equivalence"
        H2[AI with simulated pleasure circuit will match biological behavior but differ in neural signatures]
        
        H2M1["Behavioral equivalence: |d| < 0.2 (small effect size)"]
        H2M2["Neural difference: |d| > 0.8 (large effect size)"]
        H2M3[Modulation index: Higher in biological system, p < 0.01]
        
        H2 --- H2M1
        H2 --- H2M2
        H2 --- H2M3
        
        H2A1[Paired t-tests comparing behavioral metrics]
        H2A2[MANOVA on neural signature metrics]
        H2A3[Representational Similarity Analysis]
        
        H2 --- H2A1
        H2 --- H2A2
        H2 --- H2A3
    end
    
    subgraph "H3: Complexity-Divergence"
        H3[Divergence between systems will increase with task complexity]
        
        H3M1[Regression analysis: R² > 0.6]
        H3M2["Divergence metric: D(BI, SI)task"]
        
        H3 --- H3M1
        H3 --- H3M2
        
        H3A1[Regression analysis of divergence vs complexity]
        H3A2[Repeated measures ANOVA]
        H3A3[Curve fitting to characterize relationship]
        
        H3 --- H3A1
        H3 --- H3A2
        H3 --- H3A3
    end
    
    subgraph "H4: Information Integration"
        H4[Φ will correlate with subjective experience indicators with substrate-specific differences]
        
        H4M1[Correlation strength: r > 0.7]
        H4M2["Difference in correlations: |r₁-r₂| > 0.2"]
        
        H4 --- H4M1
        H4 --- H4M2
        
        H4A1[Correlation analysis between Φ and behavioral indicators]
        H4A2[Comparison of correlation patterns between systems]
        H4A3[Path analysis modeling direct/indirect relationships]
        
        H4 --- H4A1
        H4 --- H4A2
        H4 --- H4A3
    end
    
    H1 --> Overall[Overall Conclusion about Consciousness Correlates]
    H2 --> Overall
    H3 --> Overall
    H4 --> Overall
```

8. **Project Timeline and Milestones**: Provides a Gantt chart showing the 36-month project timeline across three major phases, with key milestones and publication targets.

```mermaid
gantt
    title BARLI Project Timeline (36 Months)
    dateFormat  YYYY-MM-DD
    section Phase 1: Setup and Calibration
    Infrastructure Development           :a1, 2026-01-01, 3M
    System Development                   :a2, after a1, 3M
    Protocol Validation                  :a3, after a2, 3M
    Calibration Phase                    :a4, after a3, 3M
    Full System Readiness                :milestone, after a4, 0d
    
    section Phase 2: Initial Experiments
    Simple Conditioning Experiments      :b1, after a4, 3M
    Reinforcement Learning Tasks         :b2, after b1, 3M
    Intermediate Data Analysis           :b3, after b2, 3M
    Complex Decision-Making Tasks        :b4, after b3, 3M
    Initial Dataset Complete             :milestone, after b4, 0d
    
    section Phase 3: Advanced Experiments
    Social and Contextual Tasks          :c1, after b4, 3M
    Comprehensive Data Analysis          :c2, after c1, 3M
    Integration and Synthesis            :c3, after c2, 3M
    Dissemination and Future Planning    :c4, after c3, 3M
    Project Completion                   :milestone, after c4, 0d
    
    section Publications and Deliverables
    Methods Paper                        :p1, 2026-10-01, 2M
    Initial Findings Paper               :p2, 2027-07-01, 3M
    Comprehensive Results Paper          :p3, 2028-07-01, 3M
    Open Dataset Release                 :p4, 2029-12-01, 1M
```

9. **Operationalizing Subjective Experience**: Details the metrics and measurements used to quantify aspects of subjective experience, from neural oscillations to behavioral indicators.

```mermaid
graph LR
    subgraph "Neural Oscillatory Signatures"
        NOS1["Gamma Band Activity (30-100 Hz)"]
        NOS2[Cross-Frequency Coupling]
        NOS3[Neural Complexity Measures]
        
        NOS1_1["Gamma power: ∫₃₀¹⁰⁰ P(f) df"]
        NOS1_2[Gamma coherence between recording sites]
        NOS1_3[Gamma bursting rate and duration]
        
        NOS1 --- NOS1_1
        NOS1 --- NOS1_2
        NOS1 --- NOS1_3
        
        NOS2_1[Modulation Index: MI]
        NOS2_2[Preferred phase of theta]
        NOS2_3[Coupling directionality]
        
        NOS2 --- NOS2_1
        NOS2 --- NOS2_2
        NOS2 --- NOS2_3
        
        NOS3_1["Lempel-Ziv complexity (LZC)"]
        NOS3_2[Sample entropy]
        NOS3_3[Coalition entropy]
        
        NOS3 --- NOS3_1
        NOS3 --- NOS3_2
        NOS3 --- NOS3_3
    end
    
    subgraph "Neurotransmitter Dynamics"
        ND1[Reward Chemical Balance]
        ND2[Temporal Release Patterns]
        ND3[Hedonic Impact Indicators]
        
        ND1_1["DA/5-HT ratio: R(D/S)"]
        ND1_2["Absolute concentrations: [DA], [5-HT]"]
        ND1_3[Release probability]
        
        ND1 --- ND1_1
        ND1 --- ND1_2
        ND1 --- ND1_3
        
        ND2_1["Phasic/tonic ratio: R(P/T)"]
        ND2_2[Response latency]
        ND2_3[Decay kinetics]
        
        ND2 --- ND2_1
        ND2 --- ND2_2
        ND2 --- ND2_3
        
        ND3_1["Endorphin concentration: [END]"]
        ND3_2["Endocannabinoid levels: [2-AG], [AEA]"]
        ND3_3[Opioid receptor activation]
        
        ND3 --- ND3_1
        ND3 --- ND3_2
        ND3 --- ND3_3
    end
    
    subgraph "Behavioral Indicators"
        BI1["Ultrasonic Vocalizations (USVs)"]
        BI2[Facial and Bodily Expressions]
        BI3[Motivational Indicators]
        
        BI1_1["USV ratio: USV(ratio) = N(50kHz)/N(22kHz)"]
        BI1_2[Call rate: calls per minute]
        BI1_3[Acoustic features]
        
        BI1 --- BI1_1
        BI1 --- BI1_2
        BI1 --- BI1_3
        
        BI2_1[Grimace Scale]
        BI2_2[Facial relaxation]
        BI2_3[Body posture]
        
        BI2 --- BI2_1
        BI2 --- BI2_2
        BI2 --- BI2_3
        
        BI3_1[Breakpoint in progressive ratio]
        BI3_2[Preference strength]
        BI3_3[Consumption pattern]
        
        BI3 --- BI3_1
        BI3 --- BI3_2
        BI3 --- BI3_3
    end
    
    subgraph "Integrated Information Metrics"
        IIM1["Phi (Φ) Approximation"]
        IIM2[Information Dynamics]
        IIM3[Metastability Measures]
        
        IIM1_1["Approximate Φ"]
        IIM1_2[Effective Information]
        IIM1_3[Causal Density]
        
        IIM1 --- IIM1_1
        IIM1 --- IIM1_2
        IIM1 --- IIM1_3
        
        IIM2_1[Transfer Entropy]
        IIM2_2[Active Information Storage]
        IIM2_3[Predictive Information]
        
        IIM2 --- IIM2_1
        IIM2 --- IIM2_2
        IIM2 --- IIM2_3
        
        IIM3_1[Synchrony variability]
        IIM3_2[Coalition entropy]
        IIM3_3[Criticality indicators]
        
        IIM3 --- IIM3_1
        IIM3 --- IIM3_2
        IIM3 --- IIM3_3
    end
    
    subgraph "AI System Subjective Correlates"
        AISC1[Representational Geometry]
        AISC2[Reward Prediction Dynamics]
        AISC3[Simulated Neurotransmitter Dynamics]
        
        AISC1_1["Representational Dissimilarity Matrix (RDM)"]
        AISC1_2[Dimensionality]
        AISC1_3[Clustering coefficient]
        
        AISC1 --- AISC1_1
        AISC1 --- AISC1_2
        AISC1 --- AISC1_3
        
        AISC2_1["Reward Prediction Error (RPE)"]
        AISC2_2[Uncertainty estimation]
        AISC2_3[Surprise signals]
        
        AISC2 --- AISC2_1
        AISC2 --- AISC2_2
        AISC2 --- AISC2_3
        
        AISC3_1[Simulated DA/5-HT ratio]
        AISC3_2[Phasic/tonic patterns]
        AISC3_3[Neuromodulatory effects]
        
        AISC3 --- AISC3_1
        AISC3 --- AISC3_2
        AISC3 --- AISC3_3
    end
    
    NOS1 --> ComparisonFramework
    NOS2 --> ComparisonFramework
    NOS3 --> ComparisonFramework
    ND1 --> ComparisonFramework
    ND2 --> ComparisonFramework
    ND3 --> ComparisonFramework
    BI1 --> ComparisonFramework
    BI2 --> ComparisonFramework
    BI3 --> ComparisonFramework
    IIM1 --> ComparisonFramework
    IIM2 --> ComparisonFramework
    IIM3 --> ComparisonFramework
    AISC1 --> ComparisonFramework
    AISC2 --> ComparisonFramework
    AISC3 --> ComparisonFramework
    
    ComparisonFramework[Cross-System Comparison Framework]
```

10. **Ethical Considerations and Regulatory Compliance**: Illustrates the comprehensive ethical framework, including animal welfare principles, regulatory compliance, AI ethics, and data management practices.

```mermaid
flowchart LR
    subgraph "Animal Welfare & 3Rs Principle"
        AW1[Replacement Strategies]
        AW2[Reduction Strategies]
        AW3[Refinement Approaches]
        
        AW1_1[Use of Existing Data]
        AW1_2[Alternative Models]
        AW1_3[Justification for Animal Use]
        
        AW1 --- AW1_1
        AW1 --- AW1_2
        AW1 --- AW1_3
        
        AW2_1[Statistical Optimization]
        AW2_2[Maximizing Data Collection]
        AW2_3[Tissue Sharing]
        
        AW2 --- AW2_1
        AW2 --- AW2_2
        AW2 --- AW2_3
        
        AW3_1[Surgical Procedures]
        AW3_2[Pain Management]
        AW3_3[Housing and Enrichment]
        AW3_4[Humane Endpoints]
        
        AW3 --- AW3_1
        AW3 --- AW3_2
        AW3 --- AW3_3
        AW3 --- AW3_4
    end
    
    subgraph "Regulatory Compliance"
        RC1["Institutional Animal Care and Use Committee (IACUC)"]
        RC2[Animal Welfare Regulations]
        RC3[Researcher Training and Qualification]
        
        RC1_1[Protocol Submission]
        RC1_2[Ongoing Oversight]
        RC1_3[Documentation Requirements]
        
        RC1 --- RC1_1
        RC1 --- RC1_2
        RC1 --- RC1_3
        
        RC2_1[Federal Compliance]
        RC2_2[State and Local Requirements]
        RC2_3[International Standards]
        
        RC2 --- RC2_1
        RC2 --- RC2_2
        RC2 --- RC2_3
        
        RC3_1[Required Training]
        RC3_2[Surgical Qualifications]
        RC3_3[Continuing Education]
        
        RC3 --- RC3_1
        RC3 --- RC3_2
        RC3 --- RC3_3
    end
    
    subgraph "Responsible AI Development"
        AI1[AI Safety Protocols]
        AI2[Avoiding AI Misuse]
        AI3[Artificial Sentience Considerations]
        
        AI1_1[System Containment]
        AI1_2[Monitoring Frameworks]
        AI1_3[Interpretability Measures]
        
        AI1 --- AI1_1
        AI1 --- AI1_2
        AI1 --- AI1_3
        
        AI2_1[Dual-Use Considerations]
        AI2_2[Data Security]
        AI2_3[Responsible Disclosure]
        
        AI2 --- AI2_1
        AI2 --- AI2_2
        AI2 --- AI2_3
        
        AI3_1[Welfare Monitoring]
        AI3_2[Systems Design]
        AI3_3[Contingency Planning]
        
        AI3 --- AI3_1
        AI3 --- AI3_2
        AI3 --- AI3_3
    end
    
    subgraph "Data Management and Privacy"
        DM1[Data Security]
        DM2[Confidentiality and Anonymization]
        DM3[Open Science and Data Sharing]
        
        DM1_1[Storage Infrastructure]
        DM1_2[Access Protocols]
        DM1_3[Data Transmission]
        
        DM1 --- DM1_1
        DM1 --- DM1_2
        DM1 --- DM1_3
        
        DM2_1[Identification Removal]
        DM2_2[Aggregation Techniques]
        DM2_3[Data Minimization]
        
        DM2 --- DM2_1
        DM2 --- DM2_2
        DM2 --- DM2_3
        
        DM3_1[Data Sharing Plan]
        DM3_2[Reproducibility Package]
        DM3_3[Licensing and Attribution]
        
        DM3 --- DM3_1
        DM3 --- DM3_2
        DM3 --- DM3_3
    end
    
    subgraph "Societal Implications"
        SI1[Philosophical and Societal Impact]
        SI2[Stakeholder Consultation]
        SI3[Responsible Communication]
        
        SI1_1[Knowledge Dissemination]
        SI1_2[Ethical Implications]
        SI1_3[Policy Engagement]
        
        SI1 --- SI1_1
        SI1 --- SI1_2
        SI1 --- SI1_3
        
        SI2_1[Scientific Community]
        SI2_2[Ethics Boards]
        SI2_3[Public Engagement]
        
        SI2 --- SI2_1
        SI2 --- SI2_2
        SI2 --- SI2_3
        
        SI3_1[Media Engagement]
        SI3_2[Managing Expectations]
        SI3_3[Scientific Integrity]
        
        SI3 --- SI3_1
        SI3 --- SI3_2
        SI3 --- SI3_3
    end
    
    AW1 --> EthicsCommittee
    AW2 --> EthicsCommittee
    AW3 --> EthicsCommittee
    RC1 --> EthicsCommittee
    RC2 --> EthicsCommittee
    RC3 --> EthicsCommittee
    AI1 --> EthicsCommittee
    AI2 --> EthicsCommittee
    AI3 --> EthicsCommittee
    DM1 --> EthicsCommittee
    DM2 --> EthicsCommittee
    DM3 --> EthicsCommittee
    SI1 --> EthicsCommittee
    SI2 --> EthicsCommittee
    SI3 --> EthicsCommittee
    
    EthicsCommittee[Ethics Committee Oversight and Review]
```

11. **Cross-System Comparison Methodology**: Shows how the biological and simulated systems are compared across different dimensions, including the calculation of similarity metrics and analysis of task complexity effects.

```mermaid
graph LR
    subgraph "Biological System (BI)"
        BI_NE[Neural Activity]
        BI_NT[Neurotransmitter Dynamics]
        BI_BH[Behavioral Responses]
        
        BI_NE --- BI_NT
        BI_NT --- BI_BH
        BI_NE --- BI_BH
    end
    
    subgraph "Simulated System (SI)"
        SI_NE[Simulated Neural Activity]
        SI_NT[Simulated Neurotransmitter Dynamics]
        SI_BH[Simulated Behavioral Responses]
        
        SI_NE --- SI_NT
        SI_NT --- SI_BH
        SI_NE --- SI_BH
    end
    
    subgraph "Comparison Methods"
        CM1[Behavioral Comparison]
        CM2[Neural Activity Comparison]
        CM3[Information Integration Comparison]
        
        CM1_1[Performance Matching]
        CM1_2[Strategy Analysis]
        CM1_3[Mixed-effects Models]
        
        CM1 --- CM1_1
        CM1 --- CM1_2
        CM1 --- CM1_3
        
        CM2_1[Representational Similarity Analysis]
        CM2_2[Dynamic Time Warping]
        CM2_3[Information-Theoretic Measures]
        
        CM2 --- CM2_1
        CM2 --- CM2_2
        CM2 --- CM2_3
        
        CM3_1["Phi (Φ) Comparison"]
        CM3_2[Causal Analysis]
        CM3_3[Complexity Measures]
        
        CM3 --- CM3_1
        CM3 --- CM3_2
        CM3 --- CM3_3
    end
    
    subgraph "Similarity Metrics"
        SM1[Behavioral Similarity]
        SM2[Neural Pattern Similarity]
        SM3[Temporal Dynamics Similarity]
        SM4[Information Processing Similarity]
        SM5[Weighted Composite Similarity Index]
        
        SM1 --- SM5
        SM2 --- SM5
        SM3 --- SM5
        SM4 --- SM5
        
        SM_F["S(BI, SI) = ∑ wi Si(BI, SI)"]
        
        SM5 --- SM_F
    end
    
    BI_BH -->|Compare| CM1
    SI_BH -->|Compare| CM1
    
    BI_NE -->|Compare| CM2
    SI_NE -->|Compare| CM2
    
    BI_NE -->|Compute Φ| CM3
    SI_NE -->|Compute Φ| CM3
    
    CM1 --> SM1
    CM2 --> SM2
    CM2 --> SM3
    CM3 --> SM4
    
    subgraph "Task Complexity Analysis"
        TC1[Simple Conditioning]
        TC2[Probabilistic Learning]
        TC3[Temporal Discounting]
        TC4[Context-Dependent Decisions]
        TC5[Social Learning]
        
        TC1 -->|Increasing Complexity| TC2
        TC2 -->|Increasing Complexity| TC3
        TC3 -->|Increasing Complexity| TC4
        TC4 -->|Increasing Complexity| TC5
        
        TC_D["Divergence Metric: D(BI, SI)task"]
        
        TC1 --- TC_D
        TC2 --- TC_D
        TC3 --- TC_D
        TC4 --- TC_D
        TC5 --- TC_D
    end
    
    SM_F --> Findings[Research Findings]
    TC_D --> Findings
```

12. **Risk Management and Contingency Planning**: Outlines potential technical, biological, schedule, and budget risks, along with mitigation strategies, contingency plans, and monitoring processes.

```mermaid
graph LR
    subgraph "Technical Risks"
        TR1[Neural Recording Challenges]
        TR2[Computational Infrastructure Issues]
        TR3[Software Integration Problems]
        
        TR1_M[Mitigation: Redundant recording sites, regular testing]
        TR1_C[Contingency: Alternative recording technologies]
        
        TR1 --- TR1_M
        TR1 --- TR1_C
        
        TR2_M[Mitigation: Scalable design, cloud computing options]
        TR2_C[Contingency: Simplified models, prioritized analyses]
        
        TR2 --- TR2_M
        TR2 --- TR2_C
        
        TR3_M[Mitigation: Early integration testing, middleware]
        TR3_C[Contingency: Custom interface development]
        
        TR3 --- TR3_M
        TR3 --- TR3_C
    end
    
    subgraph "Biological Risks"
        BR1[Surgical Complications]
        BR2[Animal Health Issues]
        BR3[Signal Stability Problems]
        
        BR1_M[Mitigation: Refined techniques, experienced personnel]
        BR1_C[Contingency: Modified implantation strategies]
        
        BR1 --- BR1_M
        BR1 --- BR1_C
        
        BR2_M[Mitigation: Health monitoring, optimized housing]
        BR2_C[Contingency: Flexible schedule, adjusted cohort size]
        
        BR2 --- BR2_M
        BR2 --- BR2_C
        
        BR3_M[Mitigation: Regular calibration, robust signal processing]
        BR3_C[Contingency: Alternative metrics, control recordings]
        
        BR3 --- BR3_M
        BR3 --- BR3_C
    end
    
    subgraph "Schedule Risks"
        SR1[Regulatory Delays]
        SR2[Equipment Procurement Delays]
        SR3[Personnel Recruitment Challenges]
        
        SR1_M[Mitigation: Early submission, thorough preparation]
        SR1_C[Contingency: Parallel work on non-animal components]
        
        SR1 --- SR1_M
        SR1 --- SR1_C
        
        SR2_M[Mitigation: Early ordering, alternative suppliers]
        SR2_C[Contingency: Equipment sharing, phased implementation]
        
        SR2 --- SR2_M
        SR2 --- SR2_C
        
        SR3_M[Mitigation: Early recruitment, competitive compensation]
        SR3_C[Contingency: Training existing staff, consulting]
        
        SR3 --- SR3_M
        SR3 --- SR3_C
    end
    
    subgraph "Budget Risks"
        BuR1[Cost Escalation]
        BuR2[Funding Disruptions]
        BuR3[Unexpected Expenses]
        
        BuR1_M[Mitigation: Conservative budgeting, price guarantees]
        BuR1_C[Contingency: Reallocation from contingency fund]
        
        BuR1 --- BuR1_M
        BuR1 --- BuR1_C
        
        BuR2_M[Mitigation: Diversified funding, milestone-based releases]
        BuR2_C[Contingency: Modular project design]
        
        BuR2 --- BuR2_M
        BuR2 --- BuR2_C
        
        BuR3_M[Mitigation: Comprehensive planning, expert consultation]
        BuR3_C[Contingency: Contingency fund, scope prioritization]
        
        BuR3 --- BuR3_M
        BuR3 --- BuR3_C
    end
    
    subgraph "Risk Monitoring Process"
        RM1[Daily Technical Monitoring]
        RM2[Weekly Risk Assessment]
        RM3[Monthly Comprehensive Review]
        RM4[Quarterly Strategic Risk Evaluation]
        
        RM1 --> RM2
        RM2 --> RM3
        RM3 --> RM4
        RM4 --> RM1
    end
    
    subgraph "Contingency Scenarios"
        CS1[Major Equipment Failure]
        CS2[Unsuccessful Neural-Digital Interface]
        CS3[Animal Health Crisis]
        CS4[Critical Data Loss]
        CS5[Regulatory Compliance Issue]
        
        CS1_R[Response: Deploy backup system, revise experimental plan]
        CS2_R[Response: Test alternative configurations, simplified targets]
        CS3_R[Response: Veterinary intervention, enhanced monitoring]
        CS4_R[Response: Data recovery, enhanced backup systems]
        CS5_R[Response: Temporary procedure suspension, protocol modification]
        
        CS1 --- CS1_R
        CS2 --- CS2_R
        CS3 --- CS3_R
        CS4 --- CS4_R
        CS5 --- CS5_R
    end
    
    TR1 --> RM1
    TR2 --> RM1
    TR3 --> RM1
    BR1 --> RM1
    BR2 --> RM1
    BR3 --> RM1
    SR1 --> RM2
    SR2 --> RM2
    SR3 --> RM2
    BuR1 --> RM3
    BuR2 --> RM3
    BuR3 --> RM3
```



















