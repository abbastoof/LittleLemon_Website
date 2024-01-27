## **Introduction**

### **Project Summary**

The project, named **littlelemon**, aims to create the Little Lemon website with five pages: Home, About, Booking, Menu, and Menu Item. The primary objectives include implementing a Menu page and a Menu Item page. The modifications involve altering various files such as **settings.py**, **urls.py**, **models.py**, **views.py**, **admin.py**, and HTML templates.

## **Run the Project**

1. Open a terminal in the project directory.
2. Create a superuser for Django admin:

    ```bash
    python manage.py createsuperuser
    ```

   Follow the prompts to set up the superuser credentials.

3. Run migrations:

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

4. Start the development server:

    ```bash
    python manage.py runserver
    ```

5. Open a web browser and go to [http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin) to log in with the superuser credentials. Add menu items through the Django admin panel.

6. Access the homepage at [http://127.0.0.1:8000](http://127.0.0.1:8000) and navigate to the Menu page.

7. Click on menu items to verify their details on the Menu Item page.

## **Summary of Changes**

- **Menu Page:**
  - Created a `Menu` model in **models.py** with attributes `name` and `price`.
  - Registered the `Menu` model in **admin.py**.
  - Configured URL paths in **urls.py**.
  - Developed a view function in **views.py** to display menu items.
  - Created the **menu.html** template to present menu items.

- **Menu Item Page:**
  - Updated the `Menu` model in **models.py** with an additional attribute `menu_item_description`.
  - Extended the URL paths in **urls.py** for menu items.
  - Developed a view function in **views.py** to display menu item details.
  - Created the **menu_item.html** template to present menu item details.

- **Footer:**
  - Designed the **_footer.html** template with a copyright notice and Little Lemon logo.

The project successfully achieves the goals of creating a functional website with dynamic content for menus and menu items.
