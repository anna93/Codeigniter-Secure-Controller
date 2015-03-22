Codeigniter-Secure-Controller
=============================

In the Codeigniter PHP framework, the single entry point for any web page/method is a controller.

Controllers serve everything.
By default, Codeigniter has one base controller class named 'CI_Controller' located at system/core/controller.php which 
does not check for authentication(whether the user is logged in or not). Since, every userdefined controller needs to extend 
the base controller, it makes more sense to extend one intermediate controller which checks for the authentication 
info in its constructor itself! This project defines that Intermediate controller.

Here is the code, which extends the base class 'CI_Controller', which of course is an insecure controller. However if 
authentication check is required then extend the 'Secure_Controller'.

Note:
The Secure_Controller uses a session variable named 'logged_in' to check for the availability of a session, you can modify the code
accordingly.

Replace your controller.php with this file in system/core/ .

Happy coding!!!
