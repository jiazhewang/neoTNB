.PHONY : deploy
deploy :
	git checkout source
	jekyll build
	git add -A
	git commit -m "update source"
	mkdir /tmp
	cp -r _site/ /tmp/
	git checkout gh-pages
	rm -r ./*
	cp -r /tmp/_site/* ./
	git add -A
	git commit -m "deploy blog"
	git push origin gh-pages
	git checkout source
	echo "deploy succeed"
	git push origin source
	echo "push source"
