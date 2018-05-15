## How to make any changes to the website
If you want to make any changes to the website, first fork the repository, make your changes to your forked version, and then submit a pull request.

## How to add someone to the people page
To add a new person to the people page (`/people.html`), add a new entry to `_data/people.yml`.
The names should be sorted in alphabetical order by last name, regardless of their position.

## How to add a photo
To add a photo of yourself or another person, put the photo into `assets/img` and follow the filename pattern.
Then, add or update your entry in `_data/people.yml` to point to your new photo.
The photos are displayed at 170px by 170px.
See [this pull request](https://github.com/penn-nlp/penn-nlp.github.io/pull/3) for an example.

## How to add someone to the alumni page
To add a new person to the alumni page (`/alumni.html`), create a new entry in `_data/alumni.yml`.
The entries should be sorted by graduation year followed by last name.
