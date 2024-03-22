# Blog-Doc


# Blog_Platform

### Note:
       - Clear command is **cls**.
### Note:
       - Use **alt + enter** To import.


- 1st crate the python **Blogs** project then,

- in this Blog project Ctreate the **Blog_platform APP**

- Then create the new **blog APP**.

- In **blog APP** >> models.py create **Category, and post** models.

- Then, go in **main Blog_Platform** >> **settings.py** >> add **blog** App in **INSTALLED_APPS**.

- Then, Registered our created models, in **blog >>> admin.py**(By this we see our models in admin site.)

- INSTALLED the **pillow** in terminal.

- Then, Run the **makemigrations** command (it create models).
 
- Then, Run the **migrate** command(it commit the created models.).

## Create Admin pannel.
- Create supersuser(**ADMIN**) by run this command.
   - python manage.py createsuperuser
- To show upload image in correct folder we go in **setting.py** import **os** and declared **MEDIA_URL** AND **MEDIA_ROOT**.

- In **urls.py** also import this 
    - from django.conf.urls.static import static
    - from django.conf import settings
- Then go in main Blog_Platform (app) /**urls.py** (add the  (+static) path in admin.py).

- Then configure the both **Category or Post** in **admin.py**. to Show the table of attribute in admin site.
    - In configuraions we use differrnt fulction like **search_Field**.
- Then we want to show the image with catgory at admin site we do this,
   - make fulction in **models.py** & import which return in newly making image function.
    - By using image tag we displlay the immage at the adminsite.
- WE use the **list_fillter** function in post **admin site.
- Then we use **Rich editor** in**Post app**.
   - Go google >> search **tinymce pypi**.
   - Or use this link **https://pypi.org/project/django-tinymce/**

- Now we change te Admin **Theme**.
- search on goolgle **material admin site django** open 1st link.

- Tinymce code is not work with changing theme so, we use the **js** code for this we create the **static** dirctory in **blog** app then in **static** folder we create ** js** and **css** folder. and write the js code in js directory folder **script.js** and use thisjs code file code in **admin.py >> class media**, at **admin.py** with using the valid **api key** which enabled the text editor at admin site.

   - Api key get from this site (**https://www.tiny.cloud/my-account/integrate/#html**).

### Note:
- if with **material** admin code **tinymce** is not work then we use the **java script version**.

- If you want to change the **color** theme of admin site.
   - GO google search >>> **material admin site django**.
   - Then, copy the **MATERIA_ADMIN_SITE** CODE AND PASTE IN **SETTINGS.PY** at the bottom.

## Start the front site work
- create the **urls.py** file in our created app **blog**. Then, copy the code from main **urls.py** to
**blog/urls.py** with necessory changing or deleting extra code.
- Also add the code in **main urls.py**.
- If user try to excees with (**/ blank**) mean blank then **home** function is run which is created in **Viwes.py**.
- Then import this function in **blog/urls.py**.

## Create template (Html page)
