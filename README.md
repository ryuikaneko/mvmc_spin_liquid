# spin liquids and unconventional ordered states by mVMC

## What do these scripts do?

* Description of spin liquids and unconventional ordered states
  by fermionic wave functions such as the projected BCS states
  and the Slater-Jastrow-type wave functions
* Use [mVMC](https://github.com/issp-center-dev/mVMC)
  with the generalized pairing wave functions
  that include the projected BCS states
  and the Slater-Jastrow-type wave functions

## References

* mVMC
  * [DOI:10.1143/JPSJ.77.114701](https://doi.org/10.1143/JPSJ.77.114701)
  * [DOI:10.1016/j.cpc.2018.08.014](https://doi.org/10.1016/j.cpc.2018.08.014)
* "Dictionary" of spin liquid ansatze
  * [DOI:10.1103/PhysRevB.65.165113](https://doi.org/10.1103/PhysRevB.65.165113)
  * [arXiv:0905.4854](https://arxiv.org/abs/0905.4854)

## Famous wave functions

(under construction)

* 1D Heisenberg model

  * Projected Fermi sea in 1D, ground state of the Haldane-Shastry model
    * Wave function
      * f_k = 1 (|k|<pi/2), f_k = 0 (|k|>pi/2)
      * Equivalent to
        \epsilon_k = - 2 \cos k,
        \Delta_k = 0,
        \mu_k = 0
        (Note that constant shift is allowed in f_k since f_ii is
        arbitrary for the hard Gutzwiller projection)
    * See
      [DOI:10.1103/PhysRevB.36.381](https://doi.org/10.1103/PhysRevB.36.381)
      [DOI:10.1103/PhysRevLett.59.1472](https://doi.org/10.1103/PhysRevLett.59.1472)
      [DOI:10.1103/PhysRevLett.60.635](https://doi.org/10.1103/PhysRevLett.60.635)
      [DOI:10.1103/PhysRevLett.60.639](https://doi.org/10.1103/PhysRevLett.60.639)

  * Ground state of the Majumdar-Ghosh model
    * Wave function
      * f_ij = 1 (|i-j|=1), f_ij = 0 otherwise
      * Equivalent to
        \epsilon_k = -2t \cos 2k,
        \Delta_k = 4\sqrt{2}t \cos k,
        \mu = 0,
        which results in f_k = \sqrt{2} \cos k
    * See
      [DOI:10.1063/1.1664978](https://doi.org/10.1063/1.1664978)
      [DOI:10.1063/1.1664979](https://doi.org/10.1063/1.1664979)
      [arXiv:0905.4854](https://arxiv.org/abs/0905.4854) 

  * VBS order with translation invariant wave functions
    * Wave function
      * Choose \epsilon_k and \Delta_k so that
        \sqrt{(\epsilon_k)^2 + (\Delta_k)^2} > 0 for all k
      * Seems valid in 1D but not sure for higher dimensions
    * See
      [DOI:10.1103/PhysRevLett.91.257005](https://doi.org/10.1103/PhysRevLett.91.257005) 
      [DOI:10.1103/PhysRevB.93.125127](https://doi.org/10.1103/PhysRevB.93.125127)

* 1D Hubbard model, t-J model

  * Tomonaga-Luttinger liquid
    * Wave function
      * Long-range part of the Jastrow factor affects the charge gap
    * See
      [DOI:10.1103/PhysRevLett.94.026406](https://doi.org/10.1103/PhysRevLett.94.026406)
      [DOI:10.1103/PhysRevB.72.085121](https://doi.org/10.1103/PhysRevB.72.085121)

  * Luther-Emery liquid
    * Wave function
      * Close the charge gap by choosing the Jastrow factor for metal
      * Open the spin gap by choosing
        \sqrt{(\epsilon_k)^2 + (\Delta_k)^2} > 0 for all k
    * See
      [DOI:10.1103/PhysRevLett.94.026406](https://doi.org/10.1103/PhysRevLett.94.026406)
      [DOI:10.1103/PhysRevB.72.085121](https://doi.org/10.1103/PhysRevB.72.085121)

* 2D Heisenberg model

  * Square lattice

    * Ground state ansatz for the pure square Heisenberg model
      * See
        [DOI:10.1103/PhysRevB.37.3774](https://doi.org/10.1103/PhysRevB.37.3774)
        [DOI:10.1103/PhysRevB.100.125131](https://doi.org/10.1103/PhysRevB.100.125131)

    * Gapless Z2 spin liquid ansatz for the J1-J2 square Heisenberg model
      (J2:next nearest neighbor)
      * Wave function
        * Z2Azz13 spin liquid defined as
          \epsilon_k = 2t(\cos k_x + \cos k_y),
          \Delta_k = \Delta_{x^2-y^2} (\cos k_x - \cos k_y)
          + \Delta_{xy} \sin 2k_x \sin 2k_y
      * See
        [nhscp2014, F.Becca](http://www.issp.u-tokyo.ac.jp/public/nhscp2014/files/talks/S3A-1Becca.pdf)
        [DOI:10.1103/PhysRevB.88.060402](https://doi.org/10.1103/PhysRevB.88.060402)
        [DOI:10.1103/PhysRevB.100.125131](https://doi.org/10.1103/PhysRevB.100.125131)

    * Projected Fermi sea
      * The state shows unexpected long-range magnetic order,
        obeys the are law in 2D
      * See
        [DOI:10.1209/0295-5075/103/57002](https://doi.org/10.1209/0295-5075/103/57002)
        [DOI:10.1103/PhysRevLett.107.067202](https://doi.org/10.1103/PhysRevLett.107.067202)
        [DOI:10.1103/PhysRevB.93.125127](https://doi.org/10.1103/PhysRevB.93.125127)

  * Triangular lattice

    * Ground state ansatz for the pure triangular Heisenberg model
      * (Short-range) 3-site order (120 Neel) is reproduced by a 2-site
        (not a 3-site!) unit cell structure
      * See
        [DOI:10.1103/PhysRevLett.92.1570031](https://doi.org/10.1103/PhysRevLett.92.157003)
        [DOI:10.1103/PhysRevB.74.014408](https://doi.org/10.1103/PhysRevB.74.014408)
        [DOI:10.1103/PhysRevB.80.012404](https://doi.org/10.1103/PhysRevB.80.012404)

    * Spin liquid ansatz for the J-J' triangular Heisenberg model (J':spatial anisotropy)
      * See
        [arXiv:cond-mat/0210662](https://arxiv.org/abs/cond-mat/0210662)
        [DOI:10.1103/PhysRevLett.92.1570031](https://doi.org/10.1103/PhysRevLett.92.157003)
        [DOI:10.1103/PhysRevB.74.014408](https://doi.org/10.1103/PhysRevB.74.014408)
        [DOI:10.1103/PhysRevB.80.012404](https://doi.org/10.1103/PhysRevB.80.012404)
        [DOI:10.1103/PhysRevB.93.085111](https://doi.org/10.1103/PhysRevB.93.085111)

    * Gapless U(1) Dirac spin liquid ansatz for the J1-J2 triangular
      Heisenberg model (J2:next nearest neighbor)
      * See
        [DOI:10.1103/PhysRevB.93.144411](https://doi.org/10.1103/PhysRevB.93.144411)
      * See also
        [DOI:10.7566/JPSJ.83.093707](https://doi.org/10.7566/JPSJ.83.093707)

    * Spin liquid with spinon Fermi surface, projected Fermi sea,
      ground state ansatz for the triangular Heisenberg model with
      the strong ring-exchange interaction
      * See
        [DOI:10.1103/PhysRevB.72.045105](https://doi.org/10.1103/PhysRevB.72.045105)

  * Honeycomb lattice

    * Spin liquid ansatz for the J1-J2 honeycomb Heisenberg model (J2:next nearest neighbor)
      * See
        [DOI:10.1103/PhysRevB.96.104401](https://doi.org/10.1103/PhysRevB.96.104401)

  * Kagome lattice

    * Gapped Z2 spin liquid ansatz
      * See
        [DOI:10.1103/PhysRevB.84.020407](https://doi.org/10.1103/PhysRevB.84.020407) 
        [arXiv:1601.02165](https://arxiv.org/abs/1601.02165)
      * See also (not VMC but)
        [DOI:10.1126/science.1201080](https://doi.org/10.1126/science.1201080)
        [DOI:10.1103/PhysRevLett.109.067201](https://doi.org/10.1103/PhysRevLett.109.067201)

    * Gapless U(1) Dirac spin liquid ansatz
      * See
        [DOI:10.1103/PhysRevLett.98.117205](https://doi.org/10.1103/PhysRevLett.98.117205)
        [DOI:10.1103/PhysRevB.84.020407](https://doi.org/10.1103/PhysRevB.84.020407) 
        [DOI:10.1103/PhysRevB.91.020402](https://doi.org/10.1103/PhysRevB.91.020402)

* 2D Hubbard model

  * Charge order with translation invariant wave functions
    * See
      [DOI:10.1103/PhysRevB.93.125127](https://doi.org/10.1103/PhysRevB.93.125127)

* 3D Heisenberg model

  * Pyrochlore lattice

