### PHP Laravel
> Laravel 8.x (https://laravel.com) \
PHP 7.2+ (https://www.php.net) \
Composer (https://getcomposer.org/) \
PHP/MySQL/Apache/Nginx in BaoTa (https://www.bt.cn/new/index.html)

### 1. Composer help
``` shell
# composer
composer
---
Composer version 2.2.9 2022-03-15 22:13:37

Usage:
  command [options] [arguments]

Options:
  -h, --help                     Display this help message
  -q, --quiet                    Do not output any message
  -V, --version                  Display this application version
      --ansi                     Force ANSI output
      --no-ansi                  Disable ANSI output
  -n, --no-interaction           Do not ask any interactive question
      --profile                  Display timing and memory usage information
      --no-plugins               Whether to disable plugins.
      --no-scripts               Skips the execution of all scripts defined in composer.json file.
  -d, --working-dir=WORKING-DIR  If specified, use the given directory as working directory.
      --no-cache                 Prevent use of the cache
  -v|vv|vvv, --verbose           Increase the verbosity of messages: 1 for normal output, 2 for more verbose output and 3 for debug

Available commands:
  about                Shows a short information about Composer.
  archive              Creates an archive of this composer package.
  browse               Opens the packages repository URL or homepage in your browser.
  cc                   Clears composers internal package cache.
  check-platform-reqs  Check that platform requirements are satisfied.
  clear-cache          Clears composers internal package cache.
  clearcache           Clears composers internal package cache.
  config               Sets config options.
  create-project       Creates new project from a package into given directory.
  depends              Shows which packages cause the given package to be installed.
  diagnose             Diagnoses the system to identify common errors.
  dump-autoload        Dumps the autoloader.
  dumpautoload         Dumps the autoloader.
  exec                 Executes a vendored binary/script.
  fund                 Discover how to help fund the maintenance of your dependencies.
  global               Allows running commands in the global composer dir ($COMPOSER_HOME).
  help                 Displays help for a command
  home                 Opens the packages repository URL or homepage in your browser.
  i                    Installs the project dependencies from the composer.lock file if present, or falls back on the composer.json.
  info                 Shows information about packages.
  init                 Creates a basic composer.json file in current directory.
  install              Installs the project dependencies from the composer.lock file if present, or falls back on the composer.json.
  licenses             Shows information about licenses of dependencies.
  list                 Lists commands
  outdated             Shows a list of installed packages that have updates available, including their latest version.
  prohibits            Shows which packages prevent the given package from being installed.
  reinstall            Uninstalls and reinstalls the given package names
  remove               Removes a package from the require or require-dev.
  require              Adds required packages to your composer.json and installs them.
  run                  Runs the scripts defined in composer.json.
  run-script           Runs the scripts defined in composer.json.
  search               Searches for packages.
  self-update          Updates composer.phar to the latest version.
  selfupdate           Updates composer.phar to the latest version.
  show                 Shows information about packages.
  status               Shows a list of locally modified packages.
  suggests             Shows package suggestions.
  u                    Upgrades your dependencies to the latest version according to composer.json, and updates the composer.lock file.
  update               Upgrades your dependencies to the latest version according to composer.json, and updates the composer.lock file.
  upgrade              Upgrades your dependencies to the latest version according to composer.json, and updates the composer.lock file.
  validate             Validates a composer.json and composer.lock.
  why                  Shows which packages cause the given package to be installed.
  why-not              Shows which packages prevent the given package from being installed.
---

# composer registry
composer config repo.packagist composer https://mirrors.aliyun.com/composer/

# composer update
composer self-update

# composer install with composer.json
composer install
```
### 2. Laravel install/update
```
# Install Laravel
composer create-project laravel/laravel Laravel-Demo

# Update Laravel
composer update laravel/laravel
```

### 3. Laravel run
``` shell
# Run the projcet in the project directory
php artisan serve

# Artisan help
php artisan
---
Laravel Framework 8.83.3

Usage:
  command [options] [arguments]

Options:
  -h, --help            Display help for the given command. When no command is given display help for the list command
  -q, --quiet           Do not output any message
  -V, --version         Display this application version
      --ansi|--no-ansi  Force (or disable --no-ansi) ANSI output
  -n, --no-interaction  Do not ask any interactive question
      --env[=ENV]       The environment the command should run under
  -v|vv|vvv, --verbose  Increase the verbosity of messages: 1 for normal output, 2 for more verbose output and 3 for debug

Available commands:
  clear-compiled        Remove the compiled class file
  completion            Dump the shell completion script
  db                    Start a new database CLI session
  down                  Put the application into maintenance / demo mode
  env                   Display the current framework environment
  help                  Display help for a command
  inspire               Display an inspiring quote
  list                  List commands
  migrate               Run the database migrations
  optimize              Cache the framework bootstrap files
  serve                 Serve the application on the PHP development server
  test                  Run the application tests
  tinker                Interact with your application
  up                    Bring the application out of maintenance mode
 auth
  auth:clear-resets     Flush expired password reset tokens
 cache
  cache:clear           Flush the application cache
  cache:forget          Remove an item from the cache
  cache:table           Create a migration for the cache database table
 config
  config:cache          Create a cache file for faster configuration loading
  config:clear          Remove the configuration cache file
 db
  db:seed               Seed the database with records
  db:wipe               Drop all tables, views, and types
 event
  event:cache           Discover and cache the applications events and listeners
  event:clear           Clear all cached events and listeners
  event:generate        Generate the missing events and listeners based on registration
  event:list            List the applications events and listeners
 key
  key:generate          Set the application key
 make
  make:cast             Create a new custom Eloquent cast class
  make:channel          Create a new channel class
  make:command          Create a new Artisan command
  make:component        Create a new view component class
  make:controller       Create a new controller class
  make:event            Create a new event class
  make:exception        Create a new custom exception class
  make:factory          Create a new model factory
  make:job              Create a new job class
  make:listener         Create a new event listener class
  make:mail             Create a new email class
  make:middleware       Create a new middleware class
  make:migration        Create a new migration file
  make:model            Create a new Eloquent model class
  make:notification     Create a new notification class
  make:observer         Create a new observer class
  make:policy           Create a new policy class
  make:provider         Create a new service provider class
  make:request          Create a new form request class
  make:resource         Create a new resource
  make:rule             Create a new validation rule
  make:seeder           Create a new seeder class
  make:test             Create a new test class
 migrate
  migrate:fresh         Drop all tables and re-run all migrations
  migrate:install       Create the migration repository
  migrate:refresh       Reset and re-run all migrations
  migrate:reset         Rollback all database migrations
  migrate:rollback      Rollback the last database migration
  migrate:status        Show the status of each migration
 model
  model:prune           Prune models that are no longer needed
 notifications
  notifications:table   Create a migration for the notifications table
 optimize
  optimize:clear        Remove the cached bootstrap files
 package
  package:discover      Rebuild the cached package manifest
 queue
  queue:batches-table   Create a migration for the batches database table
  queue:clear           Delete all of the jobs from the specified queue
  queue:failed          List all of the failed queue jobs
  queue:failed-table    Create a migration for the failed queue jobs database table
  queue:flush           Flush all of the failed queue jobs
  queue:forget          Delete a failed queue job
  queue:listen          Listen to a given queue
  queue:monitor         Monitor the size of the specified queues
  queue:prune-batches   Prune stale entries from the batches database
  queue:prune-failed    Prune stale entries from the failed jobs table
  queue:restart         Restart queue worker daemons after their current job
  queue:retry           Retry a failed queue job
  queue:retry-batch     Retry the failed jobs for a batch
  queue:table           Create a migration for the queue jobs database table
  queue:work            Start processing jobs on the queue as a daemon
 route
  route:cache           Create a route cache file for faster route registration
  route:clear           Remove the route cache file
  route:list            List all registered routes
 sail
  sail:install          Install Laravel Sails default Docker Compose file
  sail:publish          Publish the Laravel Sail Docker files
 schedule
  schedule:clear-cache  Delete the cached mutex files created by scheduler
  schedule:list         List the scheduled commands
  schedule:run          Run the scheduled commands
  schedule:test         Run a scheduled command
  schedule:work         Start the schedule worker
 schema
  schema:dump           Dump the given database schema
 session
  session:table         Create a migration for the session database table
 storage
  storage:link          Create the symbolic links configured for the application
 stub
  stub:publish          Publish all stubs that are available for customization
 vendor
  vendor:publish        Publish any publishable assets from vendor packages
 view
  view:cache            Compile all of the applications Blade templates
  view:clear            Clear all compiled view files
---
```