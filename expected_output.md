# Laravel-Livewire Chat-Message-App-Scratch (Course Notes)

## Chapter 1: Introduction

### Project Setup

First thing: creating new project

```bash
$ composer create-project laravel/laravel live-wire-chat
```

```bash
$ composer require laravel/breeze --dev
```

**Q:** Why `--dev`?

After that we need to run this command:

```bash
$ php artisan breeze:install
```

You will be prompted to select option:

```
Which Breeze stack would you like to install? ───────────────┐
│ › ● Blade with Alpine                                        │
│   ○ Livewire (Volt Class API) with Alpine                    │
│   ○ Livewire (Volt Functional API) with Alpine               │
│   ○ React with Inertia                                       │
│   ○ Vue with Inertia                                         │
│   ○ API only
```

-   [ ] TODO: Check Volt and Livewire and those options

I will select "Blade" option since course is old.

**Q:** `breeze:install` will install what?

-   [ ] TODO: Study Pest and unit testing

After that we need to run:

```bash
$ npm install
```

Then:

```bash
$ npm run dev
```

**Issue:** This command of running caused issue since I have Node version 18 and it requires Node version 24.

I used those commands:

```bash
# Install n globally (if not yet)
npm install -g n

# Upgrade to latest LTS (currently 20.x or 22.x)
sudo n lts
```

And it was solved "Node was upgraded".

The above commands are for scaffolding project.

---

### Database Configuration

Next step was configuring and creating new DB "SQLite", but it is default in my project.

Now we will create the models.

### Creating Models & Migrations

```bash
$ php artisan make:model Message -m
$ php artisan make:model Conversation -m
```

We created the migrations and defined the foreign keys, and put the columns "just in migration files".

And ran this:

```bash
$ php artisan migrate
```

And after that we put the relationships in the models classes.

-   [ ] TODO & Question: I will commit but I think in the Conversation model the method `user` is not defined properly

---

### Installing Livewire

After that we will install Livewire:

```bash
$ composer require livewire/livewire
```

## Chapter 2: Install Livewire and Create Some Components

Creating some components:

```bash
$ php artisan make:livewire Chat.ChatBox
$ php artisan make:livewire Chat.ChatList
$ php artisan make:livewire Chat.CreateChat
$ php artisan make:livewire Chat.Main
$ php artisan make:livewire Chat.SendMessage
```

💡 `--dev` installs Breeze as a development dependency (not needed in production).  
💡 `breeze:install` scaffolds auth views, routes, and controllers based on the selected stack.  
💡 Volt is a Livewire syntax layer for functional-style components (Class vs Functional API).  
💡 Using SQLite is fine for local dev; ensure DB config matches `.env`.  
💡 Check `Conversation::user()` relationship: likely should be `belongsTo(User::class)` with correct foreign key (e.g., `user_id`).  
💡 Livewire components are namespaced under `App\Http\Livewire\Chat\`; confirm directory structure matches.
