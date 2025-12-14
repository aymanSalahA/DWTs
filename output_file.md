# Laravel-Livewire Chat-Message-app-scratch  (course notes)

## Chapter 1: Introduction

- first thing creating new projct 
╰─$ composer create-project laravel/laravel live-wire-chat  

╰─$ composer require laravel/breeze --dev 
Question : why --dev ?

after that we need to run this command 
╰─$ php artisan breeze:install 
you will be prompted to select option 
 Which Breeze stack would you like to install? ───────────────┐
 │ › ● Blade with Alpine                                        │
 │   ○ Livewire (Volt Class API) with Alpine                    │
 │   ○ Livewire (Volt Functional API) with Alpine               │
 │   ○ React with Inertia                                       │
 │   ○ Vue with Inertia                                         │
 │   ○ API only    
 TODO : I need to check vold and livewire and those options 
 I will select "blade" option since course is old 
question : breeze : install will install what ? 
TODO : I need to study Pest and unit testing

after that we need to run 
$ npm install

then 
$npm run dev 

This Command of running caused issue since I have node version 18 and it require node version 24 
I used those commands 
# Install n globally (if not yet)
npm install -g n

# Upgrade to latest LTS (currently 20.x or 22.x)
sudo n lts
and it was solved "node was upgraded"
The above commads are for scaffolding proejct 

----------------------------------
next step was configuring and creating new db "sqlite" , but it is default in my proejct 
Now we will create the models 

 Creating models _ migrate
╰─$ php artisan make:model Message -m 
╰─$ php artisan make:model Conversation -m 

We created the migrations and Defined the foregin keys , and put the columns "just in migration files"

and ran this 
$ php artisan migrate

and after that we put the relationships in the models clases 

TODO&question : I will commit but I think in the conversation model the method user is not defined properly 

-=------------------------------
after that we will install livewire 
$ composer require livewire/livewire

## Chapter 2: Install livewire and create some components

- creating some components : 
╰─$ php artisan make:livewire Chat.ChatBox
╰─$ php artisan make:livewire Chat.ChatList
╰─$ php artisan make:livewire Chat.CreateChat
╰─$ php artisan make:livewire Chat.Main  
╰─$ php artisan make:livewire Chat.SendMessage

💡 `--dev` installs Breeze as a development dependency (not needed in production).  
💡 `breeze:install` scaffolds auth views, routes, and controllers based on the selected stack.  
💡 Volt is a Livewire syntax layer for functional-style components (Class vs Functional API).  
💡 Using SQLite is fine for local dev; ensure DB config matches `.env`.  
💡 Check `Conversation::user()` relationship: likely should be `belongsTo(User::class)` with correct foreign key (e.g., `user_id`).  
💡 Livewire components are namespaced under `App\Http\Livewire\Chat\`; confirm directory structure matches.