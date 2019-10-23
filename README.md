# Asia-Soft-Bot-/

## База данных

![alt text](er_diagram.png)

*Примечание*

#### пользователи users
id - primary_key__
created - datetime обязательно, по умолчанию текущая дата и время__
name - varchar обязательно 256 символов__
phone - varchar обязательно 256 символов__
chat_id - varchar обязательно 256 символов__

#### обращение requests
id - primary_key__
user_id - int обязательно__
created - datetime обязательно, по умолчанию текущая дата и время__
request_type_id - int необязательно__
request_theme_id - int необязательно__
government_department_id - int необязательно__
text - varchar  обязательно 800 символов максимум__
file - varchar необязательно 256 символов__
location - varchar необязательно 256 символов__
status - int обязательно 1 символ__

#### виды обращения request_types
id - primary_key__
created - datetime обязательно, по умолчанию текущая дата и время__
name - varchar обязательно 256 символов__

#### темы обращения request_themes
id - primary_key__
created - datetime обязательно, по умолчанию текущая дата и время__
name - varchar обязательно 256 символов__

#### гос учереждения для рассмотрения government_departments
id - primary_key__
created - datetime обязательно, по умолчанию текущая дата и время__
name - varchar обязательно 256 символов
