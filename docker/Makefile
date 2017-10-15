IMG="bamboofox-blog-jekyll-img"
CTN="bamboofox-blog-jekyll"

all: build run

build:
	docker build --rm -t bruce30262/$(IMG) .
run:
	docker run -e TERM --privileged --security-opt seccomp:unconfined -p 4000:4000 --name=$(CTN) -it bruce30262/$(IMG) /bin/bash -c 'cd ~/bamboofox.github.io && bundle exec jekyll serve --host 0.0.0.0'
exec:
	docker exec -it $(CTN) /bin/bash -c 'cd ~/bamboofox.github.io && /bin/bash'
