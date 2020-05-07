Role Name db
=========
b/vars/main.yml
generate and change pass 
echo -n '%PUTYOURPASSHERE%' | sha1sum | xxd -r -p | sha1sum | tr '[a-z]' '[A-Z]' | awk '{printf "*%s", $1}'

after deploy remove default nginx conf from sites enabled
