# django_rest_framework_cart

-->How to run the project on your computer




Requirements: 
               
              Django

              Djongo (for mongodb)
              
              
              Djangorestframework
              
              
              MongoDb
              
1.Clone the repository


2.pip install all the requirements


3.Download MongoDb


4.for fresh start type the following codes on terminal >> 


                                                           rm -f db.sqlite3



                                                          rm -r shop/migrations
                                                          
                                                          
                                                          
5. Setup MongoDb: 


a) Create a database on mongodb




b) Go to settings.py in your django project and change Database configurations:







DATABASES =  


{

    'default': {
        'ENGINE': 'djongo',
        'NAME': '<write_your database name>',

    }
    
}



  c) python manage.py makemigrations shop
  
  d) python manage.py migrate
  
  e)create user: python manage.py createsuperuser
  
 f) runserver: python manage.py runserver
 
 
 Instructions: 1. This is a CRUD Rest Api Project
 
 
 
 
 -> Login user credentials :http://127.0.0.1:8000/
 
 
 ->add new user: http://127.0.0.1:8000/users/       (json PUT from django rest framework)
 
 
 -> Add products: http://127.0.0.1:8000/products/ (json PUT from django rest framework)
 
 
 ->add cart: /carts/<card_id>/add_to_cart/
 
 
 
 --> remove cart: /carts/<card_id>/remove_from_cart/ 
 
 
 
 
