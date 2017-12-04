# pal2nal_gblocker
produce a nucleotide alignment that corresponds with a GBLOCKED amino-acid alignment

## INSTALLATION

To install `pal2nal_gblocker` and documentation, type the following:

    perl Makefile.PL
    make
    sudo make install

To install without root privelages try:

    perl Makefile.PL PREFIX=/home/myuser/scripts
    make
    sudo make install

### SYSTEM REQUIREMENTS

Requires Gblocks http://molevol.cmima.csic.es/castresana/Gblocks.html
and PAL2NAL http://www.bork.embl.de/pal2nal/#Download

The `Gblocks` and `pal2nal.pl` binaries should be in your path

## AUTHOR
    Aaron Szczepanek <aaron@whitney.ufl.edu>, Joseph F. Ryan
    <joseph.ryan@whitney.ufl.edu>

## SYNOPSIS
    pal2nal_gblocker --mafft=MAFFT_FILE --fasta=FASTA_FILE [--outdir=OUTDIR]
    [--version] [--help]

## OPTIONS
    --mafft
      This is an alignment in FASTA format from the program MAFFT.

    --fasta
      This is a FASTA file of CDS sequences that correspond to the mafft
      file

    --outdir
      If provided, intermediate files will be placed in this directory

    --help
      Print this manual

    --version
      Print the version

## DESCRIPTION
    This program will accept an amino-acid alignment and corresponding CDS
    file, and produce a nucleotide alignment that corresponds with a
    GBLOCKED alignment.

## TODO
    Allow users to send options for GBLOCKS and for pal2nal

## BUGS
    Please report them to any or all of the authors.

## COPYRIGHT
    Copyright (C) 2017 Aaron Szczepanek, Joseph F. Ryan

    This program is free software: you can redistribute it and/or modify it
    under the terms of the GNU General Public License as published by the
    Free Software Foundation, either version 3 of the License, or (at your
    option) any later version.

    This program is distributed in the hope that it will be useful, but
    WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
    Public License for more details.

    You should have received a copy of the GNU General Public License along
    with this program. If not, see <http://www.gnu.org/licenses/>.
