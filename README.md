# progress

Simple command line progress bar for Matlab

## Example

`64%  [##############################..................]`

## Usage

`progress('_start')` initializes a new progress bar. Must always be called first.

`progress(i)` updates the progress bar. `i` is a percentage.

`progress(i, m)` is similar, but a percentage is automagically calculated, where `i` is the current step and `m` the maximum number of steps.

`progress('_end')` ends the progress bar.

`progress('_erase')` ends the progress bar and removes if from the command window, restoring it to the way it was before the progress bar was initiated.

`progress(message)` ends the progress bar and adds message after the bar.

`progress(..., opts)` uses options from the struct opts. See below.

## Options
`opts.percentageLength`: sets the number of characters reserved for the percentage display (default: 5)

`opts.barLength`: sets the number of characters reserved for the progress bar (default: 48)

`opts.charEmpty`: sets the "empty" character (default: '.')

`opts.charFilled`: sets the "filled" character (default: '#')