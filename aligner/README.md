There are several python programs here (`-h` for usage):

-`./align_dice` aligns words using the Dice coefficient method.

-`./align_ibm_model_1` aligns words using IBM Model 1.

-`./align_ibm_model_1_bidirectional` aligns words using IBM Model 1 and incorporates both translation directions when predicting alignments.

-`./align_ibm_model_2` aligns words using IBM Model 2.

-`./align_ibm_model_2_bidirectional` aligns words using IBM Model 2 and incorporates both translation directions when predicting alignments.

-`./check-alignments` checks that the entire dataset is aligned, and
  that there are no out-of-bounds alignment points.

-`./score-alignments` computes alignment error rate.

The scripts output alignments to stdout, so you should use output piping.

The `data` directory contains a fragment of the Canadian Hansards,
aligned by Ulrich Germann:

-`hansards.e` is the English side.

-`hansards.f` is the French side.

-`hansards.a` is the alignment of the first 37 sentences. The 
  notation i-j means the word as position i of the French is 
  aligned to the word at position j of the English. Notation 
  i?j means they are probably aligned. Positions are 0-indexed.
