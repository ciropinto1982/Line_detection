# Automated m-D SPEX codes to search for outflows in X-ray spectra

These automated and multi-domensional codes take advantage from SPEX knowledge of atomic lines cross section and energy centroids as well as relatives strength according to the given ionisation balance (and elemental abundances). The routines are optimised to speed up the spectral fits over a well defined deep grid of points in the paramers space (e.g. log_xi, kT, N_H, n_e, v_LOS, etc.) by adopting an ad-hoc structure and parameters initialisation. The main difference between photo- and collisionally-ionised codes is the need for a broadband band spectral energy distribution (SED) or ionising radiation field for the former.

1) SPEX_pion_grid_fast_input directory has modules to build SPEX's model PION (emission/absorption lines from photo-ionised plasma).

2) SPEX_xabs_grid_fast_input.sh is built on SPEX's model XABS. It reproduces & models absorption lines of photo-ionised plasma.

3) SPEX_ciez_grid_fast_input.sh is built on SPEX's model CIE (emission lines from collisionally-ionised plasma). It adopts the kT logarithmic grid stored in the file Val_CIE_T_loggrid.txt.

4) SPEX_hotz_grid_fast_input.sh is built on SPEX's model HOT (absorption lines from collisionally-ionised plasma). It adopts the kT logarithmic grid stored in the file Val_CIE_T_loggrid.txt.

5) SPEX-models-flowchart.jpeg provides an overview on the SPEX physical model scans and their architecture.

6) PYTH_read_grid_results.py is a simple PYTHON script that reads and plots SPEX results from an automated grid. This example shows how to plot Delta C-stat probability contours.

*License -* All these codes have been developed for and published in the paper Pinto et al. (2020b), doi: 10.1093/mnras/staa118, arXiv: 1911.09568, bibcode: 2020MNRAS.492.4646P. You're recommended and kindly requested to refer to that paper when using this code.
