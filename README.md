import random

print('I will flip a coin 1000 times. I will then do so 4 more times and tell you the average of the 5 trials. (Press enter to begin)')
input()

def rolls():
    
    flips = 0
    heads = 0

    while flips < 1000:
        if random.randint(0, 1) == 1:
            heads = heads + 1
        flips = flips + 1
    return heads

turns = 0
headz = 0
tailz = 0


while turns != 5:
    headz = headz + rolls()
    diff  = 1000 - rolls()
    tailz = tailz + diff
    turns = turns + 1
    

avgHeads = headz / 5
avgTails = tailz / 5

print('The average number of heads was ' + str(avgHeads) + ' time and tails came up ' + str(avgTails) + ' times.')
