# Codenames task set for DreamTeam (CHI 2018)

This is the Codenames task set used for DreamTeam, a system introduced in the CHI 2018 paper [*In Search of the Dream Team: Temporally Constrained Multi-Armed Bandits for Identifying Effective Team Structures*](http://hci.stanford.edu/publications/2018/dreamteam/zhou_sharon_dreamteam.pdf) (Sharon Zhou, Melissa Valentine, Michael Bernstein). 

## Using this task set
There are 11 game boards in a list of dictionary objects. Each board is enclosed in a dictionary object, e.g. 

```
{
    "dice":
        [
            "processor",
            "dots",
            "chance"
        ],
    "invalid":
        [
            "null",
            "patient"
        ],
    "compress":
        [
            "swelling",
            "encode"
        ]
}
```

Here, "dice", "invalid", and "compress" are clues used for the board. 

The board itself does not include the clues, and is comprised of the words "processor", "dots", "chance", "null", "patient", "swelling", and "encode" --- ideally scrambled in random order. 

The common way of presenting clues is "dice, 3" which indicates that there are 3 words on the board ("processor", "dots", "chance") corresponding to the clue "dice".

## About Codenames and this adaptation
This task is adapted from the popular board game, [Codenames](https://en.wikipedia.org/wiki/Codenames_(board_game)). 

The premise of the game is that there is a board of words, e.g. "cat", "tree", "dog". There are then clues corresponding to a subset of words on the board, e.g. "pet, 2" where *pet* refers to *2* words on the board and "plant, 1" where *plant* refers to *1* word on the board.

The players do not know which are the correct words and have to decide on which words to guess. In this adaptation, each word has only one clue. In traditional Codenames, words can have many clues.