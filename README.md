# PyMOL4Spliceosome: all spliceosome structures in one PyMOL session

[![Twitter Follow](http://img.shields.io/twitter/follow/rna_tools.svg?style=social&label=Follow)](https://twitter.com/rna_tools) [![tag](https://img.shields.io/github/release/mmagnus/PyMOL4Spliceosome.svg)](https://github.com/mmagnus/PyMOL4Spliceosome/releases) [![DOI](https://zenodo.org/badge/doi/10.1093/nar/gkz1108.svg)](http://dx.doi.org/10.1093/nar/gkz1108)

This project is a part of my rna-tools, so please cite this paper if you find this repository useful for you:

Magnus M, Antczak M, Zok T, Wiedemann J, Lukasiak P, Cao Y, Bujnicki JM, Westhof E, Szachniuk M, Miao Z. 
RNA-Puzzles toolkit: a computational resource of RNA 3D structure benchmark datasets, structure manipulation, and evaluation tools. Nucleic Acids Research. 2019 10.1093/nar/gkz1108
https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkz1108/5651330

**Tip: the session now is very big and it might slow your computer. We recommend to open it one, remove unnecessary things for your analysis and save it as a new session.**

Processed PyMOL session of cryo-em structures, see https://github.com/mmagnus/PyMOL4Spliceosome/releases to learn more about current stage of the project.

<a href="https://github.com/mmagnus/PyMOL4Spliceosome/releases"><img width="1283" alt="Screen Shot 2019-09-13 at 9 28 20 AM" src="https://user-images.githubusercontent.com/118740/64844794-e9aca900-d608-11e9-8191-379037eaaa3e.png"></a>
(BTW, the intron here is in black, it's fixed in the version 0.31, now the intron is in gray)

The structures superimposed based on the U6 RNA (if possible)

Colors and chain mapping based on pyMoL_colors-EMX.xlsx prepared by Eysmont and Magnus.

Not everything is perfect, expect some updates soon.

See https://github.com/mmagnus/PyMOL4Spliceosome/releases

and read more about the tool used to obtain this session: https://github.com/mmagnus/rna-tools/blob/master/rna_tools/tools/PyMOL4RNA/README.md


## Select all U6

![](docs/demo-u6.gif)

## Morph between two main conformations of U6

![](docs/demo-u6-morph.gif)

## Tips

    With Up Down with Righ-mouse Click

## Quick reference

	PyMOL>enable CWC15*
	PyMOL>disable CWC15*

    # select only some objects and save it to the file
    save /Users/magnus/Desktop/XXXX_triplex_zoom.pse, CXXX_P and U2_P and U6_P

    select U4* and resi 68-81
    
Read more: https://pymolwiki.org/index.php/Enable

## External

You can also download sessions for single steps prepared by the Nagai lab: <https://www2.mrc-lmb.cam.ac.uk/groups/nagai/resources/> and here <https://github.com/maxewilkinson/Spliceosome-PyMOL-sessions>

## Aligned

	save aligned/hB_6AHD.pdb, PRP_hB_6AHD
	
	align h3_6QW6 and chain 5A, PRP8_hB_6AHD
	save 
	
	fetch 6QX9
	align 6QX9 and chain 5A, PRP8_hB_6AHD	
	save hBpre_6QX9.cif, 6QX9

	fetch 6QW6
	align 6QW6 and chain 5A, PRP8_hB_6AHD	
	save h3_6QW6.cif, 6QW6

## Rings as one object

	extract Lsm_ring_h3_6QW6, (chain 62 and h3_6QW6) or (chain 64 and h3_6QW6)
	
	extract Lsm_ring_h3_6QW6, (chain 62 or chain 64) and h3_6QW6

# Sandbox

	PyMOL>select chain 5A and name hBpre_6QX9
    Selector: selection "sele" defined with 0 atoms.

# Changelog
[dev]

- Exon_Ba/N/ 100-114 gray50 it's intron, not exon, yBa_5GM6.pse
- Rings as one

# Index

All processed structures in this repository:

https://github.com/mmagnus/rna-tools/blob/master/rna_tools/tools/PyMOL4RNA/Spliceosome_PyMOL.csv

![](docs/tab1_Zhao.jpeg)

Source: L. Zhang, A. Vielle, S. Espinosa, and R. Zhao, “RNAs in the spliceosome: Insight from cryoEM structures,” WIREs RNA, vol. 10, no. 3, pp. e1523–11, Apr. 2019.

Update to the Table 1.

| Complex   | Species | PDB ID | Resolution (Å) | Lab           | Reference               |
|-----------|---------|--------|----------------|---------------|-------------------------|
| Tri-snRNP | Human   | 6QW6   | 2.92           | Kiyoshi Nagai | Charenton et al. (2019) |
| Pre-B     | Human   | 6AHD   | 3.80           | Yigong Shi    | Zhan et al. (2018)      |
| B         | Human   | 6AHD   | 3.80           | Yigong Shi    | Zhan et al. (2018)      |

Mechanism of 5' splice site transfer for human spliceosome activation. Charenton, C., Wilkinson, M.E., Nagai, K. (2019) Science 364: 362-367

Structures of the human pre-catalytic spliceosome and its precursor spliceosome. Zhan, X., Yan, C., Zhang, X., Lei, J., Shi, Y. (2018) Cell Res 28: 1129-1140

# Acknowledgement

ReMedy-International Research Agenda Unit, Centre of New Technologies, University of Warsaw, 02-097 Warsaw, Poland

M.M. was supported by the "Regenerative Mechanisms for Health-ReMedy" grant MAB/20172, carried out within the International Research Agendas Program of the Foundation for Polish Science co-financed by the European Union under the European Regional Development Fund.

# Supplements


yBa_5GM6
5GM6
Cryo-EM structure of the activated spliceosome (Bact complex) at 3.5 angstrom resolution

Structure of a yeast activated spliceosome at 3.5 angstrom resolution
Yan, C., Wan, R., Bai, R., Huang, G., Shi, Y.
(2016) Science 353: 904-911

PubMed: 27445306 Search on PubMed
DOI: 10.1126/science.aag0291

