<a name="readme-top"></a>


<!-- TABLE OF CONTENTS -->

# 📗 Table of Contents

- [📗 Table of Contents](#-table-of-contents)
- [📖 Budget app ](#-budget-app-)
  - [🛠 Built With ](#-built-with-)
    - [Tech Stack ](#tech-stack-)
    - [Key Features ](#key-features-)
  - [🚀 Live Demo ](#-live-demo-)
  - [💻 Getting Started ](#-getting-started-)
    - [Prerequisites](#prerequisites)
    - [Setup](#setup)
    - [Install](#install)
    - [Usage](#usage)
    - [Run tests](#run-tests)
    - [Deployment](#deployment)
  - [👥 Authors ](#-authors-)
  - [🔭 Future Features ](#-future-features-)
  - [🤝 Contributing ](#-contributing-)
  - [⭐️ Show your support ](#️-show-your-support-)
  - [🙏 Acknowledgments ](#-acknowledgments-)
  - [❓ FAQ (OPTIONAL) ](#-faq-optional-)
  - [📝 License ](#-license-)

<!-- PROJECT DESCRIPTION -->

# 📖 Budget app <a name="about-project"></a>

>  This is a project that is going to work as a Budget app with the necessary characteristics to make it interactive.


## 🛠 Built With <a name="built-with"></a>

### Tech Stack <a name="tech-stack"></a>

<details>
  <summary>Client</summary>
  <ul>
    <li><a href="https://code.visualstudio.com/">Viual Studio Code</a></li>
  </ul>
</details>

<details>
  <summary>Server</summary>
  <ul>
    <li><a href="https://rubyonrails.org/">Ruby</a></li>
  </ul>
</details>

<details>
<summary>Database</summary>
  <ul>
    <li><a href="https://www.postgresql.org/">PostgreSQL</a></li>
  </ul>
</details>

<!-- Features -->

### Key Features <a name="key-features"></a>

> The next key features are availble in this project.

- Register yourself as a new user.
- Update you password.
- Create categories.
- Create transactions. 
- Execute model tests.

  
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LIVE DEMO -->

## 🚀 Live Demo <a name="live-demo"></a>

> You can see the deployment once it is executed in the next link.

- [Render Live View](https://budget-app-v1.onrender.com/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->

## 💻 Getting Started <a name="getting-started"></a>

> To get a local copy up and running, follow these steps.

### Prerequisites

In order to run this project you need:

> Install a text-editor you prefer. [Code editors](https://desarrolloweb.com/colecciones/editores-codigo).

> You need a database
- [SQLlite](https://www.sqlite.org/index.html)
- [MySQL](https://www.mysql.com/)
- [Postgresql](https://www.postgresql.org/)

> [Ruby](https://www.ruby-lang.org/en/downloads/)


> [Ruby on Rails Framework](https://rubyonrails.org/)

### Setup

Clone this repository to your desired folder:

> You must have an account on git hub. [Git Hub](https://github.com/)

> You must have installed git in your local environment. [Git](https://git-scm.com/download/win)

> If you just want to take a look quickly, make a fork and open the project in the web browser by adding ".dev" instead of ."com" in the repo link.
- Example : https://github.dev/J2ZROMERO/Budget_app

### Install

Install this project with:

Execute the bundle in your terminal with the path of 
the directory.

> Execute "rails bundle" in your terminal with the specific path in order to add all the gems.

> You have to change the data bases' crentials.

> When the project si already installed execute:
 - rake db:setup or rails db:setup
    - Once this in being executed the nexts actions are generated 
    - rake db:create
    - rake db:schema:load
    - rake db:seed

> If you already have  the project in your local you can pull the lastes commit and execute the next commands:
  - rails db:reset
  - rails db:migrate:reset
  - rails db:seed

### Usage

To run the project, execute the following command:

- Once your credential is ready execute
> Ruby bin/rails db:setup

- After db:setup is executed the file seed.rb is going to execute immediately this will add prepared data to your database, and you can test the customized methods from models.

- After that execute:
> Ruby bin/rails db:migrate

- This command will ensure to load the models to tests it.

- You must be sign in to execute de create comment.
  
- shows all the caetgories
  http://localhost:3000/groups/

- shows all the post by the given user
  http://localhost:3000/api/user/1

- Create new category.
  http://localhost:3000/groups/new

- See the transactions list.
  http://localhost:3000/groups/32/budgets

- Create transactions
  http://localhost:3000/groups/32/budgets/new

  

### Run tests

- To run the tests please follow the next instruccions.
> The gem database_cleaner let us clean all the database before execute the test (:warning This gem only works for test and don't allow any input to the original data base), to use this gem is necesary to add some characteristics to the rails_helper.rb
- Add the next gem : gem 'database_cleaner' to the Gemfile
- Execute: bundle install.
- Ruby bin/rails db:migrate RAILS_ENV=test 
  - The code above will ensure to prepare the modules for tests.
- Execute: [ rspec ] if you wan to see all the tests working.
- or execute rspec spec/models/NAME-OF-THE-MODEL_spec.rb  if you want to run a especific file.
- If you want to see the tests existing and their definitions please run: " rspec --force-color --format documentation "
- To check the tests's controllers please execute the next command on your root project console: "" rspec spec/requests/ ""  you will see all the tests' controllers in execution.
- In order to see Capybara tests you can execute:
  " rspec spec/models" all the tests.
  " rspec spec/models/budget_spec.rb " single file.
### Deployment

You can deploy this project using:

- The databa.yml file is configured to be deployed with render, if you want to deploy it locally please.
  - Change your credentials.
  - default: &default
  - adapter: postgresql
  - encoding: unicode
  - username: postgres
  - password: 153624
  
- And comment the line 28 in config/puma.rb
- # workers ENV.fetch("WEB_CONCURRENCY") { 4 }
  
> Ruby bin/rails server
- hen Go to your browser in the next directions to interact with the app.
 
> http://localhost:3000/ 

> Then if you want to deploy it again in render undo changes you did.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- AUTHORS -->
## 👥 Authors <a name="authors"></a>

👤 **JOSE ZEPEDA**

- GitHub: [J2ZROMERO](https://github.com/J2ZROMERO)
- Twitter: [@JOSEZEPED4](https://twitter.com/JOSEZEPED4)
- LinkedIn: [JOSE ZEPEDA](https://www.linkedin.com/in/jose-zepeda-733ab91ab/)
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- FUTURE FEATURES -->

## 🔭 Future Features <a name="future-features"></a>

> The next features will be added.

- [ ] Tests.
- [ ] React-Redux.
- [ ] Fetch data to implement it on the interfaz to make it interactive.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->

## 🤝 Contributing <a name="contributing"></a>

Contributions, issues, and feature requests are welcome!

Feel free to check the [issues page](https://github.com/J2ZROMERO/Budget_app/issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- SUPPORT -->

## ⭐️ Show your support <a name="support"></a>

> Feel free to share your inquiries to our social links provided and we will help you. Don't forget to gift us a ⭐️



<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- ACKNOWLEDGEMENTS -->

## 🙏 Acknowledgments <a name="acknowledgements"></a>

I would like to thanks [Gregorie Vella](https://www.behance.net/gregoirevella) to create the beautiful design and make it public.

I would like to thank MICROVERSE for preparing the content to work.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- FAQ (optional) -->

## ❓ FAQ (OPTIONAL) <a name="faq"></a>

- **It can works with another data base**

  - Of couser the idea of use postgresql is because it is a powerfull db that is well suited with rails.

- **Linters are necessary**

  - If you want to have a redable and clean code it is a good option to choose

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- LICENSE -->

## 📝 License <a name="license"></a>

This project is [MIT](https://github.com/J2ZROMERO/Budget_app/blob/dev/MIT.md) licensed.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

