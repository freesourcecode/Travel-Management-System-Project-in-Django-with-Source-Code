# Travel Management System Project in Django with Source Code

The **Travel Management System** is an easy project for beginners to learn how to build a web-based python Django project.

We will provide you with the complete source code and database for the python project so that you can easily install it on your machine and learn how to program in Python Django.

>[!NOTE]
> To start creating a **Travel Management System Project in Python Django**, makes sure that you have PyCharm Professional IDE Installed in your computer.

## Admin Features of Travel Management System in Django

* **Users Management**

For the users, the admin can see the list of users details. Admin can update and delete the record of the users details.

* **Manage Package Details**

For the clients, the admin can see the list of Package details. Admin can update and delete the record of the Package details.

* **Login**

By default the admin need to login first to enable to access the system.

* **Manage Change Password**

For the change password, the admin can change strong password for better security in the system to avoid hacking the important details.

## User Features of Travel Management System in Django

* **Homepage**

For the homepage, The user can see the information about packages in a place and amounts.

* **Manage Signup**

For the signup, The user need to sign first to create an account.

* **Login**

For the login, After creating an an account the user need to login first to access the system.

* **About Us**

For the about us, It is all about mission and vision of travel management system.

* **Booking Tour**

For the booking tour, The user can reserved a place like hotel and resort.

* **Payment**

For the payment, The user need to pay using credit card or online banking.

## How to Create a Project Travel Management System in Django?

Here are the steps on **how to create a Travel Management System in Django**.

1. **Open file**.

First , open “pycharm professional” after that click “file” and click “new project”.

![image](https://github.com/user-attachments/assets/eff3785b-15f4-4ac6-b616-923ef0d153c1)

2. **Choose Django**.

Next, after click “new project“, choose “Django” and click.

![image](https://github.com/user-attachments/assets/55f6a1da-9229-4851-8039-68d8f43d8ecd)

3. **Select file location**.

Then, select a file location wherever you want.

4. **Create application name.**

After that, name your application.

5. **Click create.**

Lastly, finish creating project by clicking “create” button.

![image](https://github.com/user-attachments/assets/60bea079-244b-4613-afbc-2df1109756ae)

6. Start Coding.

Finally, we will now start adding functionality to our Django Framework by adding some functional codes.

## Functionality and Codes of the Travel Management System in Django

* **Create template for the login in form in Travel Management System in Django**.

In this section, we will learn on how create a templates for the login form. 

To start with, add the following code in your login.html under the folder of loginmodule/templates/.

```
<!-- login.html -->

{% extends 'home.html' %}
{% block content %}
<div class="agile-login">
		<div class="wrapper" >
			<h2>Login</h2>
			<div class="w3ls-form">
				<form action="/loginmodule/auth/" method="post">{% csrf_token %}
					<label>Username</label>
					<input type="text" name="username" placeholder="Username" required/>
					<label>Password</label>
					<input type="password" name="password" placeholder="Password" required />
                    <input type="submit" value="Log In" />
				<a href="/SignupApp/signup/" class="pass">Don't have account?SignUp</a>
				</form>
			</div>
            <br><h3 style="color: orangered"> {{ error }}</h3>
        </div>
		<br>
</div>
{% endblock %}
```
* **Create template for the home in Travel Management System in Django**.

In this section, we will learn on how create a templates for the home. 

To start with, add the following code in your home.html under the folder of loginmodule/templates/.

```
{%extends 'dashboard/base.html' %}
{%block content %}
<section id="main-content">
                    <div class="space-30"></div>
                    <div class="container">
                     
                        <div class="row">
                           
                            <div class="col-md-12">
                                <div class="panel">
                                    <header class="panel-heading">
                                        <h2 class="panel-title ">Products</h2><button type="button"
													              class="btn btn-primary pull-right btn-sm js-add-product"
													              data-url="{% url 'dashboard:create_product' %}">
													                <span class="glyphicon glyphicon-pencil"></span> Add Products <span class="fa fa-plus"></span></a>
													        </button>
                                    </header>
                                    <div class="panel-body">
	                                    <div class="table-responsive">
			                                <table class="table table-hover table-striped" id="product-table">
			                                    <thead>
			                                        <tr>
			                                            <th>#</th>
			                                            <th>Name</th>
			                                            <th>Rate</th>
			                                            <th>Tenure</th>
			                                            <th>Frequency</th>
			                                            <th>Guarantor</th>
			                                            <th>Collateral</th>
			                                            <th>Actions</th>
			                                        </tr>
			                                    </thead>
			                                    <tbody>
			                                    {% include 'dashboard/includes/partial_product_list.html' %}
			                                    </tbody>
			                                </table>
                                        </div>
                                    </div>
                                </div>
                                <div class="modal  " id="modal-product">
	                                <div class="modal-dialog">
		                                <div class="modal-content"></div>
	                                </div>
                                </div>
                            </div><!--col end-->
                        </div>
                    </div><!-- end of container-->

                    <!--footer start-->
                    
{% endblock %}
```
### 📌Here's the full documentation for the [Travel Management System Project in Django](https://itsourcecode.com/free-projects/python-projects/travel-management-system-project-in-django-with-source-code/)

