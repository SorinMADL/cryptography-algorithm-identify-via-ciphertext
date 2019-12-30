# See if and given text is an random str-ascii-chr or is an aes ciphertext

For start, i generated 1 big dataset to feed my model, 100k training values, 99k used for train, 500 for dev set and 500 for test set.

The model is a relativ. deep NN.
The last ACC on train, dev and test set was 100 %.

OBSV:
  - After I used normalization, i had i performance increase: from ACC = 94% to 99% (+-)
  - After I applied a good dropout my ACC increased with min 0.5 % (and that's a lot, cuz my last ACC was about 99%)
  - And to achive such a great performance (from my point of view) i chosed the learning rate 0.0001 for and ADAM optimization 
    alghoritm (with a minimbatch = 1% from len(train_set)).
    PS: (with a smaler minibatch, my alg refuse to learn)
    
Auth: Martinescu Sorin-Alexandru (Ro, Bucharest)
