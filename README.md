# link_spam_compute_ranks

One of the problems with our page ranking system is pages can collude with each other to improve their page ranks. We consider A->B a reciprocal link if there is a link path from B to A of length equal to or below the collusion level, k. The length of a link path is the number of links which are taken to travel from one page to the other.

If k = 0, then a link from A to A is a reciprocal link for node A, since no links needs to be taken to get from A to A.

If k=1, B->A would count as a reciprocal link
If there is a link A->B, which includes one link and so is of length 1, it requires two parties, A and B, to collude to increase each others page rank.

If k=2, B->A would count as a reciprocal link for node A.
A path A->C->B, for some page C, (link path of length 2),or a direct link A-> B (link path of length 1).
