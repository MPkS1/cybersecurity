flowchart TB
    classDef beginner fill:#D1F0FF,stroke:#0098DA,color:black
    classDef intermediate fill:#D7F4D7,stroke:#2D882D,color:black
    classDef advanced fill:#FFE6CC,stroke:#D79B00,color:black
    classDef expert fill:#F8CECC,stroke:#B85450,color:black
    
    Start([START HERE]) --> Intro
    
    subgraph "BEGINNER LEVEL"
        Intro["Introduction to Cybersecurity"]
        Net["Networking Fundamentals"]
        OS["Operating Systems Security"]
        
        Intro --> Net
        Net --> OS
    end
    
    subgraph "INTERMEDIATE LEVEL"
        Crypto["Cryptography"]
        WebSec["Web Application Security"]
        
        OS --> Crypto
        Crypto --> WebSec
    end
    
    subgraph "ADVANCED LEVEL"
        PenTest["Penetration Testing & Ethical Hacking"]
        Forensics["Digital Forensics"]
        
        WebSec --> PenTest
        PenTest --> Forensics
    end
    
    subgraph "EXPERT LEVEL"
        Compliance["Compliance and Best Practices"]
        Projects["Projects & Practical Experience"]
        
        Forensics --> Compliance
        Compliance --> Projects
    end
    
    %% Topic Details
    Intro --> Intro1["Common Threats"]
    Intro --> Intro2["Attack Vectors"]
    Intro --> Intro3["Security Mindset"]
    
    Net --> Net1["IP Addressing"]
    Net --> Net2["Firewalls & VPNs"]
    Net --> Net3["Secure Protocols"]
    
    OS --> OS1["Windows Security"]
    OS --> OS2["Linux Security"]
    OS --> OS3["Mac Security"]
    
    Crypto --> Crypto1["Encryption"]
    Crypto --> Crypto2["Hashing"]
    Crypto --> Crypto3["PKI"]
    
    WebSec --> WebSec1["SQL Injection"]
    WebSec --> WebSec2["XSS"]
    WebSec --> WebSec3["CSRF"]
    
    PenTest --> PenTest1["Metasploit"]
    PenTest --> PenTest2["Nmap"]
    PenTest --> PenTest3["Wireshark"]
    
    Forensics --> Forensics1["Evidence Collection"]
    Forensics --> Forensics2["Analysis Techniques"]
    Forensics --> Forensics3["Reporting"]
    
    Compliance --> Compliance1["ISO 27001"]
    Compliance --> Compliance2["NIST"]
    Compliance --> Compliance3["GDPR"]
    
    Projects --> Projects1["CTF Challenges"]
    Projects --> Projects2["Bug Bounties"]
    Projects --> Projects3["Real-world Projects"]
    
    class Intro,Net,OS beginner
    class Crypto,WebSec intermediate
    class PenTest,Forensics advanced
    class Compliance,Projects expert
    
    Projects --> Mastery([CYBERSECURITY MASTERY])
