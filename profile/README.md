# Antares

## Overview

Antares is composed of multiple programs that form a comprehensive ecosystem for 
simulating transmission systems at short- or long-term horizons. Its aim is to:
- Precisely quantify the adequacy and economic performance of national 
  or continental interconnected energy systems
- Perform investment optimization to anticipate the future development of the grid


## Main applications

```mermaid
graph TD;
data-manager -.-> antares_craft
data-manager -.-> AntaREST
antares_craft --> AntaREST
AntaREST --> core

subgraph core[Core computations]
    Antares_Simulator
    antares-xpansion
end

data-manager[<a href="https://github.com/AntaresSimulatorTeam/antares-datamanager-front" style="text-decoration:none;">data-manager</a> <br><span>Antares study generator</span>];
antares_craft[<a href="https://github.com/AntaresSimulatorTeam/antares_craft" style="text-decoration:none;">antares_craft</a> <br><span>Python library for interacting with Antares studies</span>];
AntaREST[<a href="https://github.com/AntaresSimulatorTeam/AntaREST" style="text-decoration:none;">AntaREST</a> <br><span>Web interface and REST API</span>];
antares-xpansion[<a href="https://github.com/AntaresSimulatorTeam/antares-xpansion" style="text-decoration:none;">antares-xpansion</a> <br><span>Investment module</span>];
Antares_Simulator[<a href="https://github.com/AntaresSimulatorTeam/Antares_Simulator" style="text-decoration:none;">Antares_Simulator</a> <br><span>Simulation engine</span>];

style data-manager stroke-dasharray: 2
```

You can find a more functional diagram 
[here](https://antares-doc.readthedocs.io/en/latest/overview/architecture/).

## Links

:book: [Antares documentation](https://antares-doc.readthedocs.io/en/latest/)

:new: [Release notes](https://antares-doc.readthedocs.io/en/latest/overview/changelogs/)

