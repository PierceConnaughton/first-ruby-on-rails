# README

This is my first ruby on rails application

<h2>Ruby On Rails components</h2>
Quick Explanation on how some of Ruby On Rails works
Ruby On Rails follows the MVC (Model-View-Controller) pattern.
Controllers are Ruby classes, and their public methods are actions.
Views are templates, usually written in a mixture of HTML and Ruby.
A model is a Ruby class that is used to represent data.
Migrations are used to alter the structure of an application's database.
Concerns are a way to make large controllers or models easier to understand and manage.
http_basic_authenticate_with method, which allows access to the requested action if that method allows it.

<h2>ERB</h2>
ERB is a templating system that evaluates Ruby code embedded in a document.
in an .ERB File
Here, we can see two types of ERB tags: <% %> and <%= %>. 
The <% %> tag means "evaluate the enclosed Ruby code." 
The <%= %> tag means "evaluate the enclosed Ruby code, and output the value it returns."

The code below displays an item for each item in the title
  <% @table.each do |item| %>
    
      <%= item %>
    
  <% end %>

<h2>Route Parameters</h2>
A route parameter captures a segment of the request's path, and puts that value into the params Hash, which is accessible by the controller action.
For example, when handling a request like GET http://localhost:3000/articles/1, 1 would be captured as the value for :id, which would then be accessible as params[:id] in the show action of ArticlesController.

Rails provides a routes method named resources that maps all of the conventional routes for a collection of resources
for example in the routes.rb in articales we can input resources :articles and this will create routes for get post patch and delete

<h2>Form Builder</h2>
Ruby uses a feature form builder to easily create forms.
Using a form builder, we can write a minimal amount of code to output a form that is fully configured and follows Rails conventions.

Rails provides a feature called validations to help us deal with invalid user input. Validations are rules that are checked before a model object is saved. 
If any of the checks fail, the save will be aborted, and appropriate error messages will be added to the errors attribute of the model object.

The full_messages_for method returns an array of user-friendly error messages for a specified attribute. If there are no errors for that attribute, the array will be empty.

<h2>Associating Models</h2>
Active Record associations let you easily declare the relationship between two models. 
In the model files we can declare has_many and belongs_to to define relationships between models.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
