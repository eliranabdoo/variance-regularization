# variance-regularization
A small research project for exploring the assumption that the number of attention heads in BERT is excessive.
My main idea was to condradict by conjecturing there's a tendendency to local minima in BERT induced loss functions, in areas where the attention heads are similar.
To overcome that, I've added a penalty term to the loss function, that penalizes low average point-wise variance across the attention heads.
There are many places to tweak it (using KQV or just some of them, varaince averaging methods, penalty weighting methods), but so far I didn't observe any noticable improvement.
TBD
