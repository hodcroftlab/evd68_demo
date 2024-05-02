# EV-D68 Demo

This demo includes a selection of EV-D68 sequences - full-genome. Or are they? They should be, for this run!

**Can you create a Nextstrain workflow Snakefile that will do everything needed to make a Nextstrain build?**

# Get the main steps working

Clone this directory to your local computer so you can start playing with the files. Ask Emma if you need help cloning.

Use the [Zika tutorial Snakefile](https://github.com/nextstrain/zika-tutorial/blob/master/Snakefile) as a starting point!
Create your own Snakefile in the directory, and start to fill it in based on the Zika Snakefile.

*Hint: Add files and rules to the Snakefile one by one as you go, so you can more easily spot mistakes!*

You'll need to add a reference sequence to align and then to label where genes start and end. Have a look at the [reference sequence used by the Zika tutorial](https://github.com/nextstrain/zika-tutorial/blob/master/config/zika_outgroup.gb) and note the type of file it is. A `.gb` (Genbank) file. 

There are official reference sequences stored by NCBI. For EV-D68, we often use the earliest known sequence, called 'Fermon'. 

# Don't forget to check the output!

In particular, note that the `filter` step can take a list of sequences to be excluded. Are there some that look questionable, that you should remove from the build? Are there other attributes you might want to filter sequences by - date, or sequence length? Don't forget you can always type `augur filter` to see what options are available.

You should have a quick look at intermediate files (if you can) as you go, but also carefully look at your final build. How does it compare to the [official EV-D68 build](https://nextstrain.org/enterovirus/d68/genome)? (It will be smaller - but otherwise?) You might need to change things and run again :) 

# Change up the title and attributes

The `config/auspice_config_zika.json` is copied from the Zika Tutorial - so it may not be ideal for EV-D68! How can you change it so that it fits better to the virus, and can you adjust how it displays? 


# Add clades!

Once you have a built a fairly good tree, we can try to annotate it with clades - chat with Emma!