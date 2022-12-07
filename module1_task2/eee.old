build : 
	hugo
post : joel
	hugo new posts/$(POST_NAME).md
clean : ## make clean limpiar dist
	rm -rf ./dist/* ## clean comment
joel : 
	echo -e "---\ntitle:\"$(POST_TITLE)\"\ndate: {{ .Date }}\ndraft: true\n---">>./archetypes/posts.md
helpp : 
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'
