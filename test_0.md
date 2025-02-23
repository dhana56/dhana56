### 🧬 Research Focus Areas
```mermaid
%%{init: {'theme': 'dark', 'themeVariables': { 'fontSize': '16px' }}}%%
graph TB
    %% Core Research Areas
    subgraph CORE["COMPUTATIONAL BIOLOGY"]
        direction TB
        subgraph ALG["Algorithmic Biology"]
            A1[("ML/DL<br/>Models")]:::small
            A2[("Pattern<br/>Analysis")]:::small
            A3[("Theory")]:::small
        end
        
        subgraph SYS["Systems Biology"]
            S1[("Network<br/>Analysis")]:::small
            S2[("Dynamics")]:::small
            S3[("Regulation")]:::small
        end
        
        subgraph DIS["Disease Biology"]
            D1[("Cancer")]:::small
            D2[("Viral")]:::small
            D3[("Precision<br/>Med")]:::small
        end
    end

    space[" "]:::space
    
    subgraph APPS["TRANSLATIONAL RESEARCH"]
        T1{{"Genotype-Phenotype"}}:::apps
        T2{{"Microbiome"}}:::apps
        T3{{"Therapeutics"}}:::apps
    end

    %% Connections with better spacing
    CORE --> space
    space --> APPS
    ALG --> T1
    SYS --> T2
    DIS --> T3

    %% Optimized color scheme
    classDef default fill:#1a1b27,stroke:#7aa2f7,stroke-width:1px,color:#fff
    classDef core fill:#1a1b27,stroke:#7aa2f7,stroke-width:2px,color:#fff
    classDef small fill:#24283b,stroke:#7aa2f7,stroke-width:1px,color:#fff
    classDef apps fill:#1a1b27,stroke:#ff3068,stroke-width:2px,color:#fff
    classDef space fill:none,stroke:none

    class CORE,ALG,SYS,DIS core
    class A1,A2,A3,S1,S2,S3,D1,D2,D3 small
    class T1,T2,T3 apps
    class space space

    linkStyle default stroke:#7aa2f7,stroke-width:1px
```