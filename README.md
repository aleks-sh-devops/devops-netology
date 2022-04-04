line_1 2022-03-29



#Данный /home/sheptukha/git_projects/devops-netology/terraform/.gitignore рспространяется на папку terraform


# Local .terraform directories
**/.terraform/*
#Две звездочки в начале шаблона нужны, чтобы сопоставлять каталоги в любом месте репозитория. Звездочка после означает все файлы и папки в ЛЮБЫХ директориях с указанным именем


# .tfstate files
*.tfstate
*.tfstate.*
#Игнорирование по типу файла, будут игнорироваться в АБСОЛЮТНО всех директориях Могу предположить, что звездочка после - для того, чтобы игнорировать файлы, например, после ротации логов (имя файла может стать вида tfstate.2022-03-29)


# Crash log files
crash.log
crash.*.log
#Игнорирование конкретного файла crash.log в месте, где расположен файл .gitignore Могу предположить, что звездочка после - для того, чтобы игнорировать файлы, например, после ротации логов (имя файла может стать вида crash.2022-03-29.log)

# Exclude all .tfvars files, which are likely to contain sensitive data, such as
# password, private keys, and other secrets. These should not be part of version 
# control as they are data points which are potentially sensitive and subject 
# to change depending on the environment.
*.tfvars
*.tfvars.json
#Игнорирование по типу файла, будут игнорироваться в АБСОЛЮТНО всех директориях файлы с расширением .tfvars и файлы, которые оканчиваются на .tfvars.json

# Ignore override files as they are usually used to override resources locally and so
# are not checked in
override.tf
override.tf.json
*_override.tf
*_override.tf.json
#Игнорирование конкретного файла override.tf override.tf.json, а также файлы оканчивающиеся на _override.tf и _override.tf.json  в месте, где расположен файл .gitignore

# Include override files you do wish to add to version control using negated pattern
# !example_override.tf

# Include tfplan files to ignore the plan output of command: terraform plan -out=tfplan
# example: *tfplan*

# Ignore CLI configuration files
.terraformrc
terraform.rc
#Игнорирование конкретного файла terraform.rc и .terraformrc в месте, где расположен файл .gitignore

Все что с символом # - игрорится
новая строчка
