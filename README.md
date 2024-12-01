# free handles scrapper

## Prequisite

  `$ pip install -r requirements.txt`

## Usage

Find the best available handles:

  `$ python script.py 'https://bsky.app/profile/' 'Oops!' handles.txt output.txt '1,3'`

Where `https://bsky.app/profile/` is the profile's base URL, `'Oops!'`
identifies the page shown if a profile doesn't exist (and could be available),
`handles.txt` lists the handles to check, `output.txt` logs handles triggering
an `'Oops!'` page, and `'1,10'` defines the random delay range (in seconds)
between requests.

Add the optional `--with-log-file log.txt` argument to log the tested URLs and
their corresponding HTML content. This can help identify patterns that
differentiate between found and not-found profiles.
