# Affordable-Electronoics-Store

<br>
FUNCTIONS:<br>
<b>1. Customer </b>
<br>
•	Customer can view/search products without login.<br>
•	Customer can also add/remove product to cart without login (if customer try to add same product in cart. It will add only one)<br>
•	When customer try to purchase product, then he/she must login to system.<br>
•	After creating account and login to system, he/she can place order.<br>
•	There is a payment page also (just for demo, DONT FILL YOUR CARD DETAILS THERE ,By the way, website do not save that details)<br>
•	If customer click on pay button, then their payment will be successful and their order will be placed.<br>
•	Customer can check their ordered details by clicking on orders button.<br>
•	Customer can see the order status (Pending, Confirmed, Delivered) for each order<br>
•	Customer can Download their order invoice for each order<br>
•	Customer can send feedback to admin (without login)<br>
<br>
<b>2. Admin</b><br>
•	First admin will login ( for username/password run following command in cmd )<br>
•	py manage.py createsuperuser<br>
•	Give username, email, password and your admin account will be created.<br>
•	After login, there is a dashboard (attached in screenshot) where admin can see how many customer is registered, <br>how many products are there for sale, how many orders placed.<br>
•	Admin can add/delete/view/edit the products.<br>
•	Admin can view/edit/delete customer details.<br>
•	Admin can view/delete orders.<br>
•	Admin can change status of order (order is pending, confirmed, out for delivery, delivered)<br>
•	Admin can view the feedbacks sent by customers.<br>
<br>
<b>3. Other Features </b>        <br>
•	customer places order and admin deleted that user(fraud detection), then their orders will automatically deleted<br>
•	suppose 1 customer places 4 products order and admin deleted 2 product from website, <br>then that 2 product order will also be deleted and other 2 will be their<br>
•	If user click on purchase button without having products in their cart, then website will ask to add product in cart first.<br><br>

#HOW TO RUN THIS PROJECT<br>
Install Python(3.7.6) (Dont Forget to Tick Add to Path while installing Python)<br>
Open Terminal and Execute Following Commands :<br>
pip install django==3.0.5<br>
pip install django-widget-tweaks<br>
pip install xhtml2pdf<br>
<br>
#Download This Project Zip Folder and Extract it<br>
Move to project folder in Terminal. Then run following Commands :<br>
py manage.py makemigrations<br>
py manage.py migrate<br>
py manage.py runserver<br><br>

#Now enter following URL in Your Browser Installed On Your Pc<br>
http://127.0.0.1:8000/<br>
<br>

#CHANGES REQUIRED FOR CONTACT US PAGE<br>
In settins.py file, You have to give your email and password:<br>
EMAIL_HOST_USER = 'youremail@gmail.com'<br>
EMAIL_HOST_PASSWORD = 'your email password'<br>
EMAIL_RECEIVING_USER = 'youremail@gmail.com'<br><br>

#Login to gmail through host email id in your browser and open following link and turn it ON<br>
https://myaccount.google.com/lesssecureapps<br>
<br>
<b>Drawbacks/LoopHoles:<b><br>
When user edit their profile then he/she must login again because their username/password is updated in db.<br>
Popup of product is added to cart is shown when click on Ecommerce logo (soon i will fix it)<br>
<br>

