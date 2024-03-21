# Blog-Doc

# Blog_Platform
- 1st crate the python **Blogs** project then,

- in this Blog project Ctreate the **Blog_platform APP**

- Then create the new **blog APP**.

- In **blog APP** >> models.py create **Category, and post** models.

- Then, go in **main Blog_Platform** >> **settings.py** >> add **blog** App in **INSTALLED_APPS**.

- Then, Registered our created models, in **blog >>> admin.py**(By this we see our models in admin site.)

- INSTALLED the **pillow** in terminal.

  ### Note:
       - Clear command is **cls**.

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
   - make fulction in **models.py** & import which return in newly making function.
