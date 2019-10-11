# Commit Changes

<pre>
$ git add .
$ git commit -m " "
$ git push master
</pre>

# Run Unit Tests

Run all test:

<pre>$ vendor/bin/phpunit</pre>

Run one test class:

<pre>$ vendor/bin/phpunit tests/Unit/Phase1/H2Phase1Test.php</pre>

# Deploy to Production

Discard changes in production:

<pre>git reset --hard</pre>

Deploy changes in the server:

Reference: https://laraveldaily.com/how-to-deploy-laravel-projects-to-live-server-the-ultimate-guide/

<pre>
cd /home/forge/deploymentdemo.laraveldaily.com
php artisan down
git pull origin master
composer install 
php artisan migrate
php artisan cache:clear
php artisan queue:restart
php artisan up
</pre>

# Clone specific branch

<pre>git clone --single-branch --branch <branchname> <remote-repo></pre>

# Commit to a specific branch


