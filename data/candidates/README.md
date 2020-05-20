# Contents

## Candidates from Fragment Network


These are virtual scrrening candidates expanded out from the fragment screening hits using the Fragment Network.
For info on how this works see:
* https://fragnet.informaticsmatters.com/
* https://github.com/InformaticsMatters/fragnet/tree/master/fragnet-search

There are pairs of file, a JSON format file that contains the results of the expansion and a file in SMILES format with
the structures extracted from that file. 

The best file to use are those named `expanded-22_hac0-10_rac0-3_hops3` which correspond to the current 22 fragment screening hits
expanded out used fairly aggressive parameters to generate ~85K molecules.

The files named expanded-17 were from the original 17 hits and expanded with less aggressive parameters (~42K molecules).

The files named expanded-24 contain 2 non-active site hits and should not be used but are retained for historical record. 
