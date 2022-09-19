Here we provide the tabulated pair potentials used in our final simulations. The tables are intended for `LAMMPS`. To combine these pair potentials with the subtracted model, specify something like

```
pair_style	hybrid/overlay table linear 1194 deepmd graph.pb
pair_coeff	* * deepmd
pair_coeff	1 1 table full.table La_La 2.72
pair_coeff	1 2 table full.table La_H 2.02
pair_coeff	2 2 table full.table H_H 0.74
```

where particle 1 represents lanthanum and particle 2 represents hydrogen in this case.

The lanthanum ECP used to calculate these energies is from Basis Set Exchange, and can be found [here](https://www.basissetexchange.org/basis/def2-qzvppd/format/nwchem/?version=1&elements=57).
