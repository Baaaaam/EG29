this calculation run using : 
- cyclus branch: develop -- commit e94a5a3b10131d39c88e77a21dfc36074b0d29d6

- cycamore fork: https://github.com/jlittell/cycamore.git -- branch:cleanstore -- commit bc2eade822fce9f51464324b607ab4227bc7150a

the Output.xlsm file have been filled using the CYCLUS2FCO tool:
- https://github.com/Baaaaam/CYCLUS2FCO, branch: master -- commit 549a63beee22e008c280be81167beae8d4d4f6be

the present simulation includes :

Bo-Feng - ANL - EG23 deployement schedule for all reactors.
the lifetime of each reactor have been set to 80y.

Separation of the LWR are made in a commun facility (R.Carlsen number https://github.com/rwcarlsen/eg23-sim), 3 are deployed : 2 in 2030, 1 in 2040.

Separation for FBR are greedy... (throughput 5e6, Pu output buffer 5e6 so about 1000 batch of MOX)

SFR fuel Fabricationare not gready : 1 fab for 10 SFR reactor deployement schedule, the internal parameters allow a little bit more than 10 MOX batch/y


each fuel type (UOX-A/B and SFR-A/B) have they own dedicated cooling storage (7y) and storage.

I have try to put all communs archetypes and recipes in the recycle.xml file, and each reactor type dedicaced ones in the other xml file...