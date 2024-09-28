2024-09-05 18:20

Status : #baby

Tags : [[Core Concepts]]

---
graph TD
    A[DOM Manipulation] --> B[Selecting Elements]
    A --> C[Modifying Elements]
    A --> D[Creating Elements]
    A --> E[Removing Elements]
    A --> F[Event Handling]
    A --> G[Traversing the DOM]
    A --> H[Performance Optimization]
    A --> I[Animation]
    A --> J[Forms Manipulation]

    B --> B1[getElementById]
    B --> B2[getElementsByClassName]
    B --> B3[getElementsByTagName]
    B --> B4[querySelector]
    B --> B5[querySelectorAll]
    B --> B6[matches]
    B --> B7[closest]

    C --> C1[Changing Content]
    C --> C2[Modifying Attributes]
    C --> C3[Changing Styles]
    C --> C4[Modifying Classes]

    C1 --> C1a[innerHTML]
    C1 --> C1b[textContent]
    C1 --> C1c[innerText]

    C2 --> C2a[setAttribute]
    C2 --> C2b[removeAttribute]
    C2 --> C2c[dataset]

    C3 --> C3a[style property]
    C3 --> C3b[cssText]
    C3 --> C3c[getComputedStyle]

    C4 --> C4a[classList]
    C4 --> C4b[className]

    D --> D1[createElement]
    D --> D2[createTextNode]
    D --> D3[appendChild]
    D --> D4[insertBefore]
    D --> D5[insertAdjacentHTML]
    D --> D6[cloneNode]

    E --> E1[removeChild]
    E --> E2[remove]
    E --> E3[replaceChild]

    F --> F1[addEventListener]
    F --> F2[removeEventListener]
    F --> F3[Event Object]
    F --> F4[Event Propagation]
    F --> F5[Event Delegation]
    F --> F6[Custom Events]

    G --> G1[parentNode]
    G --> G2[childNodes]
    G --> G3[nextSibling]
    G --> G4[previousSibling]
    G --> G5[firstChild]
    G --> G6[lastChild]

    H --> H1[DocumentFragment]
    H --> H2[requestAnimationFrame]
    H --> H3[Debounce and Throttle]
    H --> H4[Virtual DOM]

    I --> I1[CSS Transitions]
    I --> I2[CSS Animations]
    I --> I3[Web Animations API]

    J --> J1[form property]
    J --> J2[formData]
    J --> J3[validity]
    J --> J4[Constraint Validation API]

    %% Additional relationships
    B -.-> H1
    F5 -.-> B
    H2 -.-> I
    C3 -.-> I
    J -.-> F
    H3 -.-> F
    H4 -.-> C
    D -.-> H1
    G -.-> B6
    G -.-> B7

---
## **References** 

