# Milestone Project 4

## Contents
* [Purpose](#Purpose)
* [UX](#UX)
* [Technologies](#Technologies)
* [Testing](#Testing)
* [Supported Browsers And Devices](#Supported-Browsers-And-Devices)
* [Deployment](#Deployment)
* [Credits](#Credits)
<br>

## Purpose

The purpose of this project is to showcase everything I have learned within the Full Stack Frameworks With Django modules of the Code Institute Full Stack Development course. A full list of technologies used can be found in the technologies section of this document.
<br>
<br>
Pacific Plants is an e-commerce site that sells both indoor and outdoor plants. 
<br>
<br>
DISCLAIMER: This website is for educational purposes only and uses products and content from an existing brand. Please see the credits section for full information.
<br>
<br>
Please see below for the link to the website.

https://pacificplants.herokuapp.com/
<br>
<br>

## UX

### User Stories
As a casual user I want to:

* Easily navigate the site.
* Search the site.
* View all products available.
* Filter the products by using categories.
* Filter the products by price.
* View individual product details.
* Select quantity of a product.
* View items in shopping bag and the total cost.
* Adjust quantity of product if needed.
* Remove a product from the shopping cart. 
* Receive confirmation when an action has been performed.
* Easily enter payment information and checkout.
<br>

As a registered user I want to:

* Save my profile information for the next purchase
* Edit my profile information.
* Check my previous purchases.  
<br>

As an admin user I want to:

* Add a new product.
* Edit an existing product.
* Delete an existing product.

### Design

#### Colour Scheme
White - Navigation bar, background and button text.
<br>
Off White - Background colour.
<br>
Black - Navigation bar text.
<br>
Charcoal - Header and body text. Button hover effect.
<br>
Green - Buttons, icons and links.
<br>
#### Typography
Roboto - This font will be used throughout the whole webpage, this is because it looks clean, professional and is easy to read.
<br>
#### Wireframes
To see the wireframes for all pages on both desktop and mobile view please click the below link.
<br>
[Wireframes](wireframes/wireframes.pdf)
<br>
#### Features
* Navigation Bar - Remains at the top of the page so it is always accessible. It categorizes the products and is collapsible on mobile devices.
* Search Bar - Allows the user to search a product by name or category.
* Toasts - Provides feedback to the user by displaying a message in the top right of the screen.
* Sorting - Products can be sorted by price, rating, name and category.
* Shopping Bag - Users can add, update and remove products from the shopping bag.
* Checkout - Users can fill in their information into a form to purchase a product. This information can be saved to their profile page.
* User Profile - Users can register and login to the site. The user profile displays order history and their information if they chose to save it.
* Admin User - An admin user has permissions to add, edit and delete products.

## Technologies

### Languages Used

- HTML
- CSS
- JavaScript
- Python

### Frameworks, Libraries & Programs Used

**Front-End**
* Bootstrap
* Font-Awesome
* Google Fonts
* jQuery
* Balsamiq

**Back-end**
* Django
* Stripe

**Deployment**
* Heroku
* AWS
* Github
* Gitpod

## Testing

Test card details:
* **Card Number:** 4242 4242 4242 4242
* **Expiration Date, CVC, ZIP:** Any integer.
<br>

### Code Validation

* HTML files have been validated using the W3C HTML Validation Service website.
* CSS file has been validated using the W3C CSS Validation Service website.
* JS file has been validated using the JSHint website.
* Python file has been validated using the pylint.
<br>

### User Story Testing

**User Story** – Easily navigate the site & search the site.
<br>
* Every page has a sticky navigation bar which allows the user to easily access any page they want at all times.
* The navigation bar contains a search bar which allows the user to search for a product by name or category.
<br>

**User Story** – View all products available and filter/sort products.
<br>
* The navigation bar gives the user the option to view all products, filter them by category and sort by price, rating and category.
* The user can also sort the products when on the products page.
<br>

**User Story** – View individual product details and select quantity of a product.
<br>
* When a user clicks on a product it will display more information about the selected product. If the image is clicked on it will enlarge the image in a new tab.
* From this page the user can select the desired quantity and add the item to the shopping bag.
<br>

**User Story** – View items in shopping bag and the total cost. Also the option to amend the bag if needed.
<br>
* Users can view items added and total cost by navigating to the shopping bag page. This information will also be displayed in the top right of the page when a new item has been added to the bag.
* From the shopping bag page a user can edit the quantity of an item as well as delete an item.
<br>

**User Story** – Receive confirmation when an action has been performed.
<br>
* Users will receive a notification in the top right of the screen when an important action has been performed.
<br>

**User Story** – Easily enter payment information and checkout.
<br>
* When the user is ready to checkout they will need to simply enter their personal information into a form to complete the purchase.
<br>

**User Story** – Save/edit profile information for next purchase and check previous purchases.
<br>
* A registered user can access their profile page which will display their saved information as well as their order history. From this page they can also edit their information.
<br>

**User Story** – Add, edit and delete a product.
<br>
* An admin user can access the product management page which will allow them to add a new product.
* An admin user can also find an existing product and edit/delete it.
<br>

## Supported Browsers And Devices

Below is all the browsers and devices the website has been tested on.
<br>
<br>
**Google Chrome (Right clicked the page and selected Inspect then Toggle Device Toolbar)**
<br>
**Microsoft Edge (Right clicked the page and selected Inspect then Toggle Device Emulation)**
* Moto G4
* Galaxy S5
* Pixel 2
* Pixel 2 XL
* iPhone 5/SE
* iPhone 6/7/8
* iPhone 6/7/8 Plus
* iPhone X
* iPad
* iPad Pro
* Surface Duo
* Galaxy Fold
<br>

**Firefox (Right clicked the page and selected Inspect Element then Responsive Design Mode)**
* Galaxy S9/S9+
* iPad
* iPhone 6/7/8
* iPhone 6/7/8 Plus
* iPhone X/XS
* Kindle Fire HDX
<br>

## Deployment

This project was developed on Github, using Gitpod as IDE. It was deployed on Heroku.

### Requirements

You will need the following in your IDE environment:

1. Git
1. Python3
1. pip3

You will need accounts for the following services:

1. [Gmail](https://gmail.com)
1. [Stripe](https://stripe.com/en-gb)
1. [AWS S3](https://aws.amazon.com/)
1. [Heroku](https://www.heroku.com)

### Local Deployment

**Clone this repository:**

1. Go to the project [repo](https://github.com/sanjaysanghera/Milestone-Project-4)
2. Click the "code" button and copy the HTTPS link
3. Open Git terminal and type ```git clone``` followed by the link and hit "enter".

**Set up environment variables:**

1. Create an ```env.py``` file
2. Ensure that ```env.py``` is in your ```.gitignore``` file in the root directory
3. Add the following variables to your ```env.py``` file:
    ```
        os.environ["DEVELOPMENT"] = "True"
        os.environ["SECRET_KEY"] = "<Insert here>"
        os.environ["STRIPE_PUBLIC_KEY"] = "<Insert here>"
        os.environ["STRIPE_SECRET_KEY"] = "<Insert here>"
        os.environ["STRIPE_WH_SECRET"] = "<Insert here>"
    ```

**Add all module requirements to ```requirements.txt``` file:**

1. Run the following in the command line: ```pip3 install -r requirements.txt```

**Database setup**

Use the following commands to load the fixtures data (in this order):

1. ```python3 manage.py loaddata categories```
2. ```python3 manage.py loaddata products```

**Create admin user**

Use the following commands to create a superuser:

1. ```python3 manage.py createsuperuser```
2. Enter an e-mail, username and password for the superuser

**Run the application**

Run the following in the command line

1. ```python3 manage.py runserver```

### Deploy to Heroku

**Set up heroku account**

1. Create a new app
    - Click on "New" > "Create new app"
    - Enter a name
    - Select the region closest to you

**Set up AWS account**

1. Sign in as "Root User" 
2. Search for "S3" at the top of the site and click it to open
3. Click on "Create bucket"
    - Fill in the name (this should match your Heroku app name)
    - Set the region closest to you
    - Deselect "Block all public access"
    - Click "Create Bucket"
4. Enable static website hosting in the properties tab
    - Select "Use this bucket to host a website"
    - For Index Document, input "index.html"
    - For Error Document, input "index.html"
    - Click "save"
5. Go to the permission tab
    - In "CORS configuration", paste the following to set up the required access between the Heroku app and this S3 bucket:
        ```
        [
            {
                "AllowedHeaders": [
                    "Authorization"
                ],
                "AllowedMethods": [
                    "GET"
                ],
                "AllowedOrigins": [
                    "*"
                ],
                "ExposeHeaders": []
            }
        ]
        ```
    - In "Bucket Policy", select policy generator
        - Select "Type of Policy" should be "S3 Bucket Policy"
        - Type ```*``` in the "Principal" field
        - Select "get object" from the "Actions" dropdown
        - Input your ARN from the previous tab into the "ARN" field
        - Click "Add statement"
        - Click "Generate Policy" and copy
        - Paste policy into the bucket policy editor back on the "Bucket Policy" tab, adding ```/*``` onto the end of the resource key
        - Click save
    - Setting up IAM
        - Go back to the services menu at the top of the screen, and open IAM
        - Click on "User Groups" in the site bar and create a new group by inputting a group name
        - Check "Next Step" and then "Create Group"
        - Click on "Policies" in the side bar in then "Create policy"
        - Select the "JSON" tab, and "Import managed policy"
        - In the search bar, search for "s3" and then import the "s3 full access policy"
        - We only want full access to our Bucket, go back to copy your ARNs from before and add it within the resource brackets
          ```
            {
              "Version": "2012-10-17",
              "Statement": [
                  {
                      "Effect": "Allow",
                      "Action": "s3:*",
                      "Resource": [
                          "[INSERT ARN HERE]",
                          "[INSERT ARN HERE]/*"
                      ]
                  }
              ]
            }
            ```
        - Click "Review Policy"
        - Add a Name and Description
        - Click "Create policy"
        - Go back to "Groups" in the sidebar, and click your new group
        - Click "Attach policy"
        - Search for the policy you just created and select it
        - Click "Attach Policy"
        - Go to "Users" in the sidebar, and click "Add User"
        - Create a user named reponame-staticfiles-user, and select "programmatic access"
        - Click "Next", and select the group to add the user to
        - Click through to the end and "Create User"
        - Download the CSV file - This contains your AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY variables.

**Set up gmail**

1. Go to [Gmail](http://www.gmail.com)
2. Either log in if you already have an account, or sign up
3. Go the account settings in the upper right, and click "accounts and import" and then "other google account settings"
4. Go to the security tab and under "signing into google" turn on "2-step verification"
5. Click "Get started", enter your password and have them send you a verification code
6. Once you are verified, turn on two step verification
7. Go back to the security tab, and you should see a heading called "App Passwords", click that and enter password again if needed
8. Under the "Select app" dropdown, select "Mail"
9. Under the "Select app" dropdown, select other and type "Django"
10. Save the "Generated App Password" as this will be used as your EMAIL_HOST_PASS config variable in Heroku

**Deployment**

1. Set up Postgres in Heroku
    - Go to the resources tab in Heroku
    - Search for "Heroku Postgres"
    - Select the "Hobby Dev" free plan
2. Comment out the 'SQLite and Postgres databases' section in your ```settings.py``` file 
    and uncomment 'Postgres Database' section. Add your DATABASE_URL link obtained from Heroku Config Vars
    ```
     DATABASES = {
     'default': dj_database_url.parse('your-url-goes-here')
    }
    ```
3. Migrate your models to Postgres by inputting this in your command line:
    ```python3 manage.py migrate```
4. Import your fixtures to the new database inputting this in your command line:
    ```
    python3 manage.py loaddata categories
    python3 manage.py loaddata products
    ```
5. Create a new superuser account inputting this in your command line and then adding an email and password:
    ```
    python3 manage.py createsuperuser
    ```
6. Install unicorn, which will act as our webserver
    - ```pip3 install gunicorn```
7. Freeze requirements file
    - ```pip3 > freeze requirements.txt```
8. Create a Procfile in the root directory
    - Add ```web: gunicorn <YOUR APP NAME>.wsgi:application```
9. Set up config variables in Heroku
    - Go to your app "Settings", and click "Reveal config vars"
    - Add the following:
        | Key                    | Value                                |
        |------------------------|--------------------------------------|
        | AWS_ACCESS_KEY_ID      | < Insert from the aws csv >          |
        | AWS_SECRET_ACCESS_KEY  | < Insert from the aws csv>           |
        | DATABASE_URL           | < Insert the postgres url >          |
        | EMAIL_HOST_PASS        | < Insert the gmail password >        |
        | EMAIL_HOST_USER        | < Insert your email address>         |
        | SECRET_KEY             | < Insert secret key >                |
        | STRIPE_PUBLIC_KEY      | < Insert stripe public key >         |
        | STRIPE_SECRET_KEY      | < Insert stripe secret key >         |
        | STRIPE_WH_SECRET       | < Insert stripe webhook secret>      |
        | USE_AWS                | True                                 |

10. Go to the app "Deploy" tab and click on the "Github" option
11. Connect your Github account and input your Github repo name
12. Click on "Enable Automatic Deploys" and then "Deploy Branch"
13. You can view your deployed site by clicking on "Open App"


## Credits

### Content
- [Patch Plants](https://www.patchplants.com/gb/en/) - Product details and images have been taken from Patch Plants. 

### Code
- [Code Institute](https://www.codeinstitute.net/) - Code learnt from the Full Stack Web Developer course has been implemented in this project.




  
