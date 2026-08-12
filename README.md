# Almanac

A day of the week trainer, built around Dominic O'Brien's calendar method.
You are shown a date between 1900 and 2099, you name the day, and you can
then check your working against the codes.

Live at https://scottjbarrie.github.io/DateTester/

There is nothing to install and no build step. Opening `index.html` in a
browser works just as well.

## How the working panel reads

Each date breaks into four codes that add together, casting out sevens as
you go:

- the day of the month
- the month
- the year, which is where your character lives
- the century, plus a leap year adjustment where it applies

The year row also shows the character card for that two digit year, so the
picture sits directly beside the number it stands for.

## Adding your own characters

Everything you edit sits at the top of `index.html`, under `YOUR PALACE`.

- `ROOMS` holds the seven areas, one for each year code from 0 to 6
- `PEOPLE` holds the names, keyed by two digit year
- `MONTH_HINTS` holds the prompt for each month

Change only the text inside the quote marks. Leave the numbers and the
punctuation as they are.

## Character pictures

Pictures live in the `people` folder, named by two digit year, for example
`people/25.png`. Both `.png` and `.jpg` are handled, so a new picture can be
dropped in as whichever it happens to be. If a picture is missing, the row
simply shows without one.

They display at 88 by 132 and are stored at roughly twice that, so they stay
sharp on a phone without making the repository heavy.
