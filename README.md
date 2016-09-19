this calculation run using : 
this should be running with last CYclus/Cycamore version

the present simulation includes :

The input file for the different cases of the EG29 calculation:
  - Case 1: PWR loop only
  - Case 2: FBR loop only
  - Case 3: steady state of FBR/PWR (70/30 of the generated power)
  - Case 4: the actual transition

For each/some cases subacses have been considered:
  - x.1: lumbed composition, no decay
  - x.2: isotopic composition, no decay
  - x.3: isotopic composition, decay


Different declinaison have been perform on each cases, changing some modeling
choises:
  - basic (no sufix): fuel fabrication using cycamore::fuel_fab
  - MF: fabrication done with cicamore::Mixer
  - MLP: fab/depletion  done with MLP CLASS model (fix K_threshold)
  - MLP_STD: fab/depletion done woth MLP CLASS model (K_threshold def at 1.03i,
    3 batches)
  - MLP_STD_2: fab/depletion fone with MLP CLASS model( K_ths=1.03, 4 batches)
  - MLP_recipe: fab MLP CLASS (k_ths=1.03, 3batches) + recipe reactor
  - LII_xx incease initial storage (force decay effect) -- xXX multiply by --
    10/50/100 to be checked
  _ UOX_start: transition from actual US fleet
  - XXX_inv: add the inventory in output file
  _ pucomp

