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

Read more: https://pymolwiki.org/index.php/Enable

## External

You can also download sessions for single steps prepared by the Nagai lab: <https://www2.mrc-lmb.cam.ac.uk/groups/nagai/resources/>

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

- Rings as one

# Acknowledgement

ReMedy-International Research Agenda Unit, Centre of New Technologies, University of Warsaw, 02-097 Warsaw, Poland

M.M. was supported by the "Regenerative Mechanisms for Health-ReMedy" grant MAB/20172, carried out within the International Research Agendas Program of the Foundation for Polish Science co-financed by the European Union under the European Regional Development Fund.
