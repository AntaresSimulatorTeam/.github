# Antares

## Overview

Antares is composed of multiple programs that form a comprehensive ecosystem for 
simulating transmission systems at short- or long-term horizons. Its aim is to:
- Precisely quantify the adequacy and economic performance of national 
  or continental interconnected energy systems
- Perform investment optimization to anticipate the future development of the grid


## Main applications

```mermaid
flowchart TD
    A[data-manager\nStudy generator]
    B[antares_craft\nPython library for interacting with Antares studies]
    C[AntaREST\nWeb interface and REST API]
    
    subgraph Core computations
        direction LR
        D[Antares_Simulator<br/>Core computations]
        E[antares-xpansion<br/>Investment module]
    end
    A -.-> B
    B --> C
    A -.-> C
    C --> D
    C --> E

    %% Links (replace with actual URLs)
    click A "https://github.com/AntaresSimulatorTeam/datamanager-front" _blank
    click B "https://github.com/AntaresSimulatorTeam/antares_craft" _blank
    click C "https://github.com/AntaresSimulatorTeam/AntaREST" _blank
    click D "https://github.com/AntaresSimulatorTeam/Antares_Simulator" _blank
    click E "https://github.com/AntaresSimulatorTeam/antares-xpansion" _blank

    style A stroke-dasharray: 2
```

You can find a more functional diagram 
[here](https://antares-doc.readthedocs.io/en/latest/overview/architecture/).

## Links

:book: [Antares documentation](https://antares-doc.readthedocs.io/en/latest/)

:new: [Release notes](https://antares-doc.readthedocs.io/en/latest/overview/changelogs/)

