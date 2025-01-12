Download medias from https://mitene.us/ or https://family-album.com/ to keep a local backup.

## Usage

From mitene app, invite a family member for the web version and copy the URL ( that should be something like `https://mitene.us/f/abcd123456` )

Run the script with `python .\mitene_download.py https://mitene.us/f/abcd123456 -s 2024-11-07`, using the URL from previous step.

This will download photos and video taken after `2024-11-07T00:00:00+0900` in `out` folder. Some text files will be created with the comments.

If the album is password-protected, you can specify the password using `--password` command line argument, similar to this: `python .\mitene_download.py https://mitene.us/f/abcd123456 -s 2024-11-07 --password the_password`.

Download concurrency can be specified with `--concurrency` command line argument: `python .\mitene_download.py https://mitene.us/f/abcd123456 -s 2024-11-07 --password the_password -c 10`.


> [!NOTE]
> To use [uv](https://docs.astral.sh/uv/), use `uv run` instead of `python` such as:
> 
> ```
> uv run .\mitene_download.py https://mitene.us/f/abcd123456 -v -p the_password -s 2024-11-07
> ```
