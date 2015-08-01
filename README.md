Dockerfile for DOCL (Digital Ocean command line)
======================

Lightweight Alpine Linux with docl tool installed.
This image is based on the lightweight [Alpine Linux](https://github.com/gliderlabs/docker-alpine) with the following packages installed:

- curl
- ruby
- ruby-dev
- http://production.cf.rubygems.org/rubygems/rubygems-2.4.8.tgz
- docl

Usage
-----
To build a image based on this dockerfile:

    # git clone git@github.com:joaquindlz/docker-docl.git
    # cd docker-docl
    # docker build -t docl .

To get the builded image, execute the following command:

	# docker pull joaquindlz/docl

Running a new container based on `joaquindlz/docl`
-----------------------------------

Start your container:

	# docker run -ti --name docl -h docl joaquindlz/docl

Test docl:

	/ # docl authorize
	You'll need to enter your DigitalOcean Private Access Token.
	To be able to create / modify droplets, it needs to be read / write.
	You can create a token on the DO website vite the Apps & API menu.
	Enter your DO Token:

Docker Hub repository
--------------------

This image is on [joaquindlz/docl repository on Docker Hub](https://registry.hub.docker.com/u/joaquindlz/docl/)

More information
----------------

**Based on [Alpine Linux](http://www.alpinelinux.org/) and [DOCL Digital Ocean Command Line](https://github.com/nathansamson/docl)**
