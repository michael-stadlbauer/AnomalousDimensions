# Anomalous Dimensions Repository

This repository contains supplementary files of the publication https://inspirehep.net/literature/2832469 with the infrared anomalous dimensions in the Standard Model up to three loops in Mathematica.

## Supplementary Files

### IRAnomDim_SM_3Loop.m
This file contains the infrared (IR) anomalous dimensions up to three loops. Upon loading the file into Mathematica with the `Get` command, the following variables are created in the workspace:

- **`γCusp`**: Cusp anomalous dimensions.
- **`γColl`**: Collinear anomalous dimensions.

#### Function Details
Both functions accept 1 or 2 arguments:

1. **First Argument**: Specifies the gauge group (for `γCusp`) or the external particle (for `γColl`).
2. **Second Argument** (optional): Specifies the loop order to return. If omitted, the full anomalous dimension up to three loops is returned.

##### Examples:
- `γColl["B"]` returns the full collinear anomalous dimension of the B gauge boson up to three loops.
- `γColl["B", 2]` returns the collinear anomalous dimension of the B gauge boson at two loops only.

##### Allowed Arguments
The table below lists the allowed arguments for `γCusp` and `γColl`. Note that arguments must be passed as strings.

| `γColl`    | `γCusp`         |
|------------|-----------------|
| B          | U1              |
| W          | SU2             |
| G          | SU3             |
| eR         | SU3xSU2         |
| LL         | SU3xU1          |
| dR         | SU3xYd          |
| uR         | SU3xYu          |
| QL         | SU2xSU3         |
| H          | SU2xU1          |
|            | SU2xYd          |
|            | SU2xYu          |
|            | SU2xYl          |
|            | U1xSU2          |
|            | U1xSU3          |
|            | U1xYd           |
|            | U1xYu           |
|            | U1xYl           |

Note: Cusp anomalous dimensions are called with Standard Model values of gauge groups (e.g., SU(3), SU(2)), while the results are still given for general SU(N_1) and SU(N_2).

---

### BetaFunc_SM_2Loop.m
This file provides the beta functions for Standard Model couplings up to two loops. Upon loading the file into Mathematica, the function `beta` is created in the workspace.

#### Function Details
The `beta` function accepts a single argument specifying the coupling constant.

##### Example:
- `beta["gs"]` returns the beta function for the strong coupling \( g_s \).

##### Allowed Couplings:
- `"gs"`: Strong coupling
- `"gw"`: Weak coupling
- `"g1"`: U(1) gauge coupling
- `"yd"`: Yukawa coupling for down-type quarks
- `"yu"`: Yukawa coupling for up-type quarks
- `"yl"`: Yukawa coupling for leptons
- `"\lambda"`: Scalar quartic coupling

Note: Always the full beta function up to the two-loop order is returned. This also includes the scalar quartic coupling. 

---

## Citation

If you use these files or results from this repository in your research, please cite the associated paper https://inspirehep.net/literature/2832469

