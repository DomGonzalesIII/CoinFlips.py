# coinFlips
# First try given program description before viewing code
import random

flips = 0
heads = 0

while flips <1000:
    flip = random.randint(1,2)

    if flip == 1:
        heads = heads + 1
    else:
        heads = heads

    flips = flips + 1

tails = 1000 - heads
print('Of 1000 flips, ' + str(heads) + ' were heads and ' + str(tails) + ' were tails.')
