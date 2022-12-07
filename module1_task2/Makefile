build : 
	hugo
post : luis
	hugo new posts/$(POST_NAME).md
clean :	## make clean limpiar dist
	rm -rf ./dist/*
luis : 
	echo -e "---\ntitle:\"$(POST_TITLE)\"\ndate: {{ .Date }}\ndraft: true\n---">>./archetypes/posts.md
help : 
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'
cook :
	cook ./kitchen
