# Turbonet_person-reid
Person Re-identification with a small, custom CNN

# What happened?
I defined a small, simple CNN, based on SqueezeNet's fire modules with some depthwise convolutions in between.
I trained this net as a classifier on a self-made dataset with 10000 pictures over 10 classes of different collegues.
Then I ran this as a siamese network, with just a cosine similarity layer added.
Created a symmetric data generator, and trained the network to minimise binary_crossentropy.
570k parameters in the CNN, on that custom dataset an accuracy over over 99.9%.
CUHK01 mAP seems to be somewhere around 75%, but this should be tested decently.
