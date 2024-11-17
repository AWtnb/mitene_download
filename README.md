Download medias from https://mitene.us/ or https://family-album.com/ to keep a local backup.

## Usage

From mitene app, invite a family member for the web version and copy the URL ( that should be something like `https://mitene.us/f/abcd123456` )

Run the script with `python .\mitene_download.py https://mitene.us/f/abcd123456 -sy 2024 -sm 11 -sd 11`, using the URL from previous step.

This will download photos and video taken after 2024-11-11 in `out` folder. Some text files will be created with the comments.

If the album is password-protected, you can specify the password using `--password` command line argument, similar to this: `mitene_download https://mitene.us/f/abcd123456 --password the_password`.
