# NMR-library
## tk506's library of Pulse sequences 
Made for Bruker Topspin >= 4.2

### Relaxometry

* `cpmg_cpmgd.tk506` – CPMG sequence with CPMG detection for single-scan $T_2$ measurements (TD, 2D).
* `satrec_cpmg.tk506` – Saturation recovery with CPMG detection for $T_1$-$T_2$ correlation plots (3D, simplified from diffREXSY).
* `satrec_cpmg_1d.tk506` – 1D variant of saturation recovery with CPMG detection for $T_1$-$T_2$ correlation plots.
* `satrec_cpmg_2d.tk506` – 2D variant of saturation recovery with CPMG detection for $T_1$-$T_2$ correlation plots.
* `satrec_cpmgd.tk506` – Saturation recovery with CPMG detection for single-scan $T_2$ (TD, 2D).
* `cpmg_cpmg.tk506` – $T_2$-$T_2$ Exchange experiment (3D, Washburn and Callaghan, *PRL* 2006).

### Time-Resolved

* `ineptrd2d.tk506` – Time-resolved INEPT for non-selective polarization transfer with decoupling during acquisition (pseudo-2D).
* `zgesgp2d.tk506` – Time-resolved water suppression using excitation sculpting with gradients (pseudo-2D).
* `zgig2d.tk506` – Time-resolved 1D with heteronuclear decoupling for *In Situ* monitoring (pseudo-2D).

### Exchange

* `quest.tk506` – Applies saturation of increasing duration to study chemical exchange via QUEST experiments (pseudo-2D).
* `questi.tk506` – Saturation of increasing duration with interleaved $+cnst1$/$-cnst1$ offsets.
* `quesp.tk506` – Applies saturation of increasing power (using a Watt power list) to study exchange.
* `quespi.tk506` – Saturation of increasing power with interleaved $+cnst1$/$-cnst1$ offsets.
* `zgcest.tk506` – zgCEST sequence to monitor exchange by saturating offsets defined in `FQ1LIST` prior to 1D acquisition (pseudo-2D).

### Relaxation

* `cpmg_T2_1d.tk506` – CPMG sequence with added phase cycling for fast $T_2$ measurements with signal averaging (1D).
* `hahnecho2d_vc.tk506` – Hahn echo recorded at the peak to eliminate first-order phase correction, using a VC list.
* `hahnecho2d_vd.tk506` – NQR-compatible Hahn echo recorded at the peak using a VD list.
* `T1rho.tk506` – Direct measurement of $T_1\rho$ relaxation with auto-calculated spin-lock power (based on `cpht1rho.av`).
* `T1_oneshot.tk506` – Rapid $T_1$ determination via continuous wave free precession without phase cycling (Moraes et al., *JMR* 2016).

### Solids

* `cphahn.tk506` – Cross-polarization followed by a Hahn echo.
* `cphahn2d.tk506` – Cross-polarization followed by a rotor-synchronized Hahn echo using a `vd_list` (2D).
* `cpEXSY.tk506` – Phase-sensitive 2D homonuclear correlation via dipolar coupling or chemical exchange (noesyph-based).
* `cpSPINDIFFredor.tk506` – CP-SPINDIFF followed by REDOR filtering after the mixing time to dephase near target nuclei like $^{31}\text{P}$ or $^{15}\text{N}$ (2D).
* `cpredorSPINDIFF.tk506` – REDOR filter applied before mixing time followed by CP-SPINDIFF for symmetric 2D spectra.
* `gscpSPINDIFF.tk506` – Basic 2D homonuclear exchange experiment via CP-SPINDIFF.
* `dcpHXH2D.tk506` – 1D/2D $^{13}\text{C}$-$^{1}\text{H}$ CP experiment featuring HC CP, CH CP, and $^{1}\text{H}$ detection.
* `holeburn_lgcp_2d.tk506` – $^{1}\text{H}\{{}^{13}\text{C}\}$ REDOR hole burning with homonuclear decoupling for interface editing (pseudo-2D) (Chen, Schmidt-Rohr et al., *Solid State Nuclear Magnetic Resonance*, 2006).
* `homofslg.tk506` – 2D $^{1}\text{H}$-$^{1}\text{H}$ MAS FSLG experiment used to reference the indirect dimension of HETCORs (Kumari et al., *App. Mag. Res.* 2019).
* `pc72daswf.tk506` – SQ-DQ correlation experiment using the POST-$\text{C}_7$ sequence (fixed phase cycling for TopSpin 4.4.0+).
* `pc7cp2daswf.tk506` – 2D SQ-DQ correlation experiment with POST-$\text{C}_7$ and cross-polarization (fixed phase cycling for TopSpin 4.4.0+).
* `slgscp_pmz.tk506` – Spinlock Goldman-Shen experiment for cell interface editing (Kress & Duer, *Comms. Chem.* 2025).
* `slgscp_pmz_2d.tk506` – 2D variant of the spinlock Goldman-Shen cell interface-editing experiment (Kress & Duer, *Comms. Chem.* 2025).

### General / Root Directory

* `hahnecho.tk506` – Static Hahn echo experiment recorded at the echo peak to eliminate first-order phase correction.
* `p1popt.tk506` – Records nutation curves outside the standard `popt` module using a `VPList` in $\mu\text{s}$ (pseudo-2D).
* `zgtrip.tk506` – Triple-pulse excitation sequence that suppresses probe background signals and RF acoustic ringing via destructive interference (Wang et al., *JMR* 2021).

### Trigger

* `trig_send.tk506` send TTL trigger pulse on TTL1 
* `trig_wait.tk506` wait for TTL trigger pulse on TTL1 
Note:
- Orange = TTL output 1
- Blue = TTL output 2
- Green = TTL output 3
- Brown  = TTL output 4