FRN#0028794543 
FCC 
# Step 1: Authenticate
$ cat ~/GH_TOKEN.txt | docker login docker.pkg.github.com -u dimetrymortimerdominicus --password-stdin
# Step 2: Tag
$ docker tag IMAGE_ID docker.pkg.github.com/dimetrymortimerdominicus/dander/IMAGE_NAME:VERSION
# Step 3: Publish
$ docker push docker.pkg.github.com/dimetrymortimerdominicus/dander/IMAGE_NAME:VERSION
