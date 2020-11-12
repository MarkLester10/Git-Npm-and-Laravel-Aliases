### C:\Program Files\Git\etc\.gitconfig

    [alias]
    acm = "!f() { git add . && git commit -m \"$(echo $@)\"; }; f";
    com = checkout master
    cob = checkout -b
    b = branch

    p = push
    pl = pull

    s = status

    # Undo a `git push`
    	undopush = push -f origin HEAD^:master;

    # Undo merge
    undomerge = reset --hard HEAD@{1};

    # Undo changes not commited
    undo = reset --hard;

    # Undo last commit and remove from stage
    # Example
    # git unstage file1 file2 ...
    unstage = reset HEAD -- #file;

### From C:\Program Files\Git\etc\bash.bashrc

### Alias for composer

    alias c="composer"
    alias cr="composer require"
    alias ci="composer install"
    alias cda="composer dump-autoload"
    alias cu="composer update"

# Alias for artisan commands

    alias pa="php artisan"
    alias pas="php artisan serve"
    alias pam="php artisan migrate"
    alias pamf="php artisan migrate:fresh"
    alias pamm="php artisan make:migration"
    alias pamc="php artisan make:controller"
    alias model="php artisan make:model"
    alias middleware="php artisan make:middleware"
    alias routes="php artisan route:list"
    alias pakg="php artisan key:generate"
    alias pamt="php artisan make:test"
    alias pads="php artisan db:seed"
    alias seeder="php artisan make:seeder"

# Alias for git commands

    alias g="git"

# Alias for npm commands

    alias ni="npm install"
    alias watch="npm run watch"
    alias prod="npm run prod"
    alias dev="npm run dev"
