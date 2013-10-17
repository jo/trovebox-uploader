Upload to Trovebox
==================

Find all images in given directories (or, of not provided, in current path),
check if they need to be uploaded by comparing sha1 sums from server list
and upload each image while displaying a nice progress bar.

## Installation

I am just a tiny little Ruby script.

Clone this project

    git clone https://github.com/jo/trovebox-uploader.git

and install the required gems with `bundler`

    bundle install

or manually via `gem`

    gem install openphoto-ruby ruby-progressbar

## Configuration

Place a trovebox config file in `~/.config/trovebox/default`:

    host = https://username.trovebox.com
    consumerKey = blabla
    consumerSecret = secure
    token = bliblu
    tokenSecret = secret

## Usage

    ./upload folder1 folder2 image.jpg

This will upload all JPG images in `folder1` and `folder2`, as well as `mage.jpg`

To upload the current folder, just run

    path-to-trovebox-uploader/upload

## License

Copyright (c) 2013 Johannes J. Schmidt
Licensed under the MIT license.
