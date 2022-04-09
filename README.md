line_1 2022-03-29

**/home/sheptukha/git_projects/devops-netology/terraform/.gitignore** рспространяется на папку terraform и будет иметь преимущество перед файлом **/home/sheptukha/git_projects/devops-netology/.gitignore** в случае конфликтов

---

**\*\*/.terraform/\***  

Две звездочки в начале шаблона нужны, чтобы сопоставлять каталоги в любом месте репозитория. Звездочка после означает все файлы и папки в ЛЮБЫХ директориях с указанным именем

---

**\*.tfstate**  
**\*.tfstate.\***  

Игнорирование по типу файла, будут игнорироваться в АБСОЛЮТНО всех директориях Могу предположить, что звездочка после - для того, чтобы игнорировать файлы, например, после ротации логов (имя файла может стать вида **tfstate.2022-03-29**)

---

**crash.log**  
**crash.\*.log**  

Игнорирование конкретного файла crash.log в месте, где расположен файл **.gitignore** Могу предположить, что звездочка после - для того, чтобы игнорировать файлы, например, после ротации логов (имя файла может стать вида **crash.2022-03-29.log**

---

**\*.tfvars**  
**\*.tfvars.json**  

Игнорирование по типу файла, будут игнорироваться в АБСОЛЮТНО всех директориях файлы с расширением **.tfvars** и файлы, которые оканчиваются на **.tfvars.json**

---

**override.tf**  
**override.tf.json**  
**\*_override.tf**  
**\*_override.tf.json**  

Игнорирование конкретного файла **override.tf**, **override.tf.json**, а также файлы оканчивающиеся на **_override.tf** и **_override.tf.json**  в месте, где расположен файл **.gitignore**

---

**.terraformrc**  
**terraform.rc**  

Игнорирование конкретного файла **terraform.rc** и **.terraformrc** в месте, где расположен файл **.gitignore**  
Все что с символом **#** - игрорится  
тест