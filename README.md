# Protein Characteristics

- Sequence
- Structure
- Function
- Interactions

then derive homologies, phylogeny, domains etc.

disorder proteins - either fully or disorder domains/stretches

## Collect and compare proteins

database ontologies - hierarchical
e.g. UniProt

download fasta for Hsp90 (P07900) and HtpG (P0A6Z3)

measure order disorder with IUPred2a on them

over the line means disorder 
both proteins are from the same family but in human and bacteria?

ANCHOR gives signal for interaction domains

## protein data bank to look at structure

downloaded pdb files - special file format for structural model from PDB
IDs: 2IOP E.coli , 5FWK Homo

## PDB 101

extra database with good illustrations - better than spaghettis

## Protein blast

to find homology or homologous sequences for phylogenetic experiments

downloaded the blast hits as fasta files

## jalview

load the blasted seqs in jalview and align with clustalO

color by AA and enables manual curation of alignments

a missing bit of sequence when comparing mammalian and bacterial proteins
- represents the peak of disorder in the first plot from IUPred2a

## SWISS-MODEL

homology modelling - structure is more conserved than sequence

there might be more similarity in structure from varying sequences

the bit with disorder is sticking out of the model
- linker domain - might have importance for function
- missing in bacteria


# Short Linear Motifs --- SLiMs

high throughput experimental approaches

patterns are encoded by or: [] not: ^ any: .

## ELM - eukaryotic motif database

work through extra word document
make screenshot

## Chimera

another extra doc

for visualizing structures

explored the binding between protein and ligand

split them to see the surface between protein and ligand

can infer the Hbonds - but not between the split parts any longer

## PFAM

database for domains - wikipedia style

## human protein atlas

database for the localisation of proteins in cells

## back to ELM

align two proteins with MatchMaker and select aligned residues 

use different show methods to highlight things like motifs


## looking at an alignment of peptides in jalview

very short aligned peptides to infer slims






# Eustermann part

intro to fourier analysis & analysis of single molecule cryoEM (ecoli ribosomes)

reconstruct 3D structure from EM projections - projection slice theorem
- FFT different 2D projected images
- assemble the 2D fourier transforms into 3D
- invert Fourier transform on assembled 2D fourier slices

## Fourier analysis

construction of waves by fourier series of additive sine waves
- Amplitude, freq, period, phase -> describe wave

different description through complex numbers: fourier transform returns the complex numbers 
that describe the amplitude and phase information of each wave

power spectrum: visualization of additive sine waves with frequency on x axis
- fourier space is the extension into 2D with the pixel intensity corresponding to the height of peaks in 1D

convolution and cross correlation become multiplication operations in fourier space
- computationally efficient

## reconstruct ribosome from 50 micrographs

using RELION - analysis pipeline 
- incl motion correction
- motion induced from overall sample motion and beam-induced particle motion
- corrected by acquiring stacks instead of single frames


checked the power spectra of motion corrected and raw movies
- motion corrected show more high frequency information
- means sharper resolution is possible
- because of the outer rings that are visible in the motion corrected power spectrum


auto-picked the particles from all micrographs

extracted particles

classification of the particles into classes from the 2D data
- clustering and averaging of particles in the same rotation
- improves with each iteration because of the averaging 
- classes become more separated with each step




## radiation damage

elastic and inelastic scattering of electrons
- inelastic causes radiation damage in the sample through stochastic interactions




















git -c user.name='W-L' -c user.email='lukas.weilguny@24speed.at' commit -m '...'






