# Change root passowrd

## Set your pattern :
```
# default pattern is "PASSWORD_PATTERN"

sed -i 's/PASSWORD_PATTERN/YOUR_PATTERN/g' change-root-password.yaml
```
```
touch passwd.csv
```
## run ansible: 
```
ansible-playbook -i environments/production/inventory change-root-password.yaml -u YOUR-USERS  -e 'ansible_become=true' -e 'ansible_become_method=sudo'
```


## Outputs are in passwd.csv
```
cat passwd.csv
```

*Tested on Ubuntu/Debian